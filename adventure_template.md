|Field|Type|Null|Key|Default|Extra|
-----|-----|-----|-----|-----|-----
id|int(10) unsigned|NO|PRI| | 
zone|varchar(64)|NO| | | 
zone\_version|tinyint(3) unsigned|NO| |0| 
is\_hard|tinyint(3) unsigned|NO| |0| 
is\_raid|tinyint(3) unsigned|NO| |0| 
min\_level|tinyint(3) unsigned|NO| |1| 
max\_level|tinyint(3) unsigned|NO| |65| 
type|tinyint(3) unsigned|NO| |0| 
type\_data|int(10) unsigned|NO| |0| 
type\_count|smallint(5) unsigned|NO| |0| 
assa\_x|float|NO| |0| 
assa\_y|float|NO| |0| 
assa\_z|float|NO| |0| 
assa\_h|float|NO| |0| 
text|varchar(511)|YES| | | 
duration|int(10) unsigned|NO| |7200| 
zone\_in\_time|int(10) unsigned|NO| |1800| 
win\_points|smallint(5) unsigned|NO| |0| 
lose\_points|smallint(5) unsigned|NO| |0| 
theme|tinyint(3) unsigned|NO| |1| 
zone\_in\_zone\_id|smallint(5) unsigned|NO| |0| 
zone\_in\_x|float|NO| |0| 
zone\_in\_y|float|NO| |0| 
zone\_in\_object\_id|smallint(4)|NO| |0| 
dest\_x|float|NO| |0| 
dest\_y|float|NO| |0| 
dest\_z|float|NO| |0| 
dest\_h|float|NO| |0| 
graveyard\_zone\_id|int(10) unsigned|NO| |0| 
graveyard\_x|float|NO| |0| 
graveyard\_y|float|NO| |0| 
graveyard\_z|float|NO| |0| 
graveyard\_radius|float unsigned|NO| |0| 