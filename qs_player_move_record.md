**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
move\_id|int(11)|NO|PRI| |auto\_increment
time|timestamp|YES| | |on update CURRENT\_TIMESTAMP
char\_id|int(11)|YES| |0| 
from\_slot|mediumint(7)|YES| |0| 
to\_slot|mediumint(7)|YES| |0| 
stack\_size|mediumint(7)|YES| |0| 
char\_items|mediumint(7)|YES| |0| 
postaction|tinyint(1)|YES| |0| 