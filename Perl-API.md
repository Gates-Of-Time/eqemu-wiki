- [**Beginners Guide To Perl**](#beginners-guide-to-perl)
- [**Real Use Examples**](#real-use-examples)
    + [Conditionals](#--conditionals--)
    + [Operators](#--operators--)
    + [Text Response Example](#text-response-example)
    + [Special Text Response Examples](#special-text-response-examples)
    + [Using $npc->GetHateList();](#--using--npc--gethatelist-----)
- [**How Perl Quests Are Loaded**](#how-perl-quests-are-loaded)
    + [NPC](#npc)
    + [Player](#player)
- [**Global Scripts**](#global-scripts)
    + [Player](#player-1)
    + [NPC](#npc-1)
    + [Item](#item)
    + [Spell Scripts](#spell-scripts)
- [**Perl Debugging**](#perl-debugging)

**Sub-Pages in this category:**

- [**sub EVENTs**](https://github.com/EQEmu/Server/wiki/Perl-API---Sub-Events)
- [**Exported Variables**](https://github.com/EQEmu/Server/wiki/Perl-API---Exported-Variables)
- [**Quest API**](https://github.com/EQEmu/Server/wiki/Perl-API---Quest-API)
- [**Function Lists**](https://github.com/EQEmu/Server/wiki/Perl-API---Functions)
    + [Client](https://github.com/EQEmu/Server/wiki/Perl-API---Functions#client)
    + [Corpse](https://github.com/EQEmu/Server/wiki/Perl-API---Functions#corpse)
    + [EntityList](https://github.com/EQEmu/Server/wiki/Perl-API---Functions#entitylist)
    + [Group](https://github.com/EQEmu/Server/wiki/Perl-API---Functions#group)
    + [Raid](https://github.com/EQEmu/Server/wiki/Perl-API---Functions#raid)
    + [Mob](https://github.com/EQEmu/Server/wiki/Perl-API---Functions#mob)
    + [NPC](https://github.com/EQEmu/Server/wiki/Perl-API---Functions#npc)
    + [Quest Items](https://github.com/EQEmu/Server/wiki/Perl-API---Functions#quest-items)
    + [Object](https://github.com/EQEmu/Server/wiki/Perl-API---Functions#object)
    + [Door](https://github.com/EQEmu/Server/wiki/Perl-API---Functions#door)


***


# Beginners Guide To Perl

* Are you new to Perl? Perl isn't just a EQEmu scripting language, it's been around for eons and used in many systems
* Here is a reference to basic Perl [Beginners Guide to Perl](http://www.tizag.com/beginnerT/)

# Real Use Examples

## **Conditionals**

**Syntax**

```perl
if ($variable1 [operator] $variable2) {
    quest::commands;
}
```

**Example:**

```perl
if ($variable1 [operator] $variable2) {
    quest::commands;
}
elsif ($variable1 [someotheroperator] $variable2) {
    quest::commands;
}
else {
    quest::commands;
}
```

## Operators

Note, special operators apply to string comparisons in Perl!

```perl
$1 == $2 # If variable $1 is the same as variable $2, carry on.
$1 != $2 # If variable $1 is NOT the same as variable $2, carry on.
$1 > $2 # If variable $1 is greater than variable $2, carry on.
$1 < $2 # If variable $1 is less than variable $2, carry on.
$1 >= $2 # If variable $1 is greater than or equal to variable $2, carry on.
$1 <= $2 # If variable $1 is less than or equal to variable $2, carry on.
$1 eq $2 # If string variable $1 is the same as string variable $2, carry on.
$1 ne $2 # If string variable $1 is NOT the same as string variable $2, carry on.
$1 =~ $2 # If string variable $1 contains/matches the string variable $2, carry on.
```

In this example, if the user is a smaller level than the mob the mob says "I'm a higher level than you!"

```perl
if ($ulevel < $mlevel) {
	quest::say("I'm a higher level than you!");
}
if ($name ne "Joe") {
	quest::say("I will only talk to joe!");
}
```

## Text Response Example

All speaking responses are included in a **$text** variable

```perl
if ($text=~/hail/i) # Note the /i. This means it is case-insensitive. It is always better to include this.
if ($text=~/Hello/) # Would match "Hello", but not "hello".
if ($text=~/hello/) # Would match "hello", but not "Hello".
if ($text=~/hello/i) # Would match "Hello" and "hello".
if ($text=~/me/) # Would match the "me" in "name", but not the "me" in "NAME".
if ($text=~/\bme\b/) # Would not match the "me" in "name" or the "me" in "NAME". The "\b" means there must not be text next to the match so "me" must be by itself.
if ($text=~/^me$/i) # Would only match if "me" is the only text said. The "^" tells what must be the first thing said and the "$" tells what must be the last thing.
```

## Special Text Response Examples

These responses allow you to check for multiple strings within your text variable.

```perl
if ($text=~/Hail|Hi|Hello/i) # Will check if the text contains "Hail", "Hi", or "Hello".
if ($text!~/Hail|Hi|Hello/i) # Will check if the text does not contain "Hail", "Hi", or "Hello".
```

## **Using $npc->GetHateList();**

```perl
sub EVENT_AGGRO_SAY {
    if($text=~/hate/i) {
        my @hatelist = $npc->GetHateList();
        foreach $ent (@hatelist) {
            my $h_ent = $ent->GetEnt();  # do not forget GetEnt() or the script halts!
            my $h_dmg = $ent->GetDamage();
            my $h_hate = $ent->GetHate();
            if($h_ent) {
                my $h_ent_name = $h_ent->GetCleanName();
                quest::say("$h_ent_name is on my hate list with $h_hate hate and $h_dmg damage.");
            }
        }
    }
}
```

# How Perl Quests Are Loaded

### NPC

In order of operations, an npc's script will be dictated by the first script that it finds below

* quests/zoneshortname/id.pl
* quests/zoneshortname/npc_name.pl
* quests/global/npcid.pl
* quests/global/npc_name.pl
* quests/zoneshortname/default.pl
* quests/global/default.pl

### Player

In order of operations, a player's script will be dictated by the first script that it finds below

* quests/zoneshortname/player_v[instance_version].pl
* quests/zoneshortname/player.pl
* quests/global/player.pl

# Global Scripts

* Global scripts were designed to run on top of the scripts mentioned above, meaning if you have a player script in a zone directory and a global player script, they will both execute and not interfere with each other

### Player

* quests/global/global_player.pl

### NPC

* quests/global/global_npc.pl

### Item

Item Scripts are quest scripts attached to Items.
Items will load a script on the first event that triggers them and will load one and only one from the following location. Which ever it finds first in the following order

* ./quests/zone/items/item_script.pl
* ./quests/global/items/item_script.pl
* ./quests/zone/items/default.pl
* ./quests/global/items/default.pl

### Spell Scripts

Spell Scripts are quest scripts attached to Spells.
Spells will load a script on the first event that triggers them and will load one and only one from the following location. Which ever it finds first in the following order:

* ./quests/zone/spells/spell_id.pl
* ./quests/global/spells/spell_id.pl
* ./quests/zone/spells/default.pl
* ./quests/global/spells/default.pl

# Perl Debugging

* Run the perl file against the perl processor for syntax errors. (e.g. perl <filename.pl>)
* Reload the quest in game. #reloadquest or #rq
* See any recent API errors. #questerrors
* Peek at the zone console and see if any hints appear there. Also look at the zone logfile.