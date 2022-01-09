**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
id|int(11)|NO|PRI| |auto\_increment
name|varchar(30)|NO|UNI| | 
charname|varchar(64)|NO| | | 
sharedplat|int(11) unsigned|NO| |0| 
password|varchar(50)|NO| | | 
status|int(5)|NO| |0| 
lsaccount\_id|int(11) unsigned|YES|UNI| | 
gmspeed|tinyint(3) unsigned|NO| |0| 
revoked|tinyint(3) unsigned|NO| |0| 
karma|int(5) unsigned|NO| |0| 
minilogin\_ip|varchar(32)|NO| | | 
hideme|tinyint(4)|NO| |0| 
rulesflag|tinyint(1) unsigned|NO| |0| 
suspendeduntil|datetime|NO| |0000-00-00 00:00:00| 
time\_creation|int(10) unsigned|NO| |0| 
expansion|tinyint(4)|NO| |0| 
ban\_reason|text|YES| | | 
suspend\_reason|text|YES| | | 