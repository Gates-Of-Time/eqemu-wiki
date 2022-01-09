**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
id|int(11)|NO|PRI| |auto\_increment
spawngroupID|int(11)|NO|MUL|0| 
zone|varchar(32)|YES|MUL| | 
version|smallint(5) unsigned|NO| |0| 
x|float(14,6)|NO| |0.000000| 
y|float(14,6)|NO| |0.000000| 
z|float(14,6)|NO| |0.000000| 
heading|float(14,6)|NO| |0.000000| 
respawntime|int(11)|NO| |0| 
variance|int(11)|NO| |0| 
pathgrid|int(10)|NO| |0| 
\_condition|mediumint(8) unsigned|NO| |0| 
cond\_value|mediumint(9)|NO| |1| 
enabled|tinyint(3) unsigned|NO| |1| 
animation|tinyint(3) unsigned|NO| |0| 