**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
id|int(11) unsigned|NO|PRI| |auto\_increment
name|tinytext|YES| | | 
parent\_list|int(11) unsigned|NO| |0| 
attack\_proc|smallint(5)|NO| |-1| 
proc\_chance|tinyint(3)|NO| |3| 
range\_proc|smallint(5)|NO| |-1| 
rproc\_chance|smallint(5)|NO| |0| 
defensive\_proc|smallint(5)|NO| |-1| 
dproc\_chance|smallint(5)|NO| |0| 
fail\_recast|int(11) unsigned|NO| |0| 
engaged\_no\_sp\_recast\_min|int(11) unsigned|NO| |0| 
engaged\_no\_sp\_recast\_max|int(11) unsigned|NO| |0| 
engaged\_b\_self\_chance|tinyint(3) unsigned|NO| |0| 
engaged\_b\_other\_chance|tinyint(3) unsigned|NO| |0| 
engaged\_d\_chance|tinyint(3) unsigned|NO| |0| 
pursue\_no\_sp\_recast\_min|int(3) unsigned|NO| |0| 
pursue\_no\_sp\_recast\_max|int(11) unsigned|NO| |0| 
pursue\_d\_chance|tinyint(3) unsigned|NO| |0| 
idle\_no\_sp\_recast\_min|int(11) unsigned|NO| |0| 
idle\_no\_sp\_recast\_max|int(11) unsigned|NO| |0| 
idle\_b\_chance|tinyint(11) unsigned|NO| |0| 