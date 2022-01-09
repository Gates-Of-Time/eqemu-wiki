**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
id|int(11)|NO|PRI|0|Unique item identifier number 
minstatus|smallint(5)|NO|MUL|0|minimum account status required to use the item
Name|varchar(64)|NO|MUL| |Name of the item
aagi|int(11)|NO| |0| Agility bonus. Valid values: -127 - 127
ac|int(11)|NO| |0| AC bonus.  Valid values: -2147483647 - 2147483647
accuracy|int(11)|NO| |0| Amount of accuracy on the item.
acha|int(11)|NO| |0| Charisma bonus. Valid values: -127 - 127
adex|int(11)|NO| |0| Dexterity bonus. Valid values: -127 - 127
aint|int(11)|NO| |0| Intelligence bonus. Valid values: -127 - 127
artifactflag|tinyint(3) unsigned|NO| |0| Determines whether or not an item gets the artifact flag. 0 - No, 1 - Yes
asta|int(11)|NO| |0| Stamina bonus. Valid values: -127 - 127
astr|int(11)|NO| |0| Strength bonus. Valid values: -127 - 127
attack|int(11)|NO| |0| Attack bonus.
augrestrict|int(11)|NO| |0| [Augment Restrict Reference](https://github.com/EQEmu/Server/wiki/Augment-Restrictions)
augslot1type|tinyint(3)|NO| |0| The Type of Augment that the slot can hold. [Augment Type Reference](https://github.com/EQEmu/Server/wiki/Augment-Types)
augslot1visible|tinyint(3)|YES| | | Whether or not the augment slot is visible. 0 - No, 1 - Yes
augslot2type|tinyint(3)|NO| |0| The Type of Augment that the slot can hold. [Augment Type Reference](https://github.com/EQEmu/Server/wiki/Augment-Types)
augslot2visible|tinyint(3)|YES| | | Whether or not the augment slot is visible. 0 - No, 1 - Yes
augslot3type|tinyint(3)|NO| |0| The Type of Augment that the slot can hold. [Augment Type Reference](https://github.com/EQEmu/Server/wiki/Augment-Types)
augslot3visible|tinyint(3)|YES| | | Whether or not the augment slot is visible. 0 - No, 1 - Yes
augslot4type|tinyint(3)|NO| |0| The Type of Augment that the slot can hold. [Augment Type Reference](https://github.com/EQEmu/Server/wiki/Augment-Types)
augslot4visible|tinyint(3)|YES| | | Whether or not the augment slot is visible. 0 - No, 1 - Yes
augslot5type|tinyint(3)|NO| |0| The Type of Augment that the slot can hold. [Augment Type Reference](https://github.com/EQEmu/Server/wiki/Augment-Types)
augslot5visible|tinyint(3)|YES| | | Whether or not the augment slot is visible. 0 - No, 1 - Yes
augslot6type|tinyint(3)|NO| |0| The Type of Augment that the slot can hold. [Augment Type Reference](https://github.com/EQEmu/Server/wiki/Augment-Types)
augslot6visible|tinyint(3)|NO| |0| Whether or not the augment slot is visible. 0 - No, 1 - Yes
augtype|int(11)|NO| |0| [Augment Type Reference](https://github.com/EQEmu/Server/wiki/Augment-Types)
avoidance|int(11)|NO| |0| Amount of avoidance on the item.
awis|int(11)|NO| |0| Wisdom bonus. Value values: -127 - 127
bagsize|int(11)|NO| |0| [Bag Sizes](https://github.com/EQEmu/Server/wiki/Bag-Sizes)
bagslots|int(11)|NO| |0| The number of bag slots a bag has. Keep it at a maximum of 10.
bagtype|int(11)|NO| |0| [Bag Types](https://github.com/EQEmu/Server/wiki/Bag-Types)
bagwr|int(11)|NO| |0| The amount of weight reduction on the bag.
banedmgamt|int(11)|NO| |0| The amount of bane damage.
banedmgraceamt|int(11)|NO| |0| The amount of race bane damage.
banedmgbody|int(11)|NO| |0| The [Body Type](https://github.com/EQEmu/Server/wiki/Body-Types) the bane damages.
banedmgrace|int(11)|NO| |0| The [Race Type](https://github.com/EQEmu/Server/wiki/Race-Types) of the bane damage. 
bardtype|int(11)|NO| |0| The [Bard Type](https://github.com/EQEmu/Server/wiki/Bard-Types) of instrument.
bardvalue|int(11)|NO| |0| How much the instrument type is modified when equipped.
book|int(11)|NO| |0| The type of book displayed (scroll graphic, book, etc)
casttime|int(11)|NO| |0| The cast time of the spell in milliseconds.
casttime\_|int(11)|NO| |0| The cast time of the click effect.
charmfile|varchar(32)|NO| | | The file used by the charm to scale.
charmfileid|varchar(32)|NO| | | The ID of the file used by the charm to scale.
classes|int(11)|NO| |0| The [Classes](https://github.com/EQEmu/Server/wiki/Class-List) that can use the item.
color|int(10) unsigned|NO| |0| The color of the item.
combateffects|varchar(10)|NO| | | Amount of combat effects on the item.
extradmgskill|int(11)|NO| |0| The [Skill](https://github.com/EQEmu/Server/wiki/Skills) that receives extra damage.
extradmgamt|int(11)|NO| |0| The amount of extra damage you get in the skill.
price|int(11)|NO| |0| The price the item costs from a vendor.
cr|int(11)|NO| |0| Cold Resistance. Valid values: -127 - 127
damage|int(11)|NO| |0| Amount of damage on the item.
damageshield|int(11)|NO| |0| Amount of damage shield on the item.
deity|int(11)|NO| |0| The [Deity](https://github.com/EQEmu/Server/wiki/Diety-List) you must follow to use this item.
delay|int(11)|NO| |0| The delay of the item, determines how fast it hits. 0 Is for non-weapons.
augdistiller|int(11)|NO| |0| If this item is an augment, this is the id of the distiller that will remove it from an item safely.
dotshielding|int(11)|NO| |0| Amount of damage over time shielding on the item.
dr|int(11)|NO| |0| Disease Resistance. Valid values: -127 - 127
clicktype|int(11)|NO| |0| The [Click Type](https://github.com/EQEmu/Server/wiki/Item-Click-Types) of the item
clicklevel2|int(11)|NO| |0| Level required to use the click effect.
elemdmgtype|int(11)|NO| |0| The [Element Type](https://github.com/EQEmu/Server/wiki/Item-Element-Types) for additional damage on the weapon.
elemdmgamt|int(11)|NO| |0| The amount of element damage on the weapon.
endur|int(11)|NO| |0| Endurance bonus.
factionamt1|int(11)|NO| |0| The amount of faction adjusted while the item is equipped.
factionamt2|int(11)|NO| |0| The amount of faction adjusted while the item is equipped.
factionamt3|int(11)|NO| |0| The amount of faction adjusted while the item is equipped.
factionamt4|int(11)|NO| |0| The amount of faction adjusted while the item is equipped.
factionmod1|int(11)|NO| |0| The faction modified by factionamt1 while the item is equipped.
factionmod2|int(11)|NO| |0| The faction modified by factionamt2 while the item is equipped.
factionmod3|int(11)|NO| |0| The faction modified by factionamt3 while the item is equipped.
factionmod4|int(11)|NO| |0| The faction modified by factionamt4 while the item is equipped.
filename|varchar(32)|NO| | | If an item is a book, this determines what the actual book is. It corresponds to the name field in the books table.
focuseffect|int(11)|NO| |0| The spell ID of the focus effect you want the item to have.
fr|int(11)|NO| |0| Fire Resistance. Valid values: -127 - 127
fvnodrop|int(11)|NO| |0| Requires the Rule World:FVNoDropFlag to be set to 1, disables /ooc and uses FVNoDrop for No Trade rather than No Drop. 0 = Tradeable, 1 = No Trade
haste|int(11)|NO| |0| Haste percentage the item has.
clicklevel|int(11)|NO| |0| This is the level at which the item can cast its fully powered spell.
hp|int(11)|NO| |0| Hit point bonus
regen|int(11)|NO| |0| Health regeneration per tick.
icon|int(11)|NO| |0| The item's icon.
idfile|varchar(30)|NO| | | The model of the item. Example: IT63 is non-weapon items like armour.
itemclass|int(11)|NO| |0| The [Item Class](https://github.com/EQEmu/Server/wiki/Item-Class) of the item.
itemtype|int(11)|NO| |0| The [Item Type](https://github.com/EQEmu/Server/wiki/Item-Types) of the item.
ldonprice|int(11)|NO| |0| Amount of LDoN points you want the item to cost (price must be equal to this).
ldontheme|int(11)|NO| |0| The [LDON Theme](https://github.com/EQEmu/Server/wiki/LDON-Themes) used for the LDON price.
ldonsold|int(11)|NO| |0| Whether or not the item is sold by LDoN merchants. 0 = No, 1 = Yes
light|int(11)|NO| |0| Amount of Light generated by an item.
lore|varchar(80)|NO|MUL| | What is displayed when you identify an item. 
loregroup|int(11)|NO| |0| The [Lore Group](https://github.com/EQEmu/Server/wiki/Item-Lore-Groups) of an item.
magic|int(11)|NO| |0| Whether or not an item is magic. 0 = Not Magic, 1 = Magic
mana|int(11)|NO| |0| Mana points bonus.
manaregen|int(11)|NO| |0| Mana regeneration per tick.
enduranceregen|int(11)|NO| |0| Endurance regeneration per tick.
material|int(11)|NO| |0| The material of the item, used for armor.
herosforgemodel|int(11)|NO| |0| The heros forge model used by the item.
maxcharges|int(11)|NO| |0| Maximum spell charges on the item, -1 for infinite.
mr|int(11)|NO| |0| Magic Resistance. Valid values: -127 - 127
nodrop|int(11)|NO| |0| Whether or not an item is tradeable. 0 = No Trade, 1 = Tradeable
norent|int(11)|NO| |0| Whether or not an item is temporary. 0 = Temporary, 1 = Permanent, 255 = Permanent.
pendingloreflag|tinyint(3) unsigned|NO| |0| A leftover remnant.
pr|int(11)|NO| |0| Poison Resistance. Valid values: -127 - 127
procrate|int(11)|NO| |0| The rate at which a weapon procs. Normal is 0, 150% is 50, 50% is -50.
races|int(11)|NO| |0| The [Race Type](https://github.com/EQEmu/Server/wiki/Race-Types) that can use this item.
range|int(11)|NO| |0| Range of the item's attack. Used for Bows and/or Projectile weapons.
reclevel|int(11)|NO| |0| Recommended level for the item. Stats scale down for players below this level.
recskill|int(11)|NO| |0| Recommended skill for the item. Stats scale down for players below skill.
reqlevel|int(11)|NO| |0| Required level for the item.
sellrate|float|NO| |0| Modifies the way an item sells back to an NPC.
shielding|int(11)|NO| |0| Amount of Shielding on an item. 1 = 1%, 5 = 5%.
size|int(11)|NO| |0| The [Size](https://github.com/EQEmu/Server/wiki/Item-Sizes) of the item.
skillmodtype|int(11)|NO| |0| The [Skill](https://github.com/EQEmu/Server/wiki/Skills) you're getting a modified value in.
skillmodvalue|int(11)|NO| |0| The amount of the skill mod on the item.
slots|int(11)|NO| |0| The [Slot](https://github.com/EQEmu/Server/wiki/Inventory-Slots) the item will fit into. 
clickeffect|int(11)|NO| |0| The spell ID of the click effect you want the item to have.
spellshield|int(11)|NO| |0| The spell shielding on an item.
strikethrough|int(11)|NO| |0| The strikethrough on an item.
stunresist|int(11)|NO| |0| The stunresist on an item.
summonedflag|tinyint(3) unsigned|NO| |0| Unknown.
tradeskills|int(11)|NO| |0| Whether or not the item displays a "Used in tradeskills" message. 0 = No, 1 = Yes
favor|int(11)|NO| |0| Amount of Person Favor this item shops and give when turned in to favor NPC.
weight|int(11)|NO| |0| Weight of the item, multiplied by 10. 2 = .2, 50 = 5.
UNK012|int(11)|NO| |0| Unknown.
UNK013|int(11)|NO| |0| Unknown.
benefitflag|int(11)|NO| |0| Unknown.
UNK054|int(11)|NO| |0| Unknown.
UNK059|int(11)|NO| |0| Unknown.
booktype|int(11)|NO| |0| The language a book is written in.
recastdelay|int(11)|NO| |0| Cooldown time on a clickable effect. Stored as seconds.
recasttype|int(11)|NO| |0| Determines which recast timer the item uses. Item A has a 5 minute Recast Delay w/ Recast Type 8. Item B also has Recast Type 8, so you won't be able to cast either until the 5 minutes are up.
guildfavor|int(11)|NO| |0| Amount of Guild Favor this item shops and give when turned in to guild favor NPC.
UNK123|int(11)|NO| |0| Unknown.
UNK124|int(11)|NO| |0| Unknown.
attuneable|int(11)|NO| |0| Whether or not an item is attuneable. 0 = Not Attuneable, 1 = Attuneable
nopet|int(11)|NO| |0| Whether or not pets may use this item. 0 = Usable By Pets, 1 = Not Usable By Pets
updated|datetime|NO| |0000-00-00 00:00:00| Date/Time the item was last updated in the database.
comment|varchar(255)|NO| | | A comment in this field that is viewable only in the database.
UNK127|int(11)|NO| |0| Unknown.
pointtype|int(11)|NO| |0| Unknown.
potionbelt|int(11)|NO| |0| Whether or not this item is able to go into the potion belt. 0 = No, 1 = Yes
potionbeltslots|int(11)|NO| |0| How many potion belt slots the item gives you.
stacksize|int(11)|NO| |0| Amount of this item that players can fit into a stack. This field is irrelevant unless stackable is turned on.
notransfer|int(11)|NO| |0| Unknown.
stackable|int(11)|NO| |0| Whether or not an item is stackable. 0 = Not Stackable, 1 = Stackable
UNK134|varchar(255)|NO| | | Unknown.
UNK137|int(11)|NO| |0| Unknown.
proceffect|int(11)|NO| |0| Spell ID of the proc spell you want the item to have.
proctype|int(11)|NO| |0| Keep this at 0.
proclevel2|int(11)|NO| |0| Level that the proc will reach maximum power.
proclevel|int(11)|NO| |0| Level required for the item to proc.
UNK142|int(11)|NO| |0| Unknown.
worneffect|int(11)|NO| |0| Spell ID of the worn effect you want the item to have.
worntype|int(11)|NO| |0| Use 2 if this is a worn item.
wornlevel2|int(11)|NO| |0| Level that the worn effect will reach maximum power.
wornlevel|int(11)|NO| |0| Level required for the worn effect on the item to take effect.
UNK147|int(11)|NO| |0| Unknown.
focustype|int(11)|NO| |0| Use 6 if the item has a focus effect.
focuslevel2|int(11)|NO| |0| Level that the focus effect will reach maximum power.
focuslevel|int(11)|NO| |0| Level required for the focus effect on the item to take effect.
UNK152|int(11)|NO| |0| Unknown.
scrolleffect|int(11)|NO| |0| The spell ID that the scroll scribes.
scrolltype|int(11)|NO| |0| Use 7 if the item is a scroll.
scrolllevel2|int(11)|NO| |0| Leave this at 0.
scrolllevel|int(11)|NO| |0| Leave this at 0.
UNK157|int(11)|NO| |0| Unknown.
serialized|datetime|YES| | | Unknown.
verified|datetime|YES| | | Unknown.
serialization|text|YES| | | Unknown.
source|varchar(20)|NO| | | Who contributed the item to the database.
UNK033|int(11)|NO| |0| Unknown.
lorefile|varchar(32)|NO| | | Unknown.
UNK014|int(11)|NO| |0| Unknown.
svcorruption|int(11)|NO| |0| Corruption Resistance. Valid values: -127 - 127
skillmodmax|int(11)|NO| |0| 
UNK060|int(11)|NO| |0| Unknown.
augslot1unk2|int(11)|NO| |0| Unknown.
augslot2unk2|int(11)|NO| |0| Unknown.
augslot3unk2|int(11)|NO| |0| Unknown.
augslot4unk2|int(11)|NO| |0| Unknown.
augslot5unk2|int(11)|NO| |0| Unknown.
augslot6unk2|int(11)|NO| |0| Unknown.
UNK120|int(11)|NO| |0| Unknown.
UNK121|int(11)|NO| |0| Unknown.
questitemflag|int(11)|NO| |0| If item is used for quests, can be enabled.
UNK132|text|YES| | | Unknown.
clickunk5|int(11)|NO| |0| Unknown.
clickunk6|varchar(32)|NO| | | Unknown.
clickunk7|int(11)|NO| |0| Unknown.
procunk1|int(11)|NO| |0| Unknown.
procunk2|int(11)|NO| |0| Unknown.
procunk3|int(11)|NO| |0| Unknown.
procunk4|int(11)|NO| |0| Unknown.
procunk6|varchar(32)|NO| | | Unknown.
procunk7|int(11)|NO| |0| Unknown.
wornunk1|int(11)|NO| |0| Unknown.
wornunk2|int(11)|NO| |0| Unknown.
wornunk3|int(11)|NO| |0| Unknown.
wornunk4|int(11)|NO| |0| Unknown.
wornunk5|int(11)|NO| |0| Unknown.
wornunk6|varchar(32)|NO| | | Unknown.
wornunk7|int(11)|NO| |0| Unknown.
focusunk1|int(11)|NO| |0| Unknown.
focusunk2|int(11)|NO| |0| Unknown.
focusunk3|int(11)|NO| |0| Unknown.
focusunk4|int(11)|NO| |0| Unknown.
focusunk5|int(11)|NO| |0| Unknown.
focusunk6|varchar(32)|NO| | | Unknown.
focusunk7|int(11)|NO| |0| Unknown.
scrollunk1|int(11)|NO| |0| Unknown.
scrollunk2|int(11)|NO| |0| Unknown.
scrollunk3|int(11)|NO| |0| Unknown.
scrollunk4|int(11)|NO| |0| Unknown.
scrollunk5|int(11)|NO| |0| Unknown.
scrollunk6|varchar(32)|NO| | | Unknown.
scrollunk7|int(11)|NO| |0| Unknown.
UNK193|int(11)|NO| |0| Unknown.
purity|int(11)|NO| |0| The purity bonus of the item.
evoitem|int(11)|NO| |0| 
evoid|int(11)|NO| |0| 
evolvinglevel|int(11)|NO| |0| 
evomax|int(11)|NO| |0| 
clickname|varchar(64)|NO| | | The click effect name.
procname|varchar(64)|NO| | | The proc effect name.
wornname|varchar(64)|NO| | | The worn effect name.
focusname|varchar(64)|NO| | | The focus effect name.
scrollname|varchar(64)|NO| | | The scroll effect name.
dsmitigation|smallint(6)|NO| |0| The damage shield mitigation bonus of the item.
heroic\_str|smallint(6)|NO| |0| Heroic Strength bonus.
heroic\_int|smallint(6)|NO| |0| Heroic Intelligence bonus.
heroic\_wis|smallint(6)|NO| |0| Heroic Wisdom bonus.
heroic\_agi|smallint(6)|NO| |0| Heroic Agility bonus.
heroic\_dex|smallint(6)|NO| |0| Heroic Dexterity bonus.
heroic\_sta|smallint(6)|NO| |0| Heroic Stamina bonus.
heroic\_cha|smallint(6)|NO| |0| Heroic Charisma bonus.
heroic\_pr|smallint(6)|NO| |0| Heroic Poison Resistance bonus.
heroic\_dr|smallint(6)|NO| |0| Heroic Disease Resistance bonus.
heroic\_fr|smallint(6)|NO| |0| Heroic Fire Resistance bonus.
heroic\_cr|smallint(6)|NO| |0| Heroic Cold Resistance bonus.
heroic\_mr|smallint(6)|NO| |0| Heroic Magic Resistance bonus.
heroic\_svcorrup|smallint(6)|NO| |0| Heroic Corruption Resistance bonus.
healamt|smallint(6)|NO| |0| The heal amount bonus on the item.
spelldmg|smallint(6)|NO| |0| The spell damage bonus on the item.
clairvoyance|smallint(6)|NO| |0| The clairvoyance on the item.
backstabdmg|smallint(6)|NO| |0| The backstab damage on the item, 32767 is the maximum.
created|varchar(64)|NO| | | Who created the item.
elitematerial|smallint(6)|NO| |0| Unused.
ldonsellbackrate|smallint(6)|NO| |0| Leave this at 70.
scriptfileid|smallint(6)|NO| |0| The script used by the item (see [EVENT_ITEM_CLICK](https://github.com/EQEmu/Server/wiki/Perl-API---Perl-Sub-Event-Examples#event_item_click))
expendablearrow|smallint(6)|NO| |0| Determines whether or not an item is an expendable arrow. 0 = No, 1 = Yes
powersourcecapacity|smallint(6)|NO| |0| Unused.
bardeffect|smallint(6)|NO| |0| The spell ID of the bard effect on the item.
bardeffecttype|smallint(6)|NO| |0| The type of bard effect on the item.
bardlevel2|smallint(6)|NO| |0| Level that the bard effect will reach maximum power.
bardlevel|smallint(6)|NO| |0| The level required for the bard effect.
bardunk1|smallint(6)|NO| |0| Unknown.
bardunk2|smallint(6)|NO| |0| Unknown.
bardunk3|smallint(6)|NO| |0| Unknown.
bardunk4|smallint(6)|NO| |0| Unknown.
bardunk5|smallint(6)|NO| |0| Unknown.
bardname|varchar(64)|NO| | | The name of the Bard effect.
bardunk7|smallint(6)|NO| |0| Unknown.
UNK214|smallint(6)|NO| |0| Unknown.
UNK219|int(11)|NO| |0| Unknown.
UNK220|int(11)|NO| |0| Unknown.
UNK221|int(11)|NO| |0| Unknown.
heirloom|int(11)|NO| |0| Whether or not the item is an heirloom.
UNK223|int(11)|NO| |0| Unknown.
UNK224|int(11)|NO| |0| Unknown.
UNK225|int(11)|NO| |0| Unknown.
UNK226|int(11)|NO| |0| Unknown.
UNK227|int(11)|NO| |0| Unknown.
UNK228|int(11)|NO| |0| Unknown.
UNK229|int(11)|NO| |0| Unknown.
UNK230|int(11)|NO| |0| Unknown.
UNK231|int(11)|NO| |0| Unknown.
UNK232|int(11)|NO| |0| Unknown.
UNK233|int(11)|NO| |0| Unknown.
UNK234|int(11)|NO| |0| Unknown.
placeable|int(11)|NO| |0| Whether or not the item is placeable.
UNK236|int(11)|NO| |0| Unknown.
UNK237|int(11)|NO| |0| Unknown.
UNK238|int(11)|NO| |0| Unknown.
UNK239|int(11)|NO| |0| Unknown.
UNK240|int(11)|NO| |0| Unknown.
UNK241|int(11)|NO| |0| Unknown.
epicitem|int(11)|NO| |0| Whether or not the item is an epic item.