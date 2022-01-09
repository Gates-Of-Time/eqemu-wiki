**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
name|varchar(16)|NO|PRI| | 
address|text|NO| | | 
port|int(11)|NO| |0| 
player\_count|int(11)|NO| |0| 
last\_alive|timestamp|NO| |CURRENT\_TIMESTAMP|on update CURRENT\_TIMESTAMP
rain|char(1)|NO| |0| 