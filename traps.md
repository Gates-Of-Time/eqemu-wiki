**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
id|int(11)|NO|PRI| |auto\_increment
zone|varchar(16)|NO|MUL| | Zone short name
version|smallint(5) unsigned|NO| |0| Version of the specified Zone
x|int(11)|NO| |0| 
y|int(11)|NO| |0| 
z|int(11)|NO| |0| 
chance|tinyint(4)|NO| |0| 0-100 percent
maxzdiff|float|NO| |0| 
radius|float|NO| |0| 
effect|int(11)|NO| |0| The type of trap (see Parameters below).
effectvalue|int(11)|NO| |0| A variable used for the trap (see Parameters below).
effectvalue2|int(11)|NO| |0| A variable used for the trap (see Parameters below).
message|varchar(200)|NO| | | Standard message unless optional message set (see Message defaults below).
skill|int(11)|NO| |0| Skill required to disarm the trap.
level|mediumint(4) unsigned|NO| |1| The level of the trap--important for spell cast traps, unused on other types.
respawn\_time|int(11) unsigned|NO| |60| Respawn time seconds.
respawn\_var|int(11) unsigned|NO| |0| Variance to respawn time in seconds.
triggered\_number|tinyint(4)|NO| |0| 
group|tinyint(4)|NO| |0| 
despawn\_when\_triggered|tinyint(4)|NO| |0| 
undetectable|tinyint(4)|NO| |0| 

## Trap Parameters

**Type**|**Effect**|**Effect Value**|**Effect Value 2**|**Notes**
-----|-----|-----|-----|-----|
Casting Trap | 0 |  Spell ID | Unused | Casts a spell on the player that triggered the trap. 
Alarm Trap | 1 | Range of effect | 0 (all NPCs aggro) or 1 (only KOS NPCs aggro) | Causes NPCs to aggro the player who triggered the trap. 
Mystic Spawn (NPC Trap) | 2 | npc_type ID of the mob spawned | number of mobs spawned | Spawns NPCs at a close spot in a small area 
Bandit Spawn (NPC Trap2) | 3 | npc_type ID of the mob spawned | number of mobs spawned | Spawns NPCs at a close spot in a large area 
Damage Trap | 4 | minimum amount of damage | maximum amount of damage | Causes damage to the player that triggered the trap. 

## Trap Message Defaults

**Type**|**Effect**|**Default Message**
-----|-----|-----
Casting Trap | 0 | "_____ triggers a trap!"
Alarm Trap | 1 | "A loud alarm rings out through the air..."
Mystic Spawn | 2 | "The air shimmers..."
Bandit Spawn | 3 | "A bandit leaps out from behind a tree!"
Damage Trap | 4 | "_____ triggers a trap!"