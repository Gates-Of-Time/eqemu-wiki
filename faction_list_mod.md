**Field**|**Type**|**Null**|**Key**|**Default**|**Notes**
-----|-----|-----|-----|-----|-----
id|int(10) unsigned|NO|PRI| |auto\_increment
faction\_id|int(10) unsigned|NO|MUL| | 
mod|smallint(6)|NO| | | mod_value
mod\_name|varchar(16)|NO| | | -[crd][value]

There are 3 types of modifications, (r)ace, (c)lass, and (d)eity.  The mod name consists of the letter indicated followed by the id of the race/class/deity.  

For example, an entry with mod_name r4 and a mod of 10, means that all characters of race 4 (wood elf) gain 10 faction points from the base faction value just for being wood elves...  well that and those kinky outfits they wear.