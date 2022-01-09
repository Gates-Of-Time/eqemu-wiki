#ProTip: hit ctrl + f (Windows) or ⌘ + f (Mac) to FIND something on this page

# List of EVENTs

A full list can always be found in the EQEmu source [https://github.com/EQEmu/Server/blob/master/zone/embparser.cpp](https://github.com/EQEmu/Server/blob/master/zone/embparser.cpp)

| Event Name | Event Trigger |
| --- | --- |
| [EVENT_AGGRO](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_aggro) | When a mob aggros a client.
| [EVENT_AGGRO_SAY](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_aggro_say) | When a mob is targeted, the player types something, and NPC is in combat.
| [EVENT_ATTACK](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_attack) | When the NPC is attacked.
| [EVENT_AUGMENT_ITEM](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_augment_item) | When a client augments an item.
| [EVENT_AUGMENT_INSERT](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_augment_insert) | When a client inserts an augment into an item.
| [EVENT_AUGMENT_REMOVE](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_augment_remove) | When a client removes an augment from an item.
| [EVENT_CAST](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_cast) | Triggered when a client casts a spell.
| [EVENT_CAST_BEGIN](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_cast_begin) | When a client begins to cast a spell.
| [EVENT_CAST_ON](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_cast_on) | When a player casts a spell on a player or NPC.
| [EVENT_CLICKDOOR](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_clickdoor) | When the client clicks on a door object.
| [EVENT_CLICK_OBJECT](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_click_object) | When the client clicks on an object.
| [EVENT_COMBAT](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_combat) | When an NPC enters or leaves combat.
| [EVENT_COMBINE_FAILURE](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_combine_failure) | When a combine is unsuccessful.
| [EVENT_COMBINE_SUCCESS](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_combine_success) | When a combine is successful.
| [EVENT_COMMAND](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_command) | When a player says anything like a command. 
| [EVENT_CONNECT](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_connect) | When a player connects to the world.
| [EVENT_DEATH](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_death) | When the NPC dies. Fires before death finishes.
| [EVENT_DEATH_COMPLETE](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_death_complete) | When the NPC dies.
| [EVENT_DEATH_ZONE](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_death_zone) | When an NPC dies (used by the zone controller).
| [EVENT_DESTROY_ITEM](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_destroy_item) | When a client destroys an item.
| [EVENT_DISCONNECT](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_disconnect) | When a player disconnects from the world.
| [EVENT_DISCOVER_ITEM](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_discover_item) | When an item is discovered.
| [EVENT_DROP_ITEM](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_drop_item) | When a client drops an item.
| [EVENT_DUEL_LOSE](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_duel_lose) | When a client loses a duel.
| [EVENT_DUEL_WIN](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_duel_win) | When a client wins a duel.
| [EVENT_ENTER](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_enter) | When a client enters a mob's proximity.
| [EVENT_ENTER_AREA](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_enter_area) | When a client enters the area of a mob.
| [EVENT_ENTERZONE](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_enterzone) | When a player enters the zone.
| [EVENT_ENVIRONMENTAL_DAMAGE](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_environmental_damage) | When taking any sort of environmental damage.
| [EVENT_EQUIP_ITEM](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_equip_item) | When a player equips an item.
| [EVENT_EXIT](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_exit) | When a client leaves a mob's proximity.
| [EVENT_FEIGN_DEATH](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_feign_death) | When a client feign death.
| [EVENT_FISH_FAILURE](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_fish_failure) | When a client fails at fishing.
| [EVENT_FISH_START](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_fish_start) | When a client starts fishing.
| [EVENT_FISH_SUCCESS](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_fish_success) | When a client succeeds at fishing.
| [EVENT_FORAGE_FAILURE](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_forage_failure) | When a client fails at foraging.
| [EVENT_FORAGE_SUCCESS](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_forage_success) | When a client succeeds at foraging.
| [EVENT_GROUP_CHANGE](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_group_change) | When a group change occurs.
| [EVENT_HATE_LIST](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_hate_list) | When a mob's hate list is changed.
| [EVENT_HP](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_hp) | When a mob's HP drops below a threshold.
| [EVENT_ITEM](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_item) | When an item or money is turned into the mob.
| [EVENT_ITEM_CLICK](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_item_click) | When an item is clicked.
| [EVENT_ITEM_CLICK_CAST](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_item_click_cast) | When a client casts the click effect on an item.
| [EVENT_ITEM_ENTER_ZONE](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_item_enter_zone) | Called when an item that would trigger EVENT_SCALE_CALC is in the inventory when a player zones in.
| [EVENT_ITEM_TICK](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_item_tick) | When the click effect of an item ticks.
| [EVENT_KILLED_MERIT](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_killed_merit) | When an NPC dies and the client is in a group credited with doing the most damage.
| [EVENT_LEAVE_AREA](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_leave_area) | When a client leaves a mob's area.
| [EVENT_LEVEL_UP](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_level_up) | When the player gains a level.
| [EVENT_LOOT](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_loot) | When a player successfully loots an item from a corpse.
| [EVENT_NPC_SLAY](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_npc_slay) | When an NPC slays another NPC.
| [EVENT_PLAYER_PICKUP](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_player_pickup) | When a player picks up an object from the ground.
| [EVENT_POPUPRESPONSE](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_popupresponse) | When a player clicks a button on a popup.
| [EVENT_PROXIMITY_SAY](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_proximity_say) | When a client enters a mob's proximity and uses an appropriate text trigger.
| [EVENT_RESPAWN](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_respawn) | Triggered on respawn.
| [EVENT_SAY](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_say) | When a mob is targeted and the player types something.
| [EVENT_SCALE_CALC](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_scale_calc) | When an item is equipped.
| [EVENT_SIGNAL](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_signal) | When a signal is received.
| [EVENT_SLAY](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_slay) | Whenever an NPC kills a player.
| [EVENT_SPAWN](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_spawn) | When the NPC spawns.
| [EVENT_SPAWN_ZONE](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_spawn_zone) | When the NPC spawns (used by the zone controller).
| [EVENT_SPELL_EFFECT_CLIENT](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_spell_effect_client) | When the spell lands on a client.
| [EVENT_SPELL_EFFECT_NPC](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_spell_effect_npc) | When the spell lands on an NPC.
| [EVENT_SPELL_EFFECT_BUFF_TIC_CLIENT](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_spell_effect_buff_tic_client) | When the spell ticks on a client.
| [EVENT_SPELL_EFFECT_BUFF_TIC_NPC](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_spell_effect_buff_tic_npc) | When the spell ticks on an NPC.
| [EVENT_SPELL_EFFECT_TRANSLOCATE_COMPLETE](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_spell_effect_translocate_complete) | When translocation is complete.
| [EVENT_SPELL_FADE](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_spell_fade) | When a spell fades.
| [EVENT_TARGET_CHANGE](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_target_change) | When a mob changes their current target or clears it.
| [EVENT_TASKACCEPTED](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_taskaccepted) | When a player accepts a task from the task selector window.
| [EVENT_TASK_COMPLETE](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_task_complete) | When a player completes a task.
| [EVENT_TASK_FAIL](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_task_fail) | When a player fails a task.
| [EVENT_TASK_STAGE_COMPLETE](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_task_stage_complete) | When a task stage is completed.
| [EVENT_TASK_UPDATE](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_task_update) | When a player's task is updated.
| [EVENT_TIMER](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_timer) | When the duration of a timer elapses.
| [EVENT_TRADE](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_trade) | When a client begins a trade.
| [EVENT_UNAUGMENT_ITEM](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_unaugment_item) | When a client removes an augment from an item.
| [EVENT_UNEQUIP_ITEM](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_unequip_item) | When a client unequips an item.
| [EVENT_USE_SKILL](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_use_skill) | When a client uses a skill
| [EVENT_WAYPOINT_ARRIVE](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_waypoint_arrive) | When a mob arrives at a waypoint.
| [EVENT_WAYPOINT_DEPART](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_waypoint_depart) | When a mob leaves a waypoint.
| [EVENT_WEAPON_PROC](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_weapon_proc) | When a weapon procs.
| [EVENT_ZONE](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events#event_zone) | When a player zones.

# EVENT Documentation

## EVENT_AGGRO
### Trigger 

- When a mob aggros a client.  

Often used for flavor text--just remember that every NPC_Type has an EmoteID that can often handle this behavior.  

### Example

- In this example, the NPC will say "Time to die PlayerName." when the NPC is aggro'd by the player.

```perl
sub EVENT_AGGRO {
	quest::say("Time to die $name.");
}
```

## EVENT_AGGRO_SAY
### Trigger

- When a mob is targeted, the player types something, and NPC is in combat.

### Exports

| Name | Type | Usage
| --- | --- | ---
|data | int | `quest::say($data); # returns int`
|text | int | `quest::say($text); # returns int`
|langid | int | `quest::say($langid); # returns int`

### Example

- In this example, the NPC, if in combat, would say the names of everyone on its hate list, and include both the amount of damage the entity has done, as well as the amount of hate the entity has generated.

```perl
sub EVENT_AGGRO_SAY {
	#:: Match when a player says "hate", case insensitive because of the /i
	if ($text=~/hate/i) {
	#:: Create an array for all entities on the NPC's hatelist
	my @hatelist = $npc->GetHateList();
		foreach $ent (@hatelist) {
			#:: The entity name
			my $h_ent = $ent->GetEnt();
			#:: The entity's total damanage
			my $h_dmg = $ent->GetDamage();
			#:: The entity's total hate
			my $h_hate = $ent->GetHate();
			#:: Match if entities exist on the hate list
			if ($h_ent) {
				#:: Create a scalar to store the clean name ("Turmoiltoad" vs. "Turmoiltoad001")
				my $h_ent_name = $h_ent->GetCleanName();
				quest::say("$h_ent_name is on my hate list with $h_hate hate and $h_dmg damage.");
			}
		}
    	}
}
```

## EVENT_ATTACK
### Trigger

- When the NPC is attacked.  

Note the subtle difference from EVENT_AGGRO, which is triggered when the NPC is aggro'd (which could occur through bad faction, for instance).

### Example

- In this example, the NPC will say "Time to die PlayerName." when the NPC is attacked by the player.

```perl
sub EVENT_ATTACK {
	quest::say("Time to die $name.");
}
```
## EVENT_AUGMENT_ITEM

### Trigger

- When a client augments an item.  

You would likely use this event in your global player.pl file.

### Example

- In this example, a message in yellow text is displayed to the client when the player adds an augment to an item.

```perl
sub EVENT_AUGMENT_ITEM {
	$client->Message(15, "Yay, it fit!");
}
```

## EVENT_AUGMENT_INSERT

### Trigger

- When a client inserts an augment into an item.  

You would likely use this event in your global player.pl file.

### Example

- In this example, a message in yellow text is displayed to the client when the player puts the augment into the augment slot of an item.

```perl
sub EVENT_AUGMENT_INSERT {
	$client->Message(15, "Yay, it fit!");
}
```

## EVENT_AUGMENT_REMOVE

### Trigger

- When a client removes an augment from an item.  You would likely use this event in your global player.pl file.

### Example

- In this example, a message in yellow text is displayed to the client when the player removes an augment from an item.

```perl
sub EVENT_AUGMENT_REMOVE {
	$client->Message(15, "Yay, you pulled it out!");
}
```

## EVENT_CAST

### Trigger

- When a client casts a spell.  

### Exports

|Name | Type | Usage
| --- | --- | ---
|spell_id | int	| `quest::say($spell_id); # returns int`

### Example

- In this example, the player would emote upon a successful cast.  

```perl
sub EVENT_CAST {
	quest::me("regains his concentration and casts his spell.");
}
```

## EVENT_CAST_BEGIN

### Trigger

- When a client begins to cast a spell.

### Exports

|Name | Type | Usage
| --- | --- | ---
|spell_id | int	| `quest::say($spell_id); # returns int`

### Example

- In this example, the player would emote if they begin casting the gate spell.  You would likely place this particular snippet into your global player.pl file.

```perl
sub EVENT_CAST_BEGIN {
	#:: Match if spell is 36 - Gate
	if ($spell_id == 36) {
		quest::me("begins casting the GATE spell");
	}
}
```

## EVENT_CAST_ON

### Trigger

- When a player casts a spell on a player or NPC.

### Exports

|Name | Type | Usage
| --- | --- | ---
|spell_id | int	| `quest::say($spell_id); # returns int`

### Example

- In this example, if the player casts Banish Summoned on an NPC with a Summoned body type, the NPC will be killed. If you were placing this snippet in an NPC's quest script, you likely wouldn't bother matching body type.

```perl
sub EVENT_CAST_ON {
	#:: Match if spell is 116 - Banish Summoned
	if ($spell_id == 116) {
		#:: Match if the NPC's body type is 28 - Summoned Creature
		if ($mob->GetBodyType() == 28) {
			$npc->Kill();
		} 
		else {
			$client->Message(13, "This spell only effects summoned creatures");
		}
	}
}
```

## EVENT_CLICKDOOR

### Trigger

- When the client clicks on a door object.  

Note that you would likely use this event in the zone player.pl file.  Since doors have open types and destination fields stored in the database, most "simple" doors do not require a separate quest script.  An example of a "simple" door would be any door that requires a single keyitem (by Item ID) to open, like the door to the basement in Befallen.

### Exports

|Name | Type | Usage
| --- | --- | ---
|doorid | int	| `quest::say($doorid); # returns int`
|version | int	| `quest::say($version); # returns int`

### Example

- In this example, a player who is part of a Deepest Guk Adventure would be teleported to Deepest Guk when they click the doorway found in the Hollow Log.

```perl
sub EVENT_CLICKDOOR {
	#:: Match if doorID is 1 - the door found in the Hollow Log that leads to Deepest Guk Adventures
	if ($doorid == 1) {
		#:: Create a variable to store the player's adventure zone instance ID
		$GukAInstance = quest::GetInstanceID("guka",50);
		#:: Match if the player has an instance
		if ($GukAInstance > 0) {
			#:: Teleport the player to their instance in Deepest Guk at the safe spot
			quest::MovePCInstance(229, $GukAInstance, 101, -841, 2.38);
		} 
		else {
			$client->Message(13, "You are not a part of a Deepest Guk adventure instance!");
		}
	}
}
```


## EVENT_CLICK_OBJECT

### Trigger

- When the client clicks on an object.  

Note the similarity between this event and Perl EVENT_CLICKDOOR, since it is easy to confuse a door object (like a Plane of Knowledge Book) with Objects (IE Pottery wheels, Brew Barrels, etc.).  You would likely use this event in the zone player.pl (or global_player.pl) files.

### Exports

|Name | Type | Usage
| --- | --- | ---
|objectid | int	| `quest::say($objectid); # returns int`
|clicker_id | int	| `quest::say($clicker_id); # returns int`

### Example

- In this example, a message is displayed to a player when they open the Ogre Cultural Forge in Oggok.

```perl
sub EVENT_CLICK_OBJECT {
        #:: Match to the ogre cultural forge in Oggok by object ID
        if ($objectid == 1075) {
                #:: Check to see if the player who clicked is a race other than Ogre
                if ($race ne "Ogre") {
                        #:: Send the client a message in color 1 (gray)
                        $client->Message(1,"The foul stench of Ogre overwhelms you as you open the forge.");
                }
                else {
                        $client->Message(1,"Mmmm--dis smells just like home.");
                }
        }
}
```

## EVENT_COMBAT

### Trigger

- When an NPC enters or leaves combat.

### Exports
|Name | Type | Usage
| --- | --- | ---
|combat_state | int | `quest::say($combat_state); # returns int`

### Example

- In this example, the NPC will say some flavor text when entering combat.

```perl
sub EVENT_COMBAT {
	#:: combat state 1 = True
	if ($combat_state == 1) {
		quest::say("Time to die $name!");
	}
}
```

## EVENT_COMBINE_FAILURE

### Trigger

- When a combine is unsuccessful.  You would likely use this event in your global / player.pl file.

### Exports

| Name | Type | Usage
| --- | --- | --- |
|recipe_id | int | `quest::say($recipe_id); # returns int`
|recipe_name | int | `quest::say($recipe_name); # returns int`

### Example

- In this example, we watch for a player failing the combine for a Hand Made Backpack and then tease them.

```perl
sub EVENT_COMBINE_FAILURE {
	#:: Match Recipe 2686: "Hand Made Backpack" by ID
	if ($recipe_id == 2686) {
		#:: Send the client a message in color 15 (yellow)
		$client->Message(15,"Awww...now where are you going to put all of your stuff?");
	}
}
```

## EVENT_COMBINE_SUCCESS

### Trigger

- When a combine is successful.

### Exports

| Name | Type | Usage
| --- | --- | --- |
|recipe_id | int | `quest::say($recipe_id); # returns int`
|recipe_name | int | `quest::say($recipe_name); # returns int`

### Example

- In this example, we send the client a message when they successfully combine a Hand Made Backpack

```perl
sub EVENT_COMBINE_SUCCESS {
	#:: Match Recipe 2686: "Hand Made Backpack" by ID
	if ($recipe_id == 2686) {
		#:: Send the client a message in color 15 (yellow)
		$client->Message(15,"Yay, now you have a place to put all of your stuff!");
	}
}
```

## EVENT_COMMAND

### Trigger

- When a player says anything like a command.  Replaced/Synonymous with [EVENT_SAY](https://github.com/EQEmu/Server/wiki/Perl-API---Perl-Sub-Event-Examples#event_say).

## EVENT_CONNECT

### Trigger

- when a player connects to the world.

You would likely be using this event in your global_player.pl.  

### Example

- In this example, veteran AAs are awarded based on accumulated play time.

```perl
sub EVENT_CONNECT {
	my %vet_aa = (481 => [31536000, 1, 1],
	482 => [63072000, 1, 1],
	483 => [94608000, 1, 1],
	484 => [126144000, 1, 1],
	485 => [157680000, 1, 1],
	486 => [189216000, 1, 1],
	487 => [220752000, 1, 1],
	511 => [252288000, 1, 1],
	2000 => [283824000, 1, 1],
	8081 => [315360000, 1, 1],
	8130 => [346896000, 1, 1],
	453 => [378432000, 1, 1],
	182 => [409968000, 1, 1],
	600 => [441504000, 1, 1]);
	foreach my $key (keys %vet_aa) {
		if ($vet_aa{$key}[2] && ($vet_aa{$key}[2] || $client->GetAccountAge() >= $vet_aa{$key}[0])) {
			$client->GrantAlternateAdvancementAbility($key, 1);
		}
	}
}
```

## EVENT_DEATH

### Trigger

- When the NPC dies. Fires before death finishes.

### Exports

| Name | Type | Details
| --- | --- | --- 
| client | client | client who killed mob
| npc | npc | npc that was killed
| killer_id | int | client ID of killer. (Does not seem castable to mob)
| killer_damage | int | How much damage was dealt on killing blow
| killer_spell | int | Spell ID used to kill mob
| killer_skill | int | Skill ID used to kill mob
| charid | int | Character ID who killed mob
| class | string | Class Name who killed mob
| faction | int | Faction comparison of killed mob vs killer
| h | float | heading of mob during death
| hpratio | float | percent health of mob after death (negative value)
| mlevel | int | level of mob killed
| mname | string | name of mob killed
| mobid | int | id of mob killed
| name | string | name of killer
| race | string | race of killer
| status | int | account status of killer
| uguild_id | int | uguild of killer
| ulevel | int | level of killer
| userid | int | user id of killer
| x | float | x position of killed mob
| y | float | y position of killed mob
| z | float | z position of killed mob
| zonehour | int | hour of zone when mob died
| zoneid | int | zone id where mob died
| zoneln | string | long name of zone where mob died
| zonemin | int | minimum level to enter zone where mob died
| zonesn | string | short name of zone where mob died
| zonetime | int | time of zone where mob died
| zoneweather | int | 

## EVENT_DEATH_COMPLETE

### Trigger

- When the NPC dies.

Often used to spawn adds or send signals upon the death of an NPC.

### Exports

| Name | Type | Usage
| --- | --- | ---
| killer_id | int | `quest::say($killer_id); # returns int `
| killer_damage | int | `quest::say($killer_damage); # returns int`
| killer_spell | int | `quest::say($killer_spell); # returns int`
| killer_skill | int | `quest::say($killer_skill); # returns int`

### Example

- In this example, we spawn a fire beetle after the death of our NPC at the NPC's location.

```perl
sub EVENT_DEATH_COMPLETE {
	#:: Spawn a 2024 - a_fire_beetle by NPC Type ID, grid 0, guildwarset 0, current X, Y, Z, and heading
	quest::spawn2(2024,0,0,$x,$y,$z,$h);
}
```

## EVENT_DEATH_ZONE

### Trigger

- When the NPC dies.

**Used by the zone controller.**

### Exports

| Name | Type | Usage
| --- | --- | ---
| killer_id | int | `quest::say($killer_id); # returns int `
| killer_damage | int | `quest::say($killer_damage); # returns int`
| killer_spell | int | `quest::say($killer_spell); # returns int`
| killer_skill | int | `quest::say($killer_skill); # returns int`
| killer_npc_id | int | `quest::say($killer_npc_id); # returns int`

## EVENT_DESTROY_ITEM

### Trigger

- When a client destroys an item.

Used mainly for logging purposes.

## EVENT_DISCONNECT

### Trigger

- When a player disconnects from the world.

Used mainly for logging purposes.

## EVENT_DISCOVER_ITEM

### Trigger

- When an item is discovered.

Used in conjunction with World Rule EnableDiscoveredItems.

### Exports

| Name | Type | Usage
| --- | --- | ---
| itemid | int | `quest::say($itemid); # returns int`

### Example

```perl
sub EVENT_DISCOVER_ITEM {
	#:: Create a scalar variable to store the item link
	$discovereditem = quest::varlink($itemid);
	#:: Shout the discovery to all zones
	quest::shout2("$name has discovered $discovereditem!  Yay!");
}
```

## EVENT_DROP_ITEM

### Trigger

- When a client drops an item.

Mainly used for logging purposes.

### Exports

| Name | Type | Usage
| --- | --- | ---
| quantity | int | `quest::say($quantity); # returns int`
| itemname | int | `quest::say($itemname); # returns int`
| itemid | int | `quest::say($itemid); # returns int`
| spell_id | int | `quest::say($spell_id); # returns int`
| slotid | int | `quest::say($slotid); # returns int`

## EVENT_DUEL_LOSE

### Trigger

- When a client loses a duel.

You would use this event in the global global_player.pl file.

### Example

- In this example, we set a quest global to keep track of a player's dueling failures.

```perl
sub EVENT_DUEL_LOSE {
	#:: Match if the player has a qglobal for duelslost
	if (!defined $qglobals{"duelslost"}) {
		#:: If no qglobal exists, set one
		quest::setglobal("duelslost",1,5,"F");
	}
	else {
		#:: If the qglobal exists, iterate the count up one
		quest::setglobal("duelslost",$qglobals{"duelslost"}+1,5,"F");
	}
}
```

## EVENT_DUEL_WIN

### Trigger

- when a client wins a duel.

You would use this event in the global global_player.pl file.

### Example

- In this example, we set a quest global to keep track of a player's dueling wins.

```perl
sub EVENT_DUEL_WIN {
	#:: Match if the player has a qglobal for duelswon
	if (!defined $qglobals{"duelswon"}) {
		#:: If no qglobal exists, set one
		quest::setglobal("duelswon",1,5,"F");
	}
	else {
		#:: If the qglobal exists, iterate the count up one
		quest::setglobal("duelswon",$qglobals{"duelswon"}+1,5,"F");
	}
}
```

## EVENT_ENTER

### Trigger

- When a client enters a mob's proximity (as defined by quest::set_proximity(min_x, max_x, min_y, max_y, min_z, max_z)).

### Example

- In this example, we first set the NPC's proximity; when a player enters the proximity, they become PVP (red).

```perl
sub EVENT_SPAWN {
	#:: Set the proximity bounds around the NPC on spawn, 200 units across
	$x = $npc->GetX();
	$y = $npc->GetY();
	quest::set_proximity($x - 100, $x + 100, $y - 100, $y + 100);
}

sub EVENT_ENTER {
	#:: Turn pvp on
	quest::pvp(on);
}
```

## EVENT_ENTER_AREA

### Trigger

- when a client enters the area of a mob.

## EVENT_ENTERZONE

### Trigger

- When a player enters the zone.  Likely you will add to the zone player.pl file.

### Example

- In this example we remove the LDON compass mark.

```perl
sub EVENT_ENTERZONE {
	#:: Clear the LDON Compass mark
	$client->ClearCompassMark();
}
```

- In this example we create a LDON compass mark

```perl
sub EVENT_ENTERZONE {
	#:: Create a scalar for storing the instance ID
	$RujDInstance = quest::GetInstanceID("rujd",50);
	#:: If the instance ID exists, it should be greater than 0--mark the player's compass if it is
	if ($RujDInstance > 0) {
		#:: Create a line on the compass leading the player to X,Y,Z
		$client->MarkCompassLoc(-157.09, 19.31, 100);
	}
}
```
## EVENT_ENVIRONMENTAL_DAMAGE

### Trigger

- When taking any sort of environmental damage.

### Exports

| Name | Type | Usage
| --- | --- | ---
| env_damage | int | `quest::say($env_damage); # returns int`
| env_damage_type | int | `quest::say($env_damage_type); # returns int`
| env_final_damage | int | `quest::say($env_final_damage); # returns int`

## EVENT_EQUIP_ITEM

### Trigger

- When a player equips an item.

## EVENT_EXIT

### Trigger

- When a client leaves a mob's proximity (as defined by quest::set_proximity).

### Example

- In this example, we first set the NPC's proximity; when a player exits the proximity, they are no longer PVP (blue).

### Example

```perl
sub EVENT_SPAWN {
	#:: Set the proximity bounds around the NPC on spawn, 200 units across
	$x = $npc->GetX();
	$y = $npc->GetY();
	quest::set_proximity($x - 100, $x + 100, $y - 100, $y + 100);
}

sub EVENT_EXIT {
	#:: Turn pvp off
	quest::pvp(off);
}
```

## EVENT_FEIGN_DEATH

### Trigger

- When a client feigns death.

### Example

```perl
sub EVENT_FEIGN_DEATH {
	#:: See if the player has a pet
	if ($client->GetPetID()) {
		#:: Identify the pet by ID and kill it
		$PetID = $entity_list->GetMobByID($client->GetPetID());
		$PetID->Kill();
	}
}
```

## EVENT_FISH_FAILURE

### Trigger

- When a client fails at fishing.

You would use this event in the zone player.pl file.

### Example

- In this example, a message is displayed by the client if fishing is unsuccessful.

```perl
sub EVENT_FISH_FAILURE {	
	$client->Message(1, "Maybe you're using the wrong bait!")
}
```

## EVENT_FISH_START

### Trigger

- when a client starts fishing.

You would use this event in the zone player.pl file.

### Example

- In this example, a message is displayed by the client if they start fishing.  

```perl
sub EVENT_FISH_START {
	$client->Message(1, "You crack a beer and toss your line in.");
}
```

## EVENT_FISH_SUCCESS

### Trigger

- when a client succeeds at fishing.

You would use this event in the zone player.pl file or the global global_player.pl file.

### Exports

|Name | Type | Usage
| --- | --- | ---
|fished_item | int | `quest::say($fished_item); # returns int`

### Example

- In this example, we set a quest global to keep track of a player's fishing successes.
- You would use this event in the global global_player.pl file.

```perl
sub EVENT_FISH_SUCCESS {
	#:: Match if the player has a qglobal for fishsuccess
	if (!defined $qglobals{"fishsuccesses"}) {
		#:: If no qglobal exists, set one
		quest::setglobal("fishsuccesses",1,5,"F");
	}
	else {
		#:: If the qglobal exists, iterate the count up one
		quest::setglobal("fishsuccesses",$qglobals{"fishsuccesses"}+1,5,"F");
	}
}
```

## EVENT_FORAGE_FAILURE

### Trigger

- When a client fails at foraging.

You would use this event in the zone player.pl or global global_player.pl file.

### Example

- In this example, we set a quest global to keep track of a player's foraging failures.

```perl
sub EVENT_FORAGE_FAILURE {
	#:: Match if the player has a qglobal for foragefails
	if (!defined $qglobals{"foragefails"}) {
		#:: If no qglobal exists, set one
		quest::setglobal("foragefails",1,5,"F");
	}
	else {
		#:: If the qglobal exists, iterate the count up one
		quest::setglobal("foragefails",$qglobals{"foragefails"}+1,5,"F");
	}
}
```

## EVENT_FORAGE_SUCCESS

### Trigger

- when a client succeeds at foraging.

You would use this event in the zone player.pl file or the global global_player.pl file.

### Exports

|Name | Type | Usage
| --- | --- | ---
|foraged_item | int | `quest::say($foraged_item); # returns int`

### Example

- In this example, we set a quest global to keep track of a player's foraging successes.

```perl
sub EVENT_FORAGE_SUCCESS {
	#:: Match if the player has a qglobal for foragesuccess
	if (!defined $qglobals{"foragesuccesses"}) {
		#:: If no qglobal exists, set one
		quest::setglobal("foragesuccesses",1,5,"F");
	}
	else {
		#:: If the qglobal exists, iterate the count up one
		quest::setglobal("foragesuccesses",$qglobals{"foragesuccesses"}+1,5,"F");
	}
}
```

## EVENT_GROUP_CHANGE

### Trigger

- when a group change occurs.

## EVENT_HATE_LIST

### Trigger

- When a mob's hate list is changed.

### Exports

|Name | Type | Usage
| --- | --- | ---
|hate_state | int | `quest::say($hate_state); # returns int`

### Example

In this example, some flavor text is added as a player is added and removed from the NPC's hate list.

```perl
sub EVENT_HATE_LIST {
	if ($hate_state == 1) {
		quest::say("$name is gonna die!");
	}
	if ($hate_state == 0) {
		quest::say("$name is no match for my might!");
	}
}
```

## EVENT_HP

### Trigger

- When a mob's HP dropping below a threshold (as defined by quest::setnexthpevent()).  

### Exports

|Name | Type | Usage
| --- | --- | ---
|hpevent | int | `quest::say($hpevent); # returns int`
|inchpevent | int | `quest::say($inchpevent); # returns int--incoming HP event`

### Example

- In this example, we set the HP event threshold, and then depop the mob when the threshold is reached.

```perl
sub EVENT_SPAWN {
	#:: Set the HP event threshold for 50 percent health
	quest::setnexthpevent(50);
}

sub EVENT_HP {
	#:: Match when the threshold is met
	if ($hpevent == 50) {
		quest::depop();
	}
}
```

## EVENT_ITEM

### Trigger

- When an item or money is turned into the mob.

### Example

- In this example, we turn in 3250 gold, a Ring of the Ancients, and a Shadowed Rapier in exchange for our Journeyman's Boots

```perl
sub EVENT_ITEM {
	#:: Create a scalar variable to store cash--only gold and platinum
	my $cash = (($platinum * 10) + $gold);
 	#:: Match if the cash is 3250gp or more
	if ($cash >= 3250) {
		#:: Match turn for 12268 - Ring of the Ancients and 7100 - Shadowed Rapier
		if (plugin::check_handin(\%itemcount, 12268 => 1, 7100 => 1)) {
			quest::say("The time to trade has come!! I am now rich and you are now fast. Take the Journeyman Boots and run like the wind.");
			#:: Give a 2300 - Journeyman's Boots
			quest::summonitem(2300);
			#:: Play the ding sound
			quest::ding();
			#:: Grant a small amount of experience
			quest::exp(1250);
      		}
	}
	else {
		#:: Return unused coin
		quest::givecash(0, 0, $gold, $platinum);
	}
	#:: Return unused items
	plugin::return_items(\%itemcount);
} 
```

## EVENT_ITEM_CLICK

### Trigger

- When an item is clicked.

This is a useful script to put in the Global quest scripts directory, so that you can make an item click work anywhere in the world.

### Exports

| Name | Type | Usage
| --- | --- | --- 
| itemid | int | `quest::say($itemid); # returns int`
| itemname | int | `quest::say($itemname); # returns int`
| slotid | int | `quest::say($slotid); # returns int`
| spell_id | int | `quest::say($spell_id); # returns int`

### Example

- This example is taken from the Evil Eye Costume Kit, which is part of the Halloween Costume illusion items.
- Note that the scriptfileid field for the item is set to 30073 in the database.
- Note that a corresponding quest file exists at global/items/script_30073.pl.

```perl
sub EVENT_ITEM_CLICK {
	#::: Use == for numeric comparison to Item ID 54711 - Evil Eye Costume Kit
	if ($itemid == 54711) {
		#::: Change the player's race to 469 - Evil Eye
		quest::playerrace(469);
	} 
}
```

## EVENT_ITEM_CLICK_CAST

### Trigger

- When a client casts the click effect on an item.

### Exports

| Name | Type | Usage
| --- | --- | --- 
| itemid | int | `quest::say($itemid); # returns int`
| itemname | int | `quest::say($itemname); # returns int`
| slotid | int | `quest::say($slotid); # returns int`
| spell_id | int | `quest::say($spell_id); # returns int`

## EVENT_ITEM_ENTER_ZONE
Called when an item that would trigger EVENT_SCALE_CALC is in the inventory when a player zones in.

## EVENT_ITEM_TICK

### Trigger

- when the click effect of an item ticks.

## EVENT_KILLED_MERIT

### Trigger

- On NPC death and applies to the group that did the most damage to the NPC (IE the group that got XP for the kill, assuming there was XP; or the group that gets loot rights to the NPC, assuming that there was loot). Although not often used, this event gives you the opportunity to assign quest globals (for character flags) or update tasks.

### Example

```perl
sub EVENT_KILLED_MERIT {
	#:: Get the name of the mob to use in the quest global
	my $slain = $npc->GetCleanName();
	#:: Set the quest global--this would apply to all group members
	$client->SetGlobal($slain,1,5,"F");
	#:: Display an emote message to each client in yellow to notify them that they received credit
	$client->Message(15, "You have received credit for killing ".$slain.".");
}
```

## EVENT_LEAVE_AREA

### Trigger

- when a client leaves a mob's area.

## EVENT_LEVEL_UP

### Trigger

- When the player gains a level.

```perl
sub EVENT_LEVEL_UP {
	#:: Shout the level up to all zones
	quest::shout2("$name has gained a level!  Welcome to $ulevel");
}
```

## EVENT_LOOT

### Trigger

- when player successfully loots an item from a corpse.

### Exports

|Name | Type | Usage
| --- | --- | ---
|looted_id | int | `quest::say($looted_id); # returns int`
|looted_charges | int | `quest::say($looted_charges); # returns int`
|corpse | int | `quest::say($corpse); # returns int`

### Example

- This example uses the loot event to match a particular item and corpse.

Note that we use the NPC's name (Fippy_Darkpaw) and not the numeric corpse ID (IE 249) or full corpse name (IE Fippy_Darkpaw`s_corpse249).

```perl
sub EVENT_LOOT {
	#::: Use == for numeric comparison to Item ID 60396 - Fippy's Paw
	#::: Use eq for string comparison to Fippy_Darkpaw's corpse
	if ($looted_id == 60396 && $corpse eq "Fippy_Darkpaw") {
		$client->Message(15, "The bloody stump of Fippy's paw--it's a lot smaller than you thought it would be.");
	}
}
```

## EVENT_NPC_SLAY

### Trigger

- When an NPC slays another NPC.

### Exports

|Name | Type | Usage
| --- | --- | ---
|killed | int | `quest::say($killed); # returns int NPCTypeID`

### Example

- In this example, we add some flavor text when the Exterminator kills the rats.

```perl
sub EVENT_NPC_SLAY {
	quest::say("Another unworthy opponent. Never cross Mining Guild 628!!");
}
```

## EVENT_PLAYER_PICKUP

### Trigger

- When a player picks up an object from the ground.  You would likely use this event in your zone player.pl file.

### Exports

|Name | Type | Usage
| --- | --- | ---
|picked_up_id | int | `quest::say($picked_up_id); # returns int`
|picked_up_entity_id | int | `quest::say($picked_up_entity_id); # returns int`

### Example

-- In this example, when the player picks up a Chalice of Conquest, a signal is sent to another NPC

```perl
#:: Chalice of Conquest quest
sub EVENT_PLAYER_PICKUP {
	#:: Match 12274 - Chalice of Conquest, ground spawn created by #Captain_Klunga.pl
	if ($picked_up_id == 12274) {
		#:: Send a signal to Dagnor's Cauldron >> #Captain_Klunga (70072)
		quest::signal(70072,1);
	}
}
```

## EVENT_POPUPRESPONSE

### Trigger

- When a player clicks a button on a popup.

Used with quest::popup.

### Exports

|Name | Type | Usage
| --- | --- | ---
|popupid | int | `quest::say($popupid); # returns int`

### Example

- a well-known example from the Guild Lobby portal pool.

```perl
sub EVENT_POPUPRESPONSE {
	#:: Triggered by sub EVENT_ENTER: quest::popup('Teleport', 'Teleport to The Plane of Hate?', 666, 1, 0);
	if ($popupid == 666) {
		#:: Teleport the player to hateplaneb
		quest::movepc(186,-393,656,3);
	}
}
```

## EVENT_PROXIMITY_SAY

### Trigger

- When the client enters a mob's proximity and uses the appropriate text trigger supplied beneath this event. 

Note that you must enable quest::set_proximity().

### Example

- In this example, we establish a proximity around the NPC and enable the NPC to listen for say messages in the proximity (IE without having the mob targeted, necessarily); we then match for a "hail" message and attack anyone foolish enough to say hello.

```perl
sub EVENT_SPAWN {
     #:: Grab the NPC's location
     $x = $npc->GetX();
     $y = $npc->GetY();
     $z = $npc->GetZ();
     #:: Enable proximity 30 units across, 30 units high, and turn on proximity say
     quest::set_proximity($x-15, $x+15, $y-15, $y+15, $z-15, $z+15, 1);
}

sub EVENT_PROXIMITY_SAY {
	#:: Match say message for "hail", /i for case insensitive
	if ($text=~/hail/i) {
		quest::say("Hello, $name!");
	}
}
```

## EVENT_RESPAWN

### Trigger

- on respawn

### Exports

|Name | Type | Usage
| --- | --- | ---
|option | int | `quest::say($option); # returns int`
|resurrect | int | `quest::say($resurrect); # returns int`

## EVENT_SAY

### Trigger

- when a mob is targeted and the player types something.

### Exports

| Name | Type | Details
| --- | --- | ---
| client | client | Client who did say event
| npc | npc | Npc who is handling say event
| charid | int | character id of who did say event
| class | string | class of who did say event
| data | int | unknown? 124078
| faction | int | faction comparison of who did say and npc
| h | float | heading position of npc
| hpratio | float | hp ratio e.g. 100
| instanceid | int | instance id of zone, typically 0
| instanceversion | int | instance version of zone, typically 0
| langid | int | language id, common is 0
| mlevel | int | mob level of npc
| mname | string | mob name of npc
| mobid | int | mob entity id of npc
| name | string | name of who did say event
| race | string | race of who did say event
| status | int | account status of who did say event
| text | string | Text of who did say event
| uguild_id | int | guild id of who did say event
| uguildrank | int | guild rank of who did say event
| ulevel | int | level of who did say event
| userid | int | user id of who did say event
| x | float | x position of npc
| y | float | y position of npc
| z | float | z position of npc
| zonehour | int | hour of zone when mob died
| zoneid | int | zone id where mob died
| zoneln | string | long name of zone where mob died
| zonemin | int | minimum level to enter zone where mob died
| zonesn | string | short name of zone where mob died
| zonetime | int | time of zone where mob died
| zoneweather | int | weather of zone where mob died

### Example

- This example is a response to a "hail"

```perl
sub EVENT_SAY {
     #::: Checks if the text is like "Hail", the "/i" is for case-insensitive.
     if ($text=~/Hail/i) {
          quest::say("Hello, $name!");
     }
}
```

- This example additionally checks the language of the "hail", and will only respond to text in that language.

```perl
sub EVENT_SAY {
     #::: Checks to see if the language is Thieves Cant (language ID 10)
     if ($langid == 10) {
          #::: Checks if the text is like "Hail", the "i" is for case-insensitive.
          if ($text=~/Hail/i) {
               # Respond, using the same language
               quest::say("Hello, $name!",10);
          }
     }
}
```

## EVENT_SCALE_CALC

### Trigger

- When an item is equipped to scale the item--probably should zone.

### Exports

| Name | Type | Usage
| --- | --- | ---
| itemid | int | `quest::say($itemid); # returns int`
| itemname | int | `quest::say($itemname); # returns int`

### Example

- In this example, we scale a charm item:  40342 - Charm of Exotic Speech.  We have a script global / items / 40342.pl
- The item has a charmfile and charmfileID assigned

```perl
sub EVENT_SCALE_CALC {
	#:: Used for charms that scale with number of rare languages learned
	my $langmastered = 0;
 
	#:: Check each rare language: Old Erudian through Elder Dragon
	for (my $i = 11; $i <= 22; $i++) {
		#:: Check if the client has mastered the language
		if ($client->GetLanguageSkill($i) == 100) {
			$langmastered++;
		}
	}
	$itemid->SetScale($langmastered/12);
}
```

## EVENT_SIGNAL

### Trigger

- Triggered using quest::signal(NPC_ID,wait_time) or quest::signalwith(NPC_ID,signal_ID,wait_time).

Generally a way to have one NPC cause another NPC to do something.  Often used with "controller" NPCs that coordinate events.

### Exports

|Name | Type | Usage
| --- | --- | ---
|signal | int | `quest::say($signal); # returns int`

### Example

- This example increments a counter each time a signal with the appropriate ID is received.

```perl
my $count = 0;

sub EVENT_SIGNAL {
     #::: Signal 1 is from the clockwork spiders being killed.
     if ($signal == 1) {
          $count++;
          if ($count == 1) {
               #::: Start a three minute timer to spawn targetable Manaetic Behemoth
               quest::settimer("wake", 180);
          }
     }
     #::: Signal 2 is from the clockwork spiders reaching Manaetic Behemoth.
     if ($signal == 2) {
          #::: Reset the count and make them start over.
          $count = 0;
          quest::stoptimer("wake");
     }
}

sub EVENT_TIMER {
     #::: This uses eq for a string comparison to match the timer "wake".
     #::: Check the count to make sure the clockwork spiders were killed and not just kited. 
     if ($timer eq "wake" && $count >= 12) {
          quest::stoptimer("wake");
          #::: Spawn the targetable version of Manaetic Behemoth in place
          quest::spawn2(206074,0,0,$x,$y,$z,0);
          #::: Depop the untargetable version of Manaetic Behemoth with respawn timer active.
          quest::depop_withtimer();
     }
}
```

## EVENT_SLAY

### Trigger

- whenever an NPC kills a player.  

Often this event is used for some flavor messages, or to spawn adds. Do not confuse this event with EVENT_DEATH_COMPLETE or EVENT_DEATH, which are used when a player kills an NPC.

### Example

- This is a well-known example from Emperor Ssraeshza, who mocks any player that he kills

```perl
sub EVENT_SLAY {
	quest::say("Your god has found you lacking.");
}
```

## EVENT_SPAWN

### Trigger

- When the NPC spawns.

This event is often used to start timers, attack player targets, establish NPC HP events or proximities, start dialogues, and more.

### Example

- In this example, when the mob spawn, we make it run and attack a nearby player while it shouts a war cry.

```perl
sub EVENT_SPAWN {
	#:: Set the NPC to run
	quest::SetRunning(1);
	#:: Shout out a war cray
	quest::shout("For Jotenheimr!!!");
	#:: Try to find a random client within 200 units of the NPC
	my $rClient = $entity_list->GetRandomClient($x,$y,$z, 200);
	#:: If there's a random sucker nearby, attack them
	if ($rClient) {
		quest::attack($rClient->GetName());
	}
}
```

## EVENT_SPAWN_ZONE

### Trigger

- When an NPC spawns.

**Used by the zone controller.**

### Exports

| Name | Type | Usage
| --- | --- | ---
| spawned_entity_id | int | `quest::say($spawned_entity_id); # returns int`
| spawned_npc_id | int | `quest::say($spawned_npc_id); # returns int`

## EVENT_SPELL_EFFECT_CLIENT

### Trigger

- When the spell lands on a client.

### Exports

|Name | Type | Usage
| --- | --- | ---
|caster_id | int | `quest::say($caster_id); # returns int`

## EVENT_SPELL_EFFECT_NPC

### Trigger

- When the spell lands on an NPC.

### Exports

|Name | Type | Usage
| --- | --- | ---
|caster_id | int | `quest::say($caster_id); # returns int`

## EVENT_SPELL_EFFECT_BUFF_TIC_CLIENT

### Trigger

- When the spell ticks on a client.

### Exports

|Name | Type | Usage
| --- | --- | ---
|caster_id | int | `quest::say($caster_id); # returns int`

## EVENT_SPELL_EFFECT_BUFF_TIC_NPC

### Trigger

- When the spell ticks on an NPC.

### Exports

|Name | Type | Usage
| --- | --- | ---
|caster_id | int | `quest::say($caster_id); # returns int`

## EVENT_SPELL_EFFECT_TRANSLOCATE_COMPLETE

### Trigger

- when translocation is complete.

## EVENT_SPELL_FADE

### Trigger

- when a spell fades.

## EVENT_TARGET_CHANGE

### Trigger

- when a mob changes their current target or clears it.

## EVENT_TASKACCEPTED

### Trigger

- when a player accepts a task from the task selector window.

Typically you would handle this functionality using the task system.

## EVENT_TASK_COMPLETE

### Trigger

- when a player completes a task.

Typically you would handle this functionality using the task system.

### Exports

| Name | Type | Usage
| --- | --- | ---
|donecount | int | `quest::say($donecount); # returns int`
|activity_id | int | `quest::say($activity_id); # returns int`
|task_id | int | `quest::say($task_id); # returns int`

## EVENT_TASK_FAIL

### Trigger

- When a player fails a task.

### Exports

| Name | Type | Usage
| --- | --- | ---
|task_id | int | `quest::say($task_id); # returns int`

Typically you would handle this functionality using the task system.

## EVENT_TASK_STAGE_COMPLETE

### Trigger

- When a task stage is completed.

Typically you would handle this functionality using the task system.

### Exports

| Name | Type | Usage
| --- | --- | ---
|activity_id | int | `quest::say($activity_id); # returns int`
|task_id | int | `quest::say($task_id); # returns int`

### Example

- In this example, when a player completes a task, it triggers the event and tries to match with task ID 212; if it matches, a yellow message is displayed to the client.

```perl
sub EVENT_TASK_STAGE_COMPLETE {
	#:: Match task id 212
	if ($task_id == 212) {
		$client->Message(15,"The zombie presence seems somewhat lessened, and perhaps they have been quelled...for the time being.");
	}
}
```

## EVENT_TASK_UPDATE

### Trigger

- when a player's task is updated.

### Exports

| Name | Type | Usage
| --- | --- | ---
|donecount | int | `quest::say($donecount); # returns int`
|activity_id | int | `quest::say($activity_id); # returns int`
|task_id | int | `quest::say($task_id); # returns int`

## EVENT_TIMER

### Trigger

- by a quest::settimer(timer_name,duration_in_seconds) or quest::settimerMS(timer_name,duration_in_milliseconds)

The timer will loop until it is stopped, and EVENT_TIMER will trigger each time that the duration of the timer elapses.  Timers can be stopped using the quest::stopalltimers() or quest::stoptimer(timer_name) functions.

### Exports

|Name | Type | Usage
| --- | --- | ---
|timer | int | `quest::say($timer); # returns int`

### Example

- This is an example of using a timer with a string name to cause an NPC to depop 30 minutes after it spawns

```perl
sub EVENT_SPAWN {
     # Start a timer that is named "depop", the duration is 1,800 seconds (30 minutes)
     quest::settimer("depop",1800); 
}

sub EVENT_TIMER {
     # Use eq for string comparison to match timer "depop"
     if ($timer eq "depop") {
          # Stop timer "depop" from looping
          quest::stoptimer("depop"); 
          quest::depop(); 
     }
}
```

## EVENT_TRADE

### Trigger

- When a client begins a trade.

## EVENT_UNAUGMENT_ITEM

### Trigger

- When a client removes an augment from an item.

## EVENT_UNEQUIP_ITEM

### Trigger

- When a client unequips an item.

## EVENT_USE_SKILL

### Trigger

- When a player uses a skill

### Exports 

|Name | Type | Description
| --- | --- | ---
|skill_id | int | `quest::say($skill_id); # returns int`
|skill_level | int | `quest::say($skill_level); # returns int`

### Example

This example would display a message to the client who uses kick and has a high enough skill level.

```perl
sub EVENT_USE_SKILL {
    #:: Match if skill is Kick (30) and Skill Level is greater than or equal to 100.
    if ($skill_id == 30 && $skill_level >= 100) {
        $client->Message(315, "You have used Kick. Your skill level is $skill_level");
    }
}
```

## EVENT_WAYPOINT_ARRIVE

### Trigger

- When an NPC arrives at a grid waypoint entry.

### Exports 

|Name | Type | Description
| --- | --- | ---
|wp | int | `quest::say($wp); # returns int`

### Example

- This example would cause your NPC to speak as it arrives at a particular waypoint.
- Don't forget to count waypoint 0 (the spawn point) when using waypoint events.

```perl
sub EVENT_WAYPOINT_Arrive {
     # If we have arrived at waypoint 10
     if ($wp == 10) {
          quest::say("We're finally here!");
     }
}
```

## EVENT_WAYPOINT_DEPART

### Trigger

- When an NPC leaves its current grid waypoint entry.

### Exports 

|Name | Type | Description
| --- | --- | ---
|wp | int | `quest::say($wp); # returns int`

### Example

- This example would cause your NPC to speak as it departs a particular waypoint.
- Don't forget to count waypoint 0 (the spawn point) when using waypoint events.

```perl
sub EVENT_WAYPOINT_DEPART {
     # If we departed waypoint 0
     if ($wp == 0) {
          quest::say("And we're off!");
     }
}
```

## EVENT_WEAPON_PROC

### Trigger

- When a weapon procs.

## EVENT_ZONE

### Trigger

- When a player leaves a zone.

### Exports 

|Name | Type | Description
| --- | --- | ---
|target_zone_id | int | `quest::say($target_zone_id); # returns int`

### Example

- In this example, we blow up pets when a player with a pet zones.

```perl
sub EVENT_ZONE {
	#:: Match if a player has a pet
	if ($client->GetPetID()) {
		#:: Get the pet's ID and kill it
		$PetID = $entity_list->GetMobByID($client->GetPetID());
		$PetID->Kill();
	}	
}
```