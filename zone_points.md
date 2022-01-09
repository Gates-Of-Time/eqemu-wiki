**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
id|int(11)|NO|PRI| |auto\_increment
zone|varchar(32)|YES| | | 
version|int(11)|NO| |0| 
number|smallint(4) unsigned|NO|MUL|1| 
y|float|NO| |0| 
x|float|NO| |0| 
z|float|NO| |0| 
heading|float|NO| |0| 
target\_y|float|NO| |0| 
target\_x|float|NO| |0| 
target\_z|float|NO| |0| 
target\_heading|float|NO| |0| 
zoneinst|smallint(5) unsigned|YES| |0| 
target\_zone\_id|int(10) unsigned|NO|MUL|0| 
target\_instance|int(10) unsigned|NO| |0| 
buffer|float|YES| |0| 
client\_version\_mask|int(10) unsigned|NO| |4294967295| 