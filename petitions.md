**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
dib|int(10) unsigned|NO|PRI| |auto\_increment
petid|int(10) unsigned|NO|MUL|0| 
charname|varchar(32)|NO| | | 
accountname|varchar(32)|NO| | | 
lastgm|varchar(32)|NO| | | 
petitiontext|text|NO| | | 
gmtext|text|YES| | | 
zone|varchar(32)|NO| | | 
urgency|int(11)|NO| |0| 
charclass|int(11)|NO| |0| 
charrace|int(11)|NO| |0| 
charlevel|int(11)|NO| |0| 
checkouts|int(11)|NO| |0| 
unavailables|int(11)|NO| |0| 
ischeckedout|tinyint(4)|NO| |0| 
senttime|bigint(11)|NO| |0| 