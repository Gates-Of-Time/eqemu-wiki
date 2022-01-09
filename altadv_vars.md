**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
skill\_id|int(11)|NO|PRI|0| 
name|varchar(128)|YES| | | 
cost|int(11)|YES| | | 
max\_level|int(11)|YES| | | 
hotkey\_sid|int(10) unsigned|NO| |0| 
hotkey\_sid2|int(10) unsigned|NO| |0| 
title\_sid|int(10) unsigned|NO| |0| 
desc\_sid|int(10) unsigned|NO| |0| 
type|tinyint(3) unsigned|NO| |1| 
spellid|int(10) unsigned|NO| |0| 
prereq\_skill|int(10) unsigned|NO| |0| 
prereq\_minpoints|int(10) unsigned|NO| |0| 
spell\_type|int(10) unsigned|NO| |0| 
spell\_refresh|int(10) unsigned|NO| |0| 
classes|int(10) unsigned|NO| |65534| 
berserker|int(10) unsigned|NO| |0| 
class\_type|int(10) unsigned|NO| |0| 
cost\_inc|tinyint(4)|NO| |0| 
aa\_expansion|smallint(3) unsigned|NO| |3| 
special\_category|int(10) unsigned|NO| |4294967295| 
sof\_type|tinyint(3) unsigned|NO| |1| 
sof\_cost\_inc|tinyint(3)|NO| |0| 
sof\_max\_level|tinyint(3) unsigned|NO| |1| 
sof\_next\_skill|int(10) unsigned|NO| |0| 
clientver|tinyint(3) unsigned|NO| |1| 
account\_time\_required|int(10) unsigned|NO| |0| 
sof\_current\_level|tinyint(3) unsigned|NO| |0| 
sof\_next\_id|int(10) unsigned|NO| |0| 
level\_inc|tinyint(3) unsigned|NO| |0| 