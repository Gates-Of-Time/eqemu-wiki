**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
id|int(11)|NO|PRI| |auto\_increment
doorid|smallint(4)|NO| |0| 
zone|varchar(32)|YES|MUL| | 
version|smallint(5)|NO| |0| 
name|varchar(32)|NO| | | 
pos\_y|float|NO| |0| 
pos\_x|float|NO| |0| 
pos\_z|float|NO| |0| 
heading|float|NO| |0| 
opentype|smallint(4)|NO| |0| 
guild|smallint(4)|NO| |0| 
lockpick|smallint(4)|NO| |0| 
keyitem|int(11)|NO| |0| 
nokeyring|tinyint(3) unsigned|NO| |0| 
triggerdoor|smallint(4)|NO| |0| 
triggertype|smallint(4)|NO| |0| 
disable\_timer|tinyint(2)|NO| |0| 
doorisopen|smallint(4)|NO| |0| 
door\_param|int(4)|NO| |0| 
dest\_zone|varchar(32)|YES| |NONE| 
dest\_instance|int(10) unsigned|NO| |0| 
dest\_x|float|YES| |0| 
dest\_y|float|YES| |0| 
dest\_z|float|YES| |0| 
dest\_heading|float|YES| |0| 
invert\_state|int(11)|YES| |0| 
incline|int(11)|YES| |0| 
size|smallint(5) unsigned|NO| |100| 
buffer|float|YES| |0| 
client\_version\_mask|int(10) unsigned|NO| |4294967295| 
is\_ldon\_door|smallint(6)|NO| |0| 