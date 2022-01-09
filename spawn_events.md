**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
id|int(10) unsigned|NO|PRI| |auto\_increment
zone|varchar(32)|YES| | | 
cond\_id|mediumint(8) unsigned|NO| |0| 
name|varchar(255)|NO| | | 
period|int(10) unsigned|NO| |0| 
next\_minute|tinyint(3) unsigned|NO| |0| 
next\_hour|tinyint(3) unsigned|NO| |0| 
next\_day|tinyint(3) unsigned|NO| |0| 
next\_month|tinyint(3) unsigned|NO| |0| 
next\_year|int(10) unsigned|NO| |0| 
enabled|tinyint(4)|NO| |1| 
action|tinyint(3) unsigned|NO| |0| 
argument|mediumint(9)|NO| |0| 
strict|tinyint(4)|NO| |0| 