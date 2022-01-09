**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
taskid|int(11) unsigned|NO|PRI|0| 
activityid|int(11) unsigned|NO|PRI|0| 
step|int(11) unsigned|NO| |0| 
activitytype|tinyint(3) unsigned|NO| |0| 
text1|varchar(64)|NO| | | 
text2|varchar(64)|NO| | | 
text3|varchar(128)|NO| | | 
goalid|int(11) unsigned|NO| |0| 
goalmethod|int(10) unsigned|NO| |0| 
goalcount|int(11)|YES| |1| 
delivertonpc|int(11) unsigned|NO| |0| 
zoneid|int(11)|NO| |0| 
optional|tinyint(1)|NO| |0| 