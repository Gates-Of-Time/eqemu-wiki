#ProTip: hit ctrl + f (Windows) or ⌘ + f (Mac) to FIND something on this page

* A full list can always be found in the EQEmu source [https://github.com/EQEmu/Server/blob/master/zone/embparser.cpp](https://github.com/EQEmu/Server/blob/master/zone/embparser.cpp)
* Exported variables are sometimes available globally during sub-events, some exported variables are only available in certain sub-events--see [[Perl API sub EVENTs|Perl-API---Sub-Events]] for a listing of each event and its exports.

| Exported Variable | Usage |
| --- | --- |
| $activity_id | Returns the ID of the task stage completed (in EVENT_TASK_STAGE_COMPLETE); Returns the ID of the task updated or complete (in EVENT_TASK_COMPLETE, EVENT_TASK_UPDATE)
| $charid | Returns the character ID of the client that triggered the Event or a negative value if no client was involved.
| $class | Returns the class of the user that triggered the event.
| $caster_id | Returns the ID of the caster (in EVENT_SPELL_EFFECT_CLIENT, EVENT_SPELL_EFFECT_NPC, EVENT_SPELL_BUFF_TIC_CLIENT, EVENT_SPELL_BUFF_TIC_NPC)
| $combat_state | Returns 1 for starting combat, returns 0 for leaving combat (in EVENT_COMBAT)
| $corpse | Returns the ID of the corpse in which an item was looted (in EVENT_LOOT)
| $donecount | Return the number of hand-ins completed [i.e. 5 of 10 Crushbone Belts, the 5 would be returned] (in EVENT_TASK_COMPLETE, EVENT_TASK_UPDATE)
| $doorid | Returns ID of the door clicked (in EVENT_CLICK_DOOR)
| $faction | Returns the faction level number of the user with the NPC
| $fished_items | Returns the item ID of fished item (in EVENT_FISH_SUCCESS)
| $foraged_item | Returns the item ID of foraged item (in EVENT_FORAGE_SUCCESS)
| $grouped | Returns 0 or 1 depending on group status (in EVENT_GROUP_CHANGED)
| $hate_state | Return the state of hate (in EVENT_HATE_LIST)
| $hpevent | Returns the value set by quest::setnexthpevent();
| $item1 | The item ID in the first slot.
| $item2 | The item ID in the second slot.
| $item3 | The item ID in the third slot.
| $item4 | The item ID in the fourth slot.
| $item1_charges | The number of charges in the first slot.
| $item2_charges | The number of charges in the second slot.
| $item3_charges | The number of charges in the third slot.
| $item4_charges | The number of charges in the fourth slot.
| $item1_attuned | The attuned setting in the first slot (1 if attuned, 0 if not attuned).
| $item2_attuned | The attuned setting in the second slot (1 if attuned, 0 if not attuned).
| $item3_attuned | The attuned setting in the third slot (1 if attuned, 0 if not attuned).
| $item4_attuned | The attuned setting in the fourth slot (1 if attuned, 0 if not attuned).
| $itemcount{itemid} | | $itemcount{1001} would return 2 if the user turned in 2 1001 items.
| $itemid | Return the item ID of items used (in EVENT_ITEM_CLICK_CAST, EVENT_ITEM_CLICK)
| $itemname | Returns the item name of items used (in EVENT_ITEM_CLICK_CAST, EVENT_ITEM_CLICK)
| $killed | Returns the NPC id of the npc slain (in EVENT_NPC_SLAY)
| $killer_damage | Returns the damage of the mob's killer's killing blow (in EVENT_DEATH, EVENT_DEATH_COMPLETE)
| $killer_id | Returns the entity ID of a mob's killer (in EVENT_DEATH, EVENT_DEATH_COMPLETE)
| $killer_skill | Returns the skill ID of the mob's killer's killing blow (in EVENT_DEATH, EVENT_DEATH_COMPLETE)
| $killer_spell | Returns the spell ID of the mob's killer's spell (in EVENT_DEATH, EVENT_DEATH_COMPLETE)
| $hasitem{itemid} | Checks the character's inventory master slots for an item
| $hpevent | Used to identify the HP Event set via quest::setnexthpevent() (in EVENT_HP)
| $hpratio | Returns HP Ratio
| $inchpevent | Used potentially for the incoming hp event or next hp event (in EVENT_HP)
| $instanceid | Returns the instance ID of the current zone
| $instanceversion | Returns the instance version
| $langid | Returns the language id the player/npc is currently using. (in EVENT_SAY, EVENT_AGGRO_SAY, EVENT_PROXIMITY_SAY)
| $looted_charges | Returns the charges of the looted item (in EVENT_LOOT)
| $looted_id | Returns the ID of the looted item (in EVENT_LOOT)
| $oncursor{itemid} | Checks the character's front item on the cursor for an item
| $objectid | Returns the object id of the clicked item (in EVENT_CLICK_OBJECT)
| $mlevel | Returns the level of the mob that the user triggered the Event on.
| $mname | Returns the mob's name (returns non-clean, for a clean name use | $npc->GetCleanName();).
| $mobid | Returns the npc_types ID of the mob that the user triggered the Event on.
| $name | Returns the name of the user that triggered the Event.
| $picked_up_id | Returns the item id picked up (in EVENT_PLAYER_PICKUP)
| $popupid | Returns the ID of the popup window (in EVENT_POPUPRESPONSE)
| $race | Returns the race of the user that triggered the Event.
| $raided | Returns 0 or 1 depending on group status (in EVENT_GROUP_CHANGED)
| $recipe | Returns the ID of the recipe (in EVENT_COMBINE_SUCCESS, EVENT_COMBINE_FAILURE)
| $signal | Returns the value of a signal sent using quest::signalwith() (in EVENT_SIGNAL)
| $slotid | Returns the slot ID of the item used (in EVENT_ITEM_CLICK_CAST, EVENT_ITEM_CLICK)
| $spell_id | Returns the ID of the spell cast (in EVENT_CAST, EVENT_CAST_ON, EVENT_CAST_BEGIN)
| $status | Returns the account status of the user that triggered the Event.
| $target_zone_id | Returns the ID of the zone to enter, such as in casting ports (in EVENT_ZONE)
| $targetid | Returns the entity id of the NPC's current (or last) target.
| $targetname | Returns the name of the NPC's current (or last) target.
| $task_id | Returns the task ID of the task accepted (in EVENT_TASKACCEPTED), stage completed (in EVENT_TASK_STAGE_COMPLETE), task failed (in EVENT_TASK_FAIL), task updated or completed (in EVENT_TASK_COMPLETE, EVENT_TASK_UPDATE)
| $text | The text sent by players to an NPC (in EVENT_SAY), from an NPC (in EVENT_AGGRO_SAY), spoken by player when nearby the NPC (in EVENT_PROXIMITY_SAY)
| $timer | Returns the value used when creating a timer with quest::settimer() (in EVENT_TIMER)
| $uguild_id | Returns the ID of the guild of the user that triggered the Event.
| $uguildrank | Returns the guild rank of the user that triggered the Event.
| $ulevel | Returns the level of the user that triggered the Event.
| $userid | Returns the ID of the user that triggered the Event.
| $version | Returns the version of the door clicked (in EVENT_CLICKDOOR)
| $wp | Returns current waypoint (in EVENT_WAYPOINT_ARRIVE and EVENT_WAYPOINT_DEPART)
| $zonehour | Returns the current in-game hour.
| $zoneid | Returns the zone id that the Event occured in.
| $zoneln | Returns the zone long name that the Event occured in.
| $zonemin | Returns the current in-game minute.
| $zonesn | Returns the zone short name that the Event occured in.
| $zonetime | Returns the current in-game time in HHMM format.
| $zoneweather | Returns current weather of zone. 0 for none, 1 for rain, 2 for snow.
| $copper | Returns the number of copper coins given to the mob.
| $silver | Returns the number of silver coins given to the mob.
| $gold | Returns the number of gold coins given to the mob.
| $platinum | Returns the number of platinum coins given to the mob.
| $x | The X coordinate of the NPC.
| $y | The Y coordinate of the NPC.
| $z | The Z coordinate of the NPC.
| $h | The heading of the NPC.