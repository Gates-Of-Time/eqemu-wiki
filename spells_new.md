**Field** | **Type** | **Null** | **Key** | **Default** | **Notes**
----- | ----- | ----- | ----- | ----- | ----- |
id | int(11) | NO | PRI | 0 | The spell description is contained in the dbstr_us.txt file in the EverQuest client.
name | varchar(64) | YES |  |  | The spell's name.
player\_1 | varchar(64) | YES |  | BLUE\_TRAIL | 
teleport\_zone | varchar(64) | YES |  |  | The zone you're teleporting to or the npc_types name of the NPC you want to spawn.
you\_cast | varchar(120) | YES |  |  | The message sent to others when you cast the spell.
other\_casts | varchar(120) | YES |  |  | The message seen when someone around you casts the spell.
cast\_on\_you | varchar(120) | YES |  |  | The message received when the spell is cast on you.
cast\_on\_other | varchar(120) | YES |  |  | The message recieved when the spell is cast on another.
spell\_fades | varchar(120) | YES |  |  | The message recieved when the spell fades.
range | int(11) | NO |  | 100 | The range of the spell.
aoerange | int(11) | NO |  | 0 | The range of the spell's area of effect if it is an area of effect spell.
pushback | int(11) | NO |  | 0 | The push back on the spell.
pushup | int(11) | NO |  | 0 | The push up on the spell.
cast\_time | int(11) | NO |  | 0 | Time, in milliseconds, it takes for the spell to cast.
recovery\_time | int(11) | NO |  | 0 | The time it takes in between casts of the spell for the spell to recover.
recast\_time | int(11) | NO |  | 0 | The recast time.
buffdurationformula | int(11) | NO |  | 7 | The formula used to calculate the duration of the spell.
buffduration | int(11) | NO |  | 65 | The duration of spell without the buff duration formula added in.
AEDuration | int(11) | NO |  | 0 | The duration of the area of effect.
mana | int(11) | NO |  | 0 | Amount of mana required to cast the spell.
effect\_base\_value1 | int(11) | NO |  | 100 | The amount or specific that is used for the effect id.
effect\_base\_value2 | int(11) | NO |  | 0 | The amount or specific that is used for the effect id.
effect\_base\_value3 | int(11) | NO |  | 0 | The amount or specific that is used for the effect id.
effect\_base\_value4 | int(11) | NO |  | 0 | The amount or specific that is used for the effect id.
effect\_base\_value5 | int(11) | NO |  | 0 | The amount or specific that is used for the effect id.
effect\_base\_value6 | int(11) | NO |  | 0 | The amount or specific that is used for the effect id.
effect\_base\_value7 | int(11) | NO |  | 0 | The amount or specific that is used for the effect id.
effect\_base\_value8 | int(11) | NO |  | 0 | The amount or specific that is used for the effect id.
effect\_base\_value9 | int(11) | NO |  | 0 | The amount or specific that is used for the effect id.
effect\_base\_value10 | int(11) | NO |  | 0 | The amount or specific that is used for the effect id.
effect\_base\_value11 | int(11) | NO |  | 0 | The amount or specific that is used for the effect id.
effect\_base\_value12 | int(11) | NO |  | 0 | The amount or specific that is used for the effect id.
effect\_limit\_value1 | int(11) | NO |  | 0 | The maximum amount that is used for the effect id.
effect\_limit\_value2 | int(11) | NO |  | 0 | The maximum amount that is used for the effect id.
effect\_limit\_value3 | int(11) | NO |  | 0 | The maximum amount that is used for the effect id.
effect\_limit\_value4 | int(11) | NO |  | 0 | The maximum amount that is used for the effect id.
effect\_limit\_value5 | int(11) | NO |  | 0 | The maximum amount that is used for the effect id.
effect\_limit\_value6 | int(11) | NO |  | 0 | The maximum amount that is used for the effect id.
effect\_limit\_value7 | int(11) | NO |  | 0 | The maximum amount that is used for the effect id.
effect\_limit\_value8 | int(11) | NO |  | 0 | The maximum amount that is used for the effect id.
effect\_limit\_value9 | int(11) | NO |  | 0 | The maximum amount that is used for the effect id.
effect\_limit\_value10 | int(11) | NO |  | 0 | The maximum amount that is used for the effect id.
effect\_limit\_value11 | int(11) | NO |  | 0 | The maximum amount that is used for the effect id.
effect\_limit\_value12 | int(11) | NO |  | 0 | The maximum amount that is used for the effect id.
max1 | int(11) | NO |  | 0 | The maximum effect base value.
max2 | int(11) | NO |  | 0 | The maximum effect base value.
max3 | int(11) | NO |  | 0 | The maximum effect base value.
max4 | int(11) | NO |  | 0 | The maximum effect base value.
max5 | int(11) | NO |  | 0 | The maximum effect base value.
max6 | int(11) | NO |  | 0 | The maximum effect base value.
max7 | int(11) | NO |  | 0 | The maximum effect base value.
max8 | int(11) | NO |  | 0 | The maximum effect base value.
max9 | int(11) | NO |  | 0 | The maximum effect base value.
max10 | int(11) | NO |  | 0 | The maximum effect base value.
max11 | int(11) | NO |  | 0 | The maximum effect base value.
max12 | int(11) | NO |  | 0 | The maximum effect base value.
icon | int(11) | NO |  | 0 | The icon ID used for spell gems. Uses new_icon now.
memicon | int(11) | NO |  | 0 | The old icon ID used for spell gems. Uses new_icon now.
components1 | int(11) | NO |  | -1 | The reagents necessary for the spell.
components2 | int(11) | NO |  | -1 | The reagents necessary for the spell.
components3 | int(11) | NO |  | -1 | The reagents necessary for the spell.
components4 | int(11) | NO |  | -1 | The reagents necessary for the spell.
component\_counts1 | int(11) | NO |  | 1 | The amount of reagents used.
component\_counts2 | int(11) | NO |  | 1 | The amount of reagents used.
component\_counts3 | int(11) | NO |  | 1 | The amount of reagents used.
component\_counts4 | int(11) | NO |  | 1 | The amount of reagents used.
NoexpendReagent1 | int(11) | NO |  | -1 | If it is a number between 1-4 it means component number 1-4 is a focus and not to expend it.
NoexpendReagent2 | int(11) | NO |  | -1 | If it is a number between 1-4 it means component number 1-4 is a focus and not to expend it.
NoexpendReagent3 | int(11) | NO |  | -1 | If it is a number between 1-4 it means component number 1-4 is a focus and not to expend it.
NoexpendReagent4 | int(11) | NO |  | -1 | If it is a number between 1-4 it means component number 1-4 is a focus and not to expend it.
formula1 | int(11) | NO |  | 100 | The formula used to determine the way the effect base value scales.
formula2 | int(11) | NO |  | 100 | The formula used to determine the way the effect base value scales.
formula3 | int(11) | NO |  | 100 | The formula used to determine the way the effect base value scales.
formula4 | int(11) | NO |  | 100 | The formula used to determine the way the effect base value scales.
formula5 | int(11) | NO |  | 100 | The formula used to determine the way the effect base value scales.
formula6 | int(11) | NO |  | 100 | The formula used to determine the way the effect base value scales.
formula7 | int(11) | NO |  | 100 | The formula used to determine the way the effect base value scales.
formula8 | int(11) | NO |  | 100 | The formula used to determine the way the effect base value scales.
formula9 | int(11) | NO |  | 100 | The formula used to determine the way the effect base value scales.
formula10 | int(11) | NO |  | 100 | The formula used to determine the way the effect base value scales.
formula11 | int(11) | NO |  | 100 | The formula used to determine the way the effect base value scales.
formula12 | int(11) | NO |  | 100 | The formula used to determine the way the effect base value scales.
LightType | int(11) | NO |  | 0 | 
goodEffect | int(11) | NO |  | 0 | Determines whether the spell is beneficial or detrimental.  0 = Detrimental, 1 = Beneficial, 2 = Beneficial, Group Only
Activated | int(11) | NO |  | 0 | 
resisttype | int(11) | NO |  | 0 |  Resist Types 
effectid1 | int(11) | NO |  | 254 | Determines what type of effect the effect id has. See  Spell Effect IDs 
effectid2 | int(11) | NO |  | 254 | Determines what type of effect the effect id has. See  Spell Effect IDs 
effectid3 | int(11) | NO |  | 254 | Determines what type of effect the effect id has. See  Spell Effect IDs 
effectid4 | int(11) | NO |  | 254 | Determines what type of effect the effect id has. See  Spell Effect IDs 
effectid5 | int(11) | NO |  | 254 | Determines what type of effect the effect id has. See  Spell Effect IDs 
effectid6 | int(11) | NO |  | 254 | Determines what type of effect the effect id has. See  Spell Effect IDs 
effectid7 | int(11) | NO |  | 254 | Determines what type of effect the effect id has. See  Spell Effect IDs 
effectid8 | int(11) | NO |  | 254 | Determines what type of effect the effect id has. See  Spell Effect IDs 
effectid9 | int(11) | NO |  | 254 | Determines what type of effect the effect id has. See  Spell Effect IDs 
effectid10 | int(11) | NO |  | 254 | Determines what type of effect the effect id has. See  Spell Effect IDs 
effectid11 | int(11) | NO |  | 254 | Determines what type of effect the effect id has. See  Spell Effect IDs 
effectid12 | int(11) | NO |  | 254 | Determines what type of effect the effect id has. See  Spell Effect IDs 
targettype | int(11) | NO |  | 2 | The target type of the spell.  Target Types 
basediff | int(11) | NO |  | 0 | Base difficulty fizzle adjustment.
skill | int(11) | NO |  | 98 | Determines the skill used to cast the spell. See  Skills 
zonetype | int(11) | NO |  | -1 | Determines the zone type necessary to cast the spell. -1 None, 0 Indoor, 1 Outdoor, 2 Dungeon, 255 Any
EnvironmentType | int(11) | NO |  | 0 | Determines the environment type necessary to cast the spell. 0 = Everywhere, 12 = Cities, 24 = Planes
TimeOfDay | int(11) | NO |  | 0 | Determines the time of day necessary to cast the spell. 0 = Any, 1 = Day Time, 2 = Night Time
classes1 | int(11) | NO |  | 255 | Defines what level each class can use the spell. See  Classes 
classes2 | int(11) | NO |  | 255 | Defines what level each class can use the spell. See  Classes 
classes3 | int(11) | NO |  | 255 | Defines what level each class can use the spell. See  Classes 
classes4 | int(11) | NO |  | 255 | Defines what level each class can use the spell. See  Classes 
classes5 | int(11) | NO |  | 255 | Defines what level each class can use the spell. See  Classes 
classes6 | int(11) | NO |  | 255 | Defines what level each class can use the spell. See  Classes 
classes7 | int(11) | NO |  | 255 | Defines what level each class can use the spell. See  Classes 
classes8 | int(11) | NO |  | 255 | Defines what level each class can use the spell. See  Classes 
classes9 | int(11) | NO |  | 255 | Defines what level each class can use the spell. See  Classes 
classes10 | int(11) | NO |  | 255 | Defines what level each class can use the spell. See  Classes 
classes11 | int(11) | NO |  | 255 | Defines what level each class can use the spell. See  Classes 
classes12 | int(11) | NO |  | 255 | Defines what level each class can use the spell. See  Classes 
classes13 | int(11) | NO |  | 255 | Defines what level each class can use the spell. See  Classes 
classes14 | int(11) | NO |  | 255 | Defines what level each class can use the spell. See  Classes 
classes15 | int(11) | NO |  | 255 | Defines what level each class can use the spell. See  Classes 
classes16 | int(11) | NO |  | 255 | Defines what level each class can use the spell. See  Classes 
CastingAnim | int(11) | NO |  | 44 | The casting animation. See [[Animation Reference (DoAnim)
TargetAnim | int(11) | NO |  | 13 | The target animation.
TravelType | int(11) | NO |  | 0 | Determines the travel type of the spell.
SpellAffectIndex | int(11) | NO |  | -1 | 
disallow\_sit | int(11) | NO |  | 0 | 
deities0 | int(11) | NO |  | 0 | 
deities1 | int(11) | NO |  | 0 | The same as the deity list, except none for agnostic.  Deity List 
deities2 | int(11) | NO |  | 0 | The same as the deity list, except none for agnostic.  Deity List 
deities3 | int(11) | NO |  | 0 | The same as the deity list, except none for agnostic.  Deity List 
deities4 | int(11) | NO |  | 0 | The same as the deity list, except none for agnostic.  Deity List 
deities5 | int(11) | NO |  | 0 | The same as the deity list, except none for agnostic.  Deity List 
deities6 | int(11) | NO |  | 0 | The same as the deity list, except none for agnostic.  Deity List 
deities7 | int(11) | NO |  | 0 | The same as the deity list, except none for agnostic.  Deity List 
deities8 | int(11) | NO |  | 0 | The same as the deity list, except none for agnostic.  Deity List 
deities9 | int(11) | NO |  | 0 | The same as the deity list, except none for agnostic.  Deity List 
deities10 | int(11) | NO |  | 0 | The same as the deity list, except none for agnostic.  Deity List 
deities11 | int(11) | NO |  | 0 | The same as the deity list, except none for agnostic.  Deity List 
deities12 | int(12) | NO |  | 0 | The same as the deity list, except none for agnostic.  Deity List 
deities13 | int(11) | NO |  | 0 | The same as the deity list, except none for agnostic.  Deity List 
deities14 | int(11) | NO |  | 0 | The same as the deity list, except none for agnostic.  Deity List 
deities15 | int(11) | NO |  | 0 | The same as the deity list, except none for agnostic.  Deity List 
deities16 | int(11) | NO |  | 0 | The same as the deity list, except none for agnostic.  Deity List 
field142 | int(11) | NO |  | 100 | 
field143 | int(11) | NO |  | 0 | 
new\_icon | int(11) | NO |  | 161 | The spell's icon.
spellanim | int(11) | NO |  | 0 | The spell animation.
uninterruptable | int(11) | NO |  | 0 | Whether or not the spell can be interrupted. 0 = Interruptable, 1 = Uninterruptable
ResistDiff | int(11) | NO |  | -150 | The resist difference by default.
dot\_stacking\_exempt | int(11) | NO |  | 0 | Whether or not the damage over time can stack.
deleteable | int(11) | NO |  | 0 | Whether or not the spell is deletable. 0 = Not Deletable, 1 = Deletable
RecourseLink | int(11) | NO |  | 0 | The proc on a spell.
no\_partial\_resist | int(11) | NO |  | 0 | 
field152 | int(11) | NO |  | 0 | 
field153 | int(11) | NO |  | 0 | 
short\_buff\_box | int(11) | NO |  | -1 | 0 = No, 1 = Yes
descnum | int(11) | NO |  | 0 | See the type column in  dbstr_us.txt 
typedescnum | int(11) | YES |  |  | The typedescnum value is used client side. See the type column in  dbstr_us.txt 
effectdescnum | int(11) | YES |  |  | See the type column in  dbstr_us.txt 
effectdescnum2 | int(11) | NO |  | 0 | 
npc\_no\_los | int(11) | NO |  | 0 | 
field160 | int(11) | NO |  | 0 | 
reflectable | int(11) | NO |  | 0 | 
bonushate | int(11) | NO |  | 0 | 
field163 | int(11) | NO |  | 100 | 
field164 | int(11) | NO |  | -150 | 
ldon\_trap | int(11) | NO |  | 0 | 
EndurCost | int(11) | NO |  | 0 | Endurance used to cast the spell.
EndurTimerIndex | int(11) | NO |  | 0 | The time in between endurance costs.
IsDiscipline | int(11) | NO |  | 0 | 
field169 | int(11) | NO |  | 0 | 
field170 | int(11) | NO |  | 0 | 
field171 | int(11) | NO |  | 0 | 
field172 | int(11) | NO |  | 0 | 
HateAdded | int(11) | NO |  | 0 | The amount of hate added by the spell.
EndurUpkeep | int(11) | NO |  | 0 | The endurance up keep for the spell.
numhitstype | int(11) | NO |  | 0 |  Numhit_Types Deterimes what behavior ticks down the numhits counter.
numhits | int(11) | NO |  | 0 | Counter that ticks down when a specified condition is met.
pvpresistbase | int(11) | NO |  | -150 | The resist base in player versus player.
pvpresistcalc | int(11) | NO |  | 100 | The calculation for resistances in player versus player.
pvpresistcap | int(11) | NO |  | -150 | The maximum resists for player versus player.
spell\_category | int(11) | NO |  | -99 | The spell's category.  Spell Categories 
field181 | int(11) | NO |  | 7 | 
field182 | int(11) | NO |  | 65 | 
pcnpc\_only\_flag | int(11) | YES |  | 0 | 
cast\_not\_standing | int(11) | YES |  | 0 | 
can\_mgb | int(11) | NO |  | 0 | Determines whether or not the spell can be used as a mass group buff. 0 = No, 1 = Yes
nodispell | int(11) | NO |  | -1 | Determines whether or not the spell can be dispelled. 0 = Can be dispelled. 1 = Can be cancelled with a cure, but not dispelled.
npc\_category | int(11) | NO |  | 0 | npc_category: 0 = Non NPC Spell, 1 = Area of Effect Detrimental, 2 = Single Target Detrimental, 3 = Buffs, 4 = Pet Spells, 5 = Healing Spells, 6 = Gate or last cast, 7 = Debuffs, 8 = Dispells
npc\_usefulness | int(11) | NO |  | 0 | Used in conjunction with npc_category. The higher the number, the more useful, the lower the number, the less useful.
MinResist | int(11) | NO |  | 0 | 
MaxResist | int(11) | NO |  | 0 | 
viral\_targets | int(11) | NO |  | 0 | 
viral\_timer | int(11) | NO |  | 0 | 
nimbuseffect | int(11) | YES |  | 0 | 
ConeStartAngle | int(11) | NO |  | 0 | 
ConeStopAngle | int(11) | NO |  | 0 | 
sneaking | int(11) | NO |  | 0 | 
not\_extendable | int(11) | NO |  | 0 | 
field198 | int(11) | NO |  | 0 | 
field199 | int(11) | NO |  | 1 | 
suspendable | int(11) | YES |  | 0 | 
viral\_range | int(11) | NO |  | 0 | 
songcap | int(11) | YES |  | 0 | 
field203 | int(11) | YES |  | 0 | 
field204 | int(11) | YES |  | 0 | 
no\_block | int(11) | NO |  | 0 | 
field206 | int(11) | YES |  | -1 | 
spellgroup | int(11) | YES |  | 0 | The spell's group. See  Spell Groups 
rank | int(11) | NO |  | 0 | 
field209 | int(11) | YES |  | 0 | 
field210 | int(11) | YES |  | 1 | 
CastRestriction | int(11) | NO |  | 0 | 
allowrest | int(11) | YES |  | 0 | 
InCombat | int(11) | NO |  | 0 | 
OutofCombat | int(11) | NO |  | 0 | 
field215 | int(11) | YES |  | 0 | 
field216 | int(11) | YES |  | 0 | 
field217 | int(11) | YES |  | 0 | 
aemaxtargets | int(11) | NO |  | 0 | 
maxtargets | int(11) | YES |  | 0 | 
field220 | int(11) | YES |  | 0 | 
field221 | int(11) | YES |  | 0 | 
field222 | int(11) | YES |  | 0 | 
field223 | int(11) | YES |  | 0 | 
persistdeath | int(11) | YES |  | 0 | 
field225 | int(11) | NO |  | 0 | 
field226 | int(11) | NO |  | 0 | 
min\_dist | float | NO |  | 0 | 
min\_dist\_mod | float | NO |  | 0 | 
max\_dist | float | NO |  | 0 | 
max\_dist\_mod | float | NO |  | 0 | 
min\_range | int(11) | NO |  | 0 | 
field232 | int(11) | NO |  | 0 | 
field233 | int(11) | NO |  | 0 | 
field234 | int(11) | NO |  | 0 | 
field235 | int(11) | NO |  | 0 | 
field236 | int(11) | NO |  | 0 | 