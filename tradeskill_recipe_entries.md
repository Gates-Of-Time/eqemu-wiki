**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
id|int(11)|NO|PRI| |auto\_increment
recipe\_id|int(11)|NO|MUL|0| 
item\_id|int(11)|NO|MUL|0| 
successcount|tinyint(2)|NO| |0| 
failcount|tinyint(2)|NO| |0| 
componentcount|tinyint(2)|NO| |1| 
salvagecount|tinyint(2)|NO| |0| 
iscontainer|tinyint(1)|NO| |0| 