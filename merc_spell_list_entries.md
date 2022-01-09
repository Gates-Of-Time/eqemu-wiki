**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
merc\_spell\_list\_entry\_id|int(10) unsigned|NO|PRI| |auto\_increment
merc\_spell\_list\_id|int(10) unsigned|NO|MUL| | 
spell\_id|int(10) unsigned|NO| | | 
spell\_type|int(10) unsigned|NO| |0| 
stance\_id|tinyint(3) unsigned|NO| |0| 
minlevel|tinyint(3) unsigned|NO| |1| 
maxlevel|tinyint(3) unsigned|NO| |255| 
slot|tinyint(4)|NO| |-1| 
procChance|tinyint(3) unsigned|NO| |0| 