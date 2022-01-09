**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
id|int(11) unsigned|NO|PRI| |auto\_increment
charid|int(11) unsigned|NO| |0| 
charname|varchar(64)|NO| | | 
zone\_id|smallint(5)|NO|MUL|0| 
instance\_id|smallint(5) unsigned|NO|MUL|0| 
x|float|NO| |0| 
y|float|NO| |0| 
z|float|NO| |0| 
heading|float|NO| |0| 
time\_of\_death|datetime|NO| |0000-00-00 00:00:00| 
is\_rezzed|tinyint(3) unsigned|YES| |0| 
is\_buried|tinyint(3)|NO| |0| 
was\_at\_graveyard|tinyint(3)|NO| |0| 
is\_locked|tinyint(11)|YES| |0| 
exp|int(11) unsigned|YES| |0| 
size|int(11) unsigned|YES| |0| 
level|int(11) unsigned|YES| |0| 
race|int(11) unsigned|YES| |0| 
gender|int(11) unsigned|YES| |0| 
class|int(11) unsigned|YES| |0| 
deity|int(11) unsigned|YES| |0| 
texture|int(11) unsigned|YES| |0| 
helm\_texture|int(11) unsigned|YES| |0| 
copper|int(11) unsigned|YES| |0| 
silver|int(11) unsigned|YES| |0| 
gold|int(11) unsigned|YES| |0| 
platinum|int(11) unsigned|YES| |0| 
hair\_color|int(11) unsigned|YES| |0| 
beard\_color|int(11) unsigned|YES| |0| 
eye\_color\_1|int(11) unsigned|YES| |0| 
eye\_color\_2|int(11) unsigned|YES| |0| 
hair\_style|int(11) unsigned|YES| |0| 
face|int(11) unsigned|YES| |0| 
beard|int(11) unsigned|YES| |0| 
drakkin\_heritage|int(11) unsigned|YES| |0| 
drakkin\_tattoo|int(11) unsigned|YES| |0| 
drakkin\_details|int(11) unsigned|YES| |0| 
wc\_1|int(11) unsigned|YES| |0| 
wc\_2|int(11) unsigned|YES| |0| 
wc\_3|int(11) unsigned|YES| |0| 
wc\_4|int(11) unsigned|YES| |0| 
wc\_5|int(11) unsigned|YES| |0| 
wc\_6|int(11) unsigned|YES| |0| 
wc\_7|int(11) unsigned|YES| |0| 
wc\_8|int(11) unsigned|YES| |0| 
wc\_9|int(11) unsigned|YES| |0| 