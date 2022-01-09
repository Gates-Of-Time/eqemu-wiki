**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
id|int(11) unsigned|NO|PRI| |auto\_increment
zoneid|int(10) unsigned|NO|MUL|0| 
version|smallint(5)|NO| |0| 
max\_x|float|NO| |2000| 
max\_y|float|NO| |2000| 
max\_z|float|NO| |10000| 
min\_x|float|NO| |-2000| 
min\_y|float|NO| |-2000| 
heading|float|NO| |0| 
name|varchar(16)|NO| | | 
item|int(10) unsigned|NO| |0| 
max\_allowed|int(10) unsigned|NO| |1| 
comment|varchar(255)|NO| | | 
respawn\_timer|bigint(20) unsigned|NO| |300000| 