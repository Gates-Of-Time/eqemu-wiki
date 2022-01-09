**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
id|int(11)|NO|PRI| |auto\_increment
from|varchar(64)|NO| | | 
to|varchar(64)|NO| | | 
message|varchar(256)|NO| | | 
minstatus|smallint(5)|NO| | | 
guilddbid|int(11)|NO| | | 
type|tinyint(3)|NO| | | 
timerecorded|timestamp|NO| |CURRENT\_TIMESTAMP|on update CURRENT\_TIMESTAMP