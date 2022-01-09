**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
npc\_faction\_id|int(11) unsigned|NO|PRI|0| 
faction\_id|int(11) unsigned|NO|PRI|0| 
value|int(11)|NO| |0| 
npc\_value|tinyint(3)|NO| |0| 
temp|tinyint(3)|NO| |0| 

### NPC Faction Entries Explained

|Field Name | Description |
|-----------|-------------|
|npc_faction_id |Value assigned to npc in npc_types.  Indexed into this table (n) times for each faction we want to impact.
|faction_id | Faction id for the faction_list table.  These map to in game factions.
|value| 	Amount gained or lost for killing the NPCs assigned to this npc_faction_id.
|npc_value| How the npcs assigned to this npc_faction_id respond to other npcs that are on the faction_id for this entry.  1:assist, 0:neutral, -1:attack
|temp |	0 (Default): Faction is permanent, player recieves a message.|
||1: Faction is temporary, player does not recieve a message.|
||2: Faction is temporary, player recieves a message.|
||3: Faction is permanent, but player does not recieve a message.|