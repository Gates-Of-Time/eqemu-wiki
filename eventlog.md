**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
id|int(10) unsigned|NO|PRI| |auto\_increment
accountname|varchar(30)|NO| | | 
accountid|int(10) unsigned|YES| |0| 
status|int(5)|NO| |0| 
charname|varchar(64)|NO| | | 
target|varchar(64)|YES| |None| 
time|timestamp|NO| |CURRENT\_TIMESTAMP|on update CURRENT\_TIMESTAMP
descriptiontype|varchar(50)|NO| | | 
description|text|NO| | | 
event\_nid|int(11)|NO| |0| 