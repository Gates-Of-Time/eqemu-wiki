**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
id|int(11) unsigned|NO|PRI| |auto\_increment
npc\_spells\_id|int(11)|NO|MUL|0| 
spellid|smallint(5)|NO| |0| 
type|int(10) unsigned|NO| |0| 
minlevel|tinyint(3) unsigned|NO| |0| 
maxlevel|tinyint(3) unsigned|NO| |255| 
manacost|smallint(5)|NO| |-1| 
recast\_delay|int(11)|NO| |-1| 
priority|smallint(5)|NO| |0| 
resist\_adjust|int(11)|YES| | | 