**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
id|int(11)|NO|PRI| |auto\_increment
name|varchar(64)|NO| | | 
tradeskill|smallint(6)|NO| |0| 
skillneeded|smallint(6)|NO| |0| 
trivial|smallint(6)|NO| |0| 
nofail|tinyint(1)|NO| |0| 
replace\_container|tinyint(1)|NO| |0| 
notes|tinytext|YES| | | 
must\_learn|tinyint(4)|NO| |0| 
quest|tinyint(1)|NO| |0| 
enabled|tinyint(1)|NO| |1| 