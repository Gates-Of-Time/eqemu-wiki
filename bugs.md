**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
id|int(11) unsigned|NO|PRI| |auto\_increment
zone|varchar(32)|NO| | | 
name|varchar(64)|NO| | | 
ui|varchar(128)|NO| | | 
x|float|NO| |0| 
y|float|NO| |0| 
z|float|NO| |0| 
type|varchar(64)|NO| | | 
flag|tinyint(3) unsigned|NO| | | 
target|varchar(64)|YES| | | 
bug|varchar(1024)|NO| | | 
date|date|NO| | | 
status|tinyint(3) unsigned|NO| |0| 