**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
spawngroupID|int(11)|NO|PRI|0| 
npcID|int(11)|NO|PRI|0| 
chance|smallint(4)|NO| |0| 
condition_value_filter|mediumint(9)|NO| |1|1:Always possible, 2-n:Will only spawn if condition_value in spawn2 matches

The spawnentry table has an entry for every NPC that is possible for a spawngroup.  Every [spawn2](https://github.com/EQEmu/Server/wiki/spawn2) entry is associated with exactly one [spawngroup](https://github.com/EQEmu/Server/wiki/spawngroup).  If an entry in the [spawn2](https://github.com/EQEmu/Server/wiki/spawn2) table is enabled, and the condition value for that entry's condition is at least 1, an NPC is picked based on chance from this (spawnentry) table.

The condition_value_filter allows further filtering of which NPC gets picked.

It is easy to get the roles of the _condition, cond_value (both from spawn2) and condition_value_filter confused.  To summarize:

**Field**|**Table**|**Notes**
-----|-----|-----
_condition|spawn2|A spawn2 entry will not fire unless _condition is zero (always on) or a specified non-zero _condition is enabled (see spawn_condition_values).
cond_value|spawn2|Only used if (_condition > 0). Nearly 100% of the usage of this field is on(1)/off(0).
condition_value_filter|spawnentry|The cond_value of the _condition in the relevant spawn2 entry must match exactly to enable this npc.

**(Note about why condition_value_filter was added)**

Most eqemu servers utilize (2) spawn2 entries to enable day/night.  One entry for Night (condition 1) and another for Day (condition 2).  Using this technique does not allow for day/night spawns to co-exist.  On live, some zones such as lake rathe, allow day mobs to spawn in spots where night mobs were killed, while leaving the rest of the night mobs up.

The addition of the condition_value_filter in spawnentry allows day/night to be implemented using a single condition and single spawn2 locations for each mob.  These spawn2 entries are always enabled (cond_value 1).  The single condition simply toggles between day/night.  This is done by using a [spawncondition](https://github.com/EQEmu/Server/wiki/spawn_conditions) with an onchange value of 0 (do nothing).  The spawnentry rows are then filtered based on the current value of the _condition.  See [spawn_events](https://github.com/EQEmu/Server/wiki/spawn_events) table for details on how day/night are enabled/disabled.