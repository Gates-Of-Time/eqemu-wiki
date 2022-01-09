**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
ServerID|int(10) unsigned|NO|PRI| |auto\_increment
ServerLongName|varchar(100)|NO|PRI| | 
ServerTagDescription|varchar(50)|NO| | | 
ServerShortName|varchar(25)|NO| | | 
ServerListTypeID|int(11)|NO| | | 
ServerLastLoginDate|datetime|YES| | | 
ServerLastIPAddr|varchar(15)|YES| | | 
ServerAdminID|int(11)|NO| | | 
ServerTrusted|int(11)|NO| | | 
Note|varchar(300)|YES| | | 