# What are Data Buckets?

* Data buckets are a replacement to the well-known `qglobals`, but they are far more performant, reliable and simpler to use

* You can use data buckets to store values unique to anything you would like, for example
  * NPC based flags
  * Zone based flags
  * Character based flags 
  * etc.

# Functions

* Data buckets exist in these 3 main functions in both Perl and LUA

```
get_data(std::string bucket_key)
set_data(std::string bucket_key, std::string bucket_value, std::string expires_in)
delete_data(std::string bucket_key)
```

# Storage

* Data buckets are stored in the [[data_buckets]] table and has a very simple structure
  * **id**
  * **key**
  * **value**
  * **expires**

* Expired data bucket rows will not be queryable via the quest API, they may exist in a table until 5-10 minutes have past and the server will garbage collect and wipe the table clean of expired buckets

# Usage Examples

### Perl

* In this simple example you can see that we are keying by character id to set the flag to make this unique per player, we are setting it with the value of 70, and since we didn't set the optional value of unix time it never expires

```perl
if ($text =~/character-flag-test/i) {
    $key = $client->CharacterID() . "-some-epic-flag";
    quest::set_data($key, 70);
    quest::say("You have traveled far! You have a mighty (" . quest::get_data($key) . ") epic points!");
}
```

![image](https://user-images.githubusercontent.com/3319450/42416821-8cef6690-823e-11e8-8b78-caec1a213f71.png)


### LUA

* In this example below you can see that we set a simple global flag, we immediately access it, delete it and then try to unsuccessfully access it again because the bucket data had already been deleted

```lua
if (e.message:findi("test")) then
    e.self:Say("This is a test!")
    eq.set_data("lua_test_key", "lua_value");
    e.self:Say("We just set some bucket data with '".. eq.get_data("lua_test_key") .. "'");
    eq.delete_data("lua_test_key");
    e.self:Say("I'm going to try and access the value again... '".. eq.get_data("lua_test_key") .. "'");
end
```

![image](https://user-images.githubusercontent.com/3319450/42416831-a726d71e-823e-11e8-92d5-cad58040e00c.png)

# Ways to Key Buckets

* Keying is simply a way to uniquely identify a flag, if you want to make some data unique to a player, then you would need something to key uniquely to that player, such as their **character_id**. If you wanted to set a flag uniquely for a NPC for example, you could use the **npc_type_id**, for a zone you could use the **zone_id**. All of these circumstances are completely up to you and you have the entire Quest API to grab something that can make something unique!

Some of the examples below should give you some ideas!

**By Character**

```perl
$key   = $client->CharacterID() . "-some-flag";
$value = 70;
quest::set_data($key, $value);
```

**By Door (And Zone)**

```perl

sub EVENT_CLICKDOOR {
    quest::say($doorid);
    if ($doorid == 4) {
        $key   = $zoneid . '-' . $doorid . '-last-person-to-click-door";
        $value = $client->GetCleanName();

        if (quest::get_data($key)) {
            $client->Message(15, "You know... the last person to click this door was '" . quest::get_data($key) . "'");
        }

        quest::set_data($key, $value);
    }
}
```

**Result**

![image](https://user-images.githubusercontent.com/3319450/42416886-d2caadae-823f-11e8-9b49-a6bd21bf8f73.png)

**Database Result**

![image](https://user-images.githubusercontent.com/3319450/42416888-dfd7a966-823f-11e8-8fc6-1829ed0c35c3.png)

**By NPC**

```perl
sub EVENT_DEATH_COMPLETE {
    $key = $npc->GetNPCTypeID() . "-death-count";
    quest::set_data($key, quest::get_data($key) + 1);

    $death_count = quest::get_data($key);
    quest::shout("Man! I've died (" . $death_count . ") times in my lifetime!");
}
```

**Result**

![image](https://user-images.githubusercontent.com/3319450/42416932-0eab7a32-8241-11e8-8b64-14d76a2c596f.png)

**Database**

![image](https://user-images.githubusercontent.com/3319450/42416937-21a01aee-8241-11e8-9c29-9a2e1ed4356d.png)

# Expiration Examples

* Below in this LUA example we will count the number of times a player has talked to an NPC, first by checking if we've got a bucket set at all, if not we will set an expiration time on it. Each time we call set_data, it will not over-ride the original expiration time unless we pass a new time parameter

```lua
function event_say(e)
	if (e.message:findi("hail")) then

		-- Set unique key for the bucket
		local key = e.other:GetCleanName() .. "_times_talked";

		-- If the bucket is empty, we need to set it
		-- The first time we will set an expiration on this (86400 seconds)
		if (eq.get_data(key) == "") then
			eq.set_data(key, '1', 86400);
		end

		local times_talked = tonumber(eq.get_data(key));

		e.self:Say("You know... You've talked to me " .. times_talked .. " time(s) today, get a life will ya!");

		-- Increment times talked
		eq.set_data(key, tostring(times_talked + 1));
	end

end
```

**Result**

![image](https://user-images.githubusercontent.com/3319450/42417093-750ed16c-8245-11e8-91f2-4746d2568ddb.png)

**Database**

![image](https://user-images.githubusercontent.com/3319450/42417095-89907c12-8245-11e8-9d5e-0090c0c24527.png)

### Acceptable Time Formats

We have the ability to use time shorthands if need-be, the following are acceptable time inputs

|Input|Time Result|
|---|---|
| 15s | 15 seconds |
| s15 | 15 seconds |
| 60m | 60 minutes |
| 7d  | 7 days |
| 1y  | 1 year |
| 600 | 600 seconds |

### Perl Expiration

* To set an expiration time in Perl, very similarly to the LUA example above, you would simply call your `set_data` function with an expiration flag as your 3rd parameter like so

```perl
quest::set_data("my_example_flag", "some_value", 3600); # 3600 seconds = 1 hour (Expire in 1 hour)
```

# Benchmarks

* Below are some simple benchmarks used to calculate performance. While even these numbers could be greatly optimized yet, these are plenty good for most use cases that server operators need. If you need even faster temporary data storage within the context of a zone, I would suggest using [[Entity Variables]] as they operate purely in memory

![image](https://user-images.githubusercontent.com/3319450/42429025-83c1d260-82fc-11e8-804f-f7490ac23600.png)

```perl
sub EVENT_SAY {
    use Time::HiRes;
    my $start = [ Time::HiRes::gettimeofday() ];

    if ($text =~ /random-write/i) {
        my $iterations = 1000;
        my $key_range = 100;
        quest::debug("Testing random-write... Iterations: (" . plugin::commify($iterations) . ") Key Range: " . $key_range);
        for ($i = 0; $i < $iterations; $i++) {
            quest::set_data("key_" . int(rand($key_range)), &generate_random_string(100));
        }
    }

    if ($text =~ /sequential-write/i) {
        my $iterations = 1000;
        quest::debug("Testing sequential-write... Iterations: (" . plugin::commify($iterations) . ")");
        for ($i = 0; $i < $iterations; $i++) {
            quest::set_data("key_" . $i, &generate_random_string(100), 15);
        }
    }

    if ($text =~ /sequential-read/i) {
        my $iterations = 1000;
        quest::debug("Testing sequential-read... Iterations: (" . plugin::commify($iterations) . ")");
        for ($i = 0; $i < $iterations; $i++) {
            $data = quest::get_data("key_" . $i);
            # if ($data ne "") {
            #     quest::say("Data for $i : $data");
            # }
        }
    }

    if ($text =~ /random-read/i) {
        my $iterations = 1000;
        quest::debug("Testing random-read... Iterations: (" . plugin::commify($iterations) . ")");
        for ($i = 0; $i < $iterations; $i++) {
            $data = quest::get_data("key_" . int(rand($iterations)));
        }
    }

    my $elapsed = Time::HiRes::tv_interval($start);
    quest::debug("Operation took: " . $elapsed);
}
```