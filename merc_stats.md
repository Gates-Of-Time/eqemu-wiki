**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
merc\_npc\_type\_id|int(11) unsigned|NO|PRI| | 
clientlevel|tinyint(2) unsigned|NO|PRI|1| 
level|tinyint(2) unsigned|NO| |1| 
hp|int(11)|NO| |1| 
mana|int(11)|NO| |0| 
AC|smallint(5)|NO| |1| 
ATK|mediumint(9)|NO| |1| 
STR|mediumint(8) unsigned|NO| |75| 
STA|mediumint(8) unsigned|NO| |75| 
DEX|mediumint(8) unsigned|NO| |75| 
AGI|mediumint(8) unsigned|NO| |75| 
\_INT|mediumint(8) unsigned|NO| |80| 
WIS|mediumint(8) unsigned|NO| |80| 
CHA|mediumint(8) unsigned|NO| |75| 
MR|smallint(5)|NO| |15| 
CR|smallint(5)|NO| |15| 
DR|smallint(5)|NO| |15| 
FR|smallint(5)|NO| |15| 
PR|smallint(5)|NO| |15| 
Corrup|smallint(5)|NO| |15| 
mindmg|int(10) unsigned|NO| |1| 
maxdmg|int(10) unsigned|NO| |1| 
attack\_count|smallint(6)|NO| |0| 
attack\_speed|tinyint(3)|NO| |0| 
attack\_delay|tinyint(3) unsigned|NO| |30| 
special\_abilities|text|YES| | | 
Accuracy|mediumint(9)|NO| |0| 
hp\_regen\_rate|int(11) unsigned|NO| |1| 
mana\_regen\_rate|int(11) unsigned|NO| |1| 
runspeed|float|NO| |0| 
statscale|int(11)|NO| |100| 
spellscale|float|NO| |100| 
healscale|float|NO| |100| 