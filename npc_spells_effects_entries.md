**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
id|int(11) unsigned|NO|PRI| |auto\_increment
npc\_spells\_effects\_id|int(11)|NO|MUL|0| 
spell\_effect\_id|smallint(5)|NO| |0| 
minlevel|tinyint(3) unsigned|NO| |0| 
maxlevel|tinyint(3) unsigned|NO| |255| 
se\_base|int(11)|NO| |0| 
se\_limit|int(11)|NO| |0| 
se\_max|int(11)|NO| |0| 