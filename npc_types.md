**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
id|int(11)|NO|PRI| |auto\_increment
name|text|NO| | | 
lastname|varchar(32)|YES| | | 
level|tinyint(2) unsigned|NO| |0| 
race|smallint(5) unsigned|NO| |0| 
class|tinyint(2) unsigned|NO| |0| 
bodytype|int(11)|NO| |1| 
hp|int(11)|NO| |0| 
mana|int(11)|NO| |0| 
gender|tinyint(2) unsigned|NO| |0| 
texture|tinyint(2) unsigned|NO| |0| 
helmtexture|tinyint(2) unsigned|NO| |0| 
herosforgemodel|int(11)|NO| |0| 
size|float|NO| |0| 
hp\_regen\_rate|int(11) unsigned|NO| |0| 
mana\_regen\_rate|int(11) unsigned|NO| |0| 
loottable\_id|int(11) unsigned|NO| |0| 
merchant\_id|int(11) unsigned|NO| |0| 
alt\_currency\_id|int(11) unsigned|NO| |0| 
npc\_spells\_id|int(11) unsigned|NO| |0| 
npc\_spells\_effects\_id|int(11) unsigned|NO| |0| 
npc\_faction\_id|int(11)|NO| |0| 
adventure\_template\_id|int(10) unsigned|NO| |0| 
trap\_template|int(10) unsigned|YES| |0| 
mindmg|int(10) unsigned|NO| |0| 
maxdmg|int(10) unsigned|NO| |0| 
attack\_count|smallint(6)|NO| |-1| 
npcspecialattks|varchar(36)|NO| | | 
special\_abilities|text|YES| | | 
aggroradius|int(10) unsigned|NO| |0| 
assistradius|int(10) unsigned|NO| |0| 
face|int(10) unsigned|NO| |1| 
luclin\_hairstyle|int(10) unsigned|NO| |1| 
luclin\_haircolor|int(10) unsigned|NO| |1| 
luclin\_eyecolor|int(10) unsigned|NO| |1| 
luclin\_eyecolor2|int(10) unsigned|NO| |1| 
luclin\_beardcolor|int(10) unsigned|NO| |1| 
luclin\_beard|int(10) unsigned|NO| |0| 
drakkin\_heritage|int(10)|NO| |0| 
drakkin\_tattoo|int(10)|NO| |0| 
drakkin\_details|int(10)|NO| |0| 
armortint\_id|int(10) unsigned|NO| |0| 
armortint\_red|tinyint(3) unsigned|NO| |0| 
armortint\_green|tinyint(3) unsigned|NO| |0| 
armortint\_blue|tinyint(3) unsigned|NO| |0| 
d\_melee\_texture1|int(11)|NO| |0| 
d\_melee\_texture2|int(11)|NO| |0| 
ammo\_idfile|varchar(30)|NO| |IT10| 
prim\_melee\_type|tinyint(4) unsigned|NO| |28| 
sec\_melee\_type|tinyint(4) unsigned|NO| |28| 
ranged\_type|tinyint(4) unsigned|NO| |7| 
runspeed|float|NO| |0| 
MR|smallint(5)|NO| |0| 
CR|smallint(5)|NO| |0| 
DR|smallint(5)|NO| |0| 
FR|smallint(5)|NO| |0| 
PR|smallint(5)|NO| |0| 
Corrup|smallint(5)|NO| |0| 
PhR|smallint(5) unsigned|NO| |0| 
see\_invis|smallint(4)|NO| |0| 
see\_invis\_undead|smallint(4)|NO| |0| 
qglobal|int(2) unsigned|NO| |0| 
AC|smallint(5)|NO| |0| 
npc\_aggro|tinyint(4)|NO| |0| 
spawn\_limit|tinyint(4)|NO| |0| 
attack\_speed|float|NO| |0| 
attack\_delay|tinyint(3) unsigned|NO| |30| 
findable|tinyint(4)|NO| |0| 
STR|mediumint(8) unsigned|NO| |75| 
STA|mediumint(8) unsigned|NO| |75| 
DEX|mediumint(8) unsigned|NO| |75| 
AGI|mediumint(8) unsigned|NO| |75| 
\_INT|mediumint(8) unsigned|NO| |80| 
WIS|mediumint(8) unsigned|NO| |75| 
CHA|mediumint(8) unsigned|NO| |75| 
see\_hide|tinyint(4)|NO| |0| 
see\_improved\_hide|tinyint(4)|NO| |0| 
trackable|tinyint(4)|NO| |1| 
isbot|tinyint(4)|NO| |0| 
exclude|tinyint(4)|NO| |1| 
ATK|mediumint(9)|NO| |0| 
Accuracy|mediumint(9)|NO| |0| 
Avoidance|mediumint(9) unsigned|NO| |0| 
slow\_mitigation|smallint(4)|NO| |0| 
version|smallint(5) unsigned|NO| |0| 
maxlevel|tinyint(3)|NO| |0| 	The max level of the NPC. This makes the mob capable of spawning between levels 'level' to 'maxlevel'.  Optionally can set resists, mana regen, hp regen, mindmg and maxdmg to 0 to auto-set based on level or to a base level and use scalerate to scale these.  HP and stats are scaled-only and should not be set to 0.
scalerate|int(11)|NO| |100| 
private\_corpse|tinyint(3) unsigned|NO| |0| 
unique\_spawn\_by\_name|tinyint(3) unsigned|NO| |0| 
underwater|tinyint(3) unsigned|NO| |0| 
isquest|tinyint(3)|NO| |0| 
emoteid|int(10) unsigned|NO| |0| 
spellscale|float|NO| |100| 
healscale|float|NO| |100| 
no\_target\_hotkey|tinyint(1) unsigned|NO| |0| 
raid\_target|tinyint(1) unsigned|NO| |0| 
armtexture|tinyint(2)|NO| |0| 
bracertexture|tinyint(2)|NO| |0| 
handtexture|tinyint(2)|NO| |0| 
legtexture|tinyint(2)|NO| |0| 
feettexture|tinyint(2)|NO| |0| 
light|tinyint(2)|NO| |0| 
walkspeed|tinyint(2)|NO| |0| 
peqid|int(11)|NO| |0| 
unique\_|tinyint(2)|NO| |0| 
fixed|tinyint(2)|NO| |0| 
ignore\_despawn|tinyint(2)|NO| |0| 
show\_name|tinyint(2)|NO| |1| 
untargetable|tinyint(2)|NO| |0| 
maxlevel|tinyint(3)|NO| |0|
model|smallint(5)|NO| |0| 	Enter a model value here to override race model on client.  Very handy for things like races that have bane weapons, as you can use the new model here, and change the race field back to the old model.