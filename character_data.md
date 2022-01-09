**Field**|**Type**|**Null**|**Key**|**Default**|**Extra**
-----|-----|-----|-----|-----|-----
id                      | int(11) unsigned      | NO   | PRI | NULL    | auto_increment |
account_id              | int(11)               | NO   | MUL | 0       |                |
name                    | varchar(64)           | NO   | UNI |         |                |
last_name               | varchar(64)           | NO   |     |         |                |
title                   | varchar(32)           | NO   |     |         |                |
suffix                  | varchar(32)           | NO   |     |         |                |
zone_id                 | int(11) unsigned      | NO   |     | 0       |                |
zone_instance           | int(11) unsigned      | NO   |     | 0       |                |
y                       | float                 | NO   |     | 0       |                |
x                       | float                 | NO   |     | 0       |                |
z                       | float                 | NO   |     | 0       |                |
heading                 | float                 | NO   |     | 0       |                |
gender                  | tinyint(11) unsigned  | NO   |     | 0       |                |
race                    | smallint(11) unsigned | NO   |     | 0       |                |
class                   | tinyint(11) unsigned  | NO   |     | 0       |                |
level                   | int(11) unsigned      | NO   |     | 0       |                |
deity                   | int(11) unsigned      | NO   |     | 0       |                |
birthday                | int(11) unsigned      | NO   |     | 0       |                |
last_login              | int(11) unsigned      | NO   |     | 0       |                |
time_played             | int(11) unsigned      | NO   |     | 0       |                |
level2                  | tinyint(11) unsigned  | NO   |     | 0       |                |
anon                    | tinyint(11) unsigned  | NO   |     | 0       |                |
gm                      | tinyint(11) unsigned  | NO   |     | 0       |                |
face                    | int(11) unsigned      | NO   |     | 0       |                |
hair_color              | tinyint(11) unsigned  | NO   |     | 0       |                |
hair_style              | tinyint(11) unsigned  | NO   |     | 0       |                |
beard                   | tinyint(11) unsigned  | NO   |     | 0       |                |
beard_color             | tinyint(11) unsigned  | NO   |     | 0       |                |
eye_color_1             | tinyint(11) unsigned  | NO   |     | 0       |                |
eye_color_2             | tinyint(11) unsigned  | NO   |     | 0       |                |
drakkin_heritage        | int(11) unsigned      | NO   |     | 0       |                |
drakkin_tattoo          | int(11) unsigned      | NO   |     | 0       |                |
drakkin_details         | int(11) unsigned      | NO   |     | 0       |                |
ability_time_seconds    | tinyint(11) unsigned  | NO   |     | 0       |                |
ability_number          | tinyint(11) unsigned  | NO   |     | 0       |                |
ability_time_minutes    | tinyint(11) unsigned  | NO   |     | 0       |                |
ability_time_hours      | tinyint(11) unsigned  | NO   |     | 0       |                |
exp                     | int(11) unsigned      | NO   |     | 0       |                |
aa_points_spent         | int(11) unsigned      | NO   |     | 0       |                |
aa_exp                  | int(11) unsigned      | NO   |     | 0       |                |
aa_points               | int(11) unsigned      | NO   |     | 0       |                |
group_leadership_exp    | int(11) unsigned      | NO   |     | 0       |                |
raid_leadership_exp     | int(11) unsigned      | NO   |     | 0       |                |
group_leadership_points | int(11) unsigned      | NO   |     | 0       |                |
raid_leadership_points  | int(11) unsigned      | NO   |     | 0       |                |
points                  | int(11) unsigned      | NO   |     | 0       |                |
cur_hp                  | int(11) unsigned      | NO   |     | 0       |                |
mana                    | int(11) unsigned      | NO   |     | 0       |                |
endurance               | int(11) unsigned      | NO   |     | 0       |                |
intoxication            | int(11) unsigned      | NO   |     | 0       |                |
str                     | int(11) unsigned      | NO   |     | 0       |                |
sta                     | int(11) unsigned      | NO   |     | 0       |                |
cha                     | int(11) unsigned      | NO   |     | 0       |                |
dex                     | int(11) unsigned      | NO   |     | 0       |                |
int                     | int(11) unsigned      | NO   |     | 0       |                |
agi                     | int(11) unsigned      | NO   |     | 0       |                |
wis                     | int(11) unsigned      | NO   |     | 0       |                |
zone_change_count       | int(11) unsigned      | NO   |     | 0       |                |
toxicity                | int(11) unsigned      | NO   |     | 0       |                |
hunger_level            | int(11) unsigned      | NO   |     | 0       |                |
thirst_level            | int(11) unsigned      | NO   |     | 0       |                |
ability_up              | int(11) unsigned      | NO   |     | 0       |                |
ldon_points_guk         | int(11) unsigned      | NO   |     | 0       |                |
ldon_points_mir         | int(11) unsigned      | NO   |     | 0       |                |
ldon_points_mmc         | int(11) unsigned      | NO   |     | 0       |                |
ldon_points_ruj         | int(11) unsigned      | NO   |     | 0       |                |
ldon_points_tak         | int(11) unsigned      | NO   |     | 0       |                |
ldon_points_available   | int(11) unsigned      | NO   |     | 0       |                |
tribute_time_remaining  | int(11) unsigned      | NO   |     | 0       |                |
career_tribute_points   | int(11) unsigned      | NO   |     | 0       |                |
tribute_points          | int(11) unsigned      | NO   |     | 0       |                |
tribute_active          | int(11) unsigned      | NO   |     | 0       |                |
pvp_status              | tinyint(11) unsigned  | NO   |     | 0       |                |
pvp_kills               | int(11) unsigned      | NO   |     | 0       |                |
pvp_deaths              | int(11) unsigned      | NO   |     | 0       |                |
pvp_current_points      | int(11) unsigned      | NO   |     | 0       |                |
pvp_career_points       | int(11) unsigned      | NO   |     | 0       |                |
pvp_best_kill_streak    | int(11) unsigned      | NO   |     | 0       |                |
pvp_worst_death_streak  | int(11) unsigned      | NO   |     | 0       |                |
pvp_current_kill_streak | int(11) unsigned      | NO   |     | 0       |                |
pvp2                    | int(11) unsigned      | NO   |     | 0       |                |
pvp_type                | int(11) unsigned      | NO   |     | 0       |                |
show_helm               | int(11) unsigned      | NO   |     | 0       |                |
group_auto_consent      | tinyint(11) unsigned  | NO   |     | 0       |                |
raid_auto_consent       | tinyint(11) unsigned  | NO   |     | 0       |                |
guild_auto_consent      | tinyint(11) unsigned  | NO   |     | 0       |                |
leadership_exp_on       | tinyint(11) unsigned  | NO   |     | 0       |                |
RestTimer               | int(11) unsigned      | NO   |     | 0       |                |
air_remaining           | int(11) unsigned      | NO   |     | 0       |                |
autosplit_enabled       | int(11) unsigned      | NO   |     | 0       |                |
lfp                     | tinyint(1) unsigned   | NO   |     | 0       |                |
lfg                     | tinyint(1) unsigned   | NO   |     | 0       |                |
mailkey                 | char(16)              | NO   |     |         |                |
xtargets                | tinyint(3) unsigned   | NO   |     | 5       |                |
firstlogon              | tinyint(3)            | NO   |     | 0       |                |
e_aa_effects            | int(11) unsigned      | NO   |     | 0       |                |
e_percent_to_aa         | int(11) unsigned      | NO   |     | 0       |                |
e_expended_aa_spent     | int(11) unsigned      | NO   |     | 0       |                |
aa_points_spent_old     | int(11) unsigned      | NO   |     | 0       |                |
aa_points_old           | int(11) unsigned      | NO   |     | 0       |                |
e_last_invsnapshot      | int(11) unsigned      | NO   |     | 0       |                |