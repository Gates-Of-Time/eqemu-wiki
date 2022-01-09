#ProTip: hit ctrl + f (Windows) or ⌘ + f (Mac) to FIND something on this page

## List of Quest API Functions ##

*  A full list can always be found in the EQEmu source [https://github.com/EQEmu/Server/blob/master/zone/questmgr.cpp](https://github.com/EQEmu/Server/blob/master/zone/questmgr.cpp)

*  Where multiple data types are indicated, please reference the function description below for a full explanation.

**Function** | **Data Type**
------ | ---
[quest::AssignGroupToInstance(instance_id)](#AssignGroupToInstance) | _uint16_
[quest::AssignRaidToInstance(instance_id)](#AssignRaidToInstance) | _uint16_
[quest::AssignToInstance(instance_id)](#AssignToInstance) | _uint16_
[quest::AssignToInstanceByCharID(instance_id, char_id)](#AssignToInstanceByCharID) | _multiple_
[quest::ChooseRandom(option1, option2, option3, option4...[no limit])](#ChooseRandom) | _multiple_
[quest::CreateInstance(zone_name, version, duration)](#CreateInstance) | _multiple_
[quest::DestroyInstance(id)](#DestroyInstance) | _int_
[quest::FlagInstanceByGroupLeader(zone, version)](#FlagInstanceByGroupLeader) | _multiple_
[quest::FlagInstanceByRaidLeader(zone, version)](#FlagInstanceByRaidLeader) | _multiple_
[quest::FlyMode(mode)](#FlyMode) | _uint8_
[quest::GetCharactersInInstance(instance_id)](#GetCharactersInInstance) | _uint16_
[quest::GetInstanceID(zone_name, version)](#GetInstanceID) | _multiple_
[quest::GetInstanceIDByCharID(zone, version, char_id)](#GetInstanceIDByCharID) | _multiple_
[quest::GetInstanceTimer()](#GetInstanceTimer) | _none_
[quest::GetInstanceTimerByID(instance_id)](#GetInstanceTimerByID) | _uint16_
[quest::GetSpellResistType(spell_id)](#GetSpellResistType) | _uint32_
[quest::GetSpellTargetType(spell_id)](#GetSpellTargetType) | _uint32_
[quest::GetTimeSeconds()](#GetTimeSeconds) | _none_
[quest::GetZoneID(zone)](#GetZoneID) | _string_
[quest::GetZoneLongName(zone)](#GetZoneLongName) | _string_
[quest::IsBeneficialSpell(spell_id)](#IsBeneficialSpell) | _uint32_
[quest::IsEffectInSpell(spell_id, effect_id)](#IsEffectInSpell) | _multiple_
[quest::IsRunning()](#IsRunning) | _none_
[quest::LearnRecipe(recipe_id)](#LearnRecipe) | _int_
[quest::MerchantCountItem(npc_id, item_id)](#MerchantCountItem) | _uint32_
[quest::MerchantSetItem(npc_id, item_id, quantity)](#MerchantSetItem) | _uint32_
[quest::ModifyNPCStat(key, value)](#ModifyNPCStat) | _string_
[quest::MovePCInstance(zone_id, instance_id, x, y, z, heading)](#MovePCInstance) | _multiple_
[quest::RemoveAllFromInstance(instance_id)](#RemoveAllFromInstance) | _uint16_
[quest::RemoveFromInstance(instance_id)](#RemoveFromInstance) | _uint16_
[quest::RemoveFromInstanceByCharID(instance_id, char_id)](#RemoveFromInstancByCharID) | _multiple_
[quest::SendMail(to, from, subject, message)](#SendMail) | _string_
[quest::SetRunning(is_running)](#SetRunning) | _bool_
[quest::UpdateInstanceTimer(instance_id, duration)](#UpdateInstanceTimer) | _multiple_
[quest::UpdateSpawnTimer(spawn2_id, updated_time_till_repop)](#UpdateSpawnTimer) | _uint32_
[quest::UpdateZoneHeader(key, value)](#UpdateZoneHeader) | _string_
[quest::activespeakactivity(task_id)](#activespeakactivity) | _int_
[quest::activespeaktask()](#activespeaktask) | _none_
[quest::activetasksinset(task_set)](#activetasksinset) | _int_
[quest::addldonloss(losses, theme_id)](#addldonloss) | _int_
[quest::addldonpoints(points, theme_id)](#addldonpoints) | _int_
[quest::addldonwin(wins, theme_id)](#addldonwin) | _int_
[quest::addloot(item_id, charges, equip_item)](#addloot) | _multiple_
[quest::addskill(skill_id, value)](#addskill) | _int_
[quest::assigntask(task_id, enforce_level_requirement)](#assigntask) | _multiple_
[quest::attack(client_name)](#attack) | _string_
[quest::attacknpc(npc_entity_id)](#attacknpc) | _int_
[quest::attacknpctype(npc_type_id)](#attacknpctype) | _int_
[quest::buryplayercorpse(character_id)](#buryplayercorpse) | _int_
[quest::castspell(spell_id, target_id)](#castspell) | _int_
[quest::changedeity(deity_id)](#changedeity) | _int_
[quest::checktitle(title_set_id)](#checktitle) | _int_
[quest::clear_npctype_cache(npc_type_id)](#clear_npctype_cache) | _int_
[quest::clear_proximity()](#clear_proximity) | _none_
[quest::clear_zone_flag(zone_id)](#clear_zone_flag) | _uint32_
[quest::clearspawntimers()](#clearspawntimers) | _none_
[quest::collectitems(item_id, remove_item)](#collectitems) | _multiple_
[quest::completedtasksinset(task_set)](#completedtasksinset) | _int_
[quest::createBot(first_name, last_name, level, race_id, class_id, gender_id)](#createBot) | _multiple_
[quest::createdoor(model_name, x, y, z, heading, object_type, size)](#createdoor) | _multiple_
[quest::creategroundobject(item_id, x, y, z, heading, decay_time)](#creategroundobject) | _multiple_
[quest::creategroundobjectfrommodel(model_name, x, y, z, heading, object_type, decay_time)](#creategroundobjectfrommodel) | _multiple_
[quest::createguild(guild_name, leader_name)](#createguild) | _string_
[quest::crosszonemessageplayerbyname(channel_id, name, message)](#crosszonemessageplayerbyname) | _multiple_
[quest::crosszonesetentityvariablebyclientname(client_name, key, value)](#crosszonesetentityvariablebyclientname) | _string_
[quest::crosszonesetentityvariablebynpctypeid(npc_type_id, key, value)](#crosszonesetentityvariablebynpctypeid) | _multiple_
[quest::crosszonesignalclientbycharid(character_id, value)](#crosszonesignalclientbycharid) | _int_
[quest::crosszonesignalclientbycharid(character_id, value)](#crosszonesignalclientbycharid) | _int_
[quest::crosszonesignalclientbycharid(name, value)](#crosszonesignalclientbycharid) | _multiple_
[quest::crosszonesignalclientbycharid(name, value)](#crosszonesignalclientbycharid) | _multiple_
[quest::crosszonesignalnpcbynpctypeid(npc_type_id, value)](#crosszonesignalnpcbynpctypeid) | _uint32_
[quest::debug(message, debug_level)](#debug) | _multiple_
[quest::delglobal(key)](#delglobal) | _string_
[quest::depop(npc_type_id)](#depop) | _int_
[quest::depop_withtimer(npc_type_id)](#depop_withtimer) | _int_
[quest::depopall(npc_type_id)](#depopall) | _int_
[quest::depopzone(start_spawn_status)](#depopzone) | _bool_
[quest::ding()](#ding) | _none_
[quest::disable_proximity_say()](#disable_proximity_say) | _none_
[quest::disable_spawn2(spawn2_id)](#disable_spawn2) | _int_
[quest::disablerecipe(recipe_id)](#disablerecipe) | _int_
[quest::disabletask(task_id)](#disabletask) | _int_
[quest::doanim(animation_id)](#doanim) | _int_
[quest::echo(emote_color_id, message)](#echo) | _multiple_
[quest::emote(message)](#emote) | _string_
[quest::enable_proximity_say()](#enable_proximity_say) | _none_
[quest::enable_spawn2(spawn2_id)](#enable_spawn2) | _int_
[quest::enabledtaskcount(task_set)](#enabledtaskcount) | _int_
[quest::enablerecipe(recipe_id)](#enablerecipe) | _int_
[quest::enabletask(task_id)](#enabletask) | _int_
[quest::enabletitle(title_set_id)](#enabletitle) | _int_
[quest::exp(amount)](#exp) | _int_
[quest::faction(faction_id, value, temp)](#faction) | _int_
[quest::factionvalue()](#factionvalue) | _none_
[quest::failtask(task_id)](#failtask) | _int_
[quest::firsttaskinset(task_set)](#firsttaskinset) | _int_
[quest::follow(entity_id, distance)](#follow) | _int_
[quest::forcedoorclose(door_id, alt_mode)](#forcedoorclose) | _multiple_
[quest::forcedooropen(door_id, alt_mode)](#forcedooropen) | _int_
[quest::get_rule(rule_name)](#get_rule) | _string_
[quest::get_spawn_condition(zone_short, instance_id, condition_id)](#get_spawn_condition) | _multiple_
[quest::getguildnamebyid(guild_id)](#getguildnamebyid) | _uint32_
[quest::getlevel(type)](#getlevel) | _int_
[quest::getplayerburiedcorpsecount(character_id)](#getplayerburiedcorpsecount) | _int_
[quest::gettaskactivitydonecount(task_id, activity_id)](#gettaskactivitydonecount) | _int_
[quest::givecash(copper, silver, gold, platinum)](#givecash) | _int_
[quest::gmmove(x, y, z)](#gmmove) | _float_
[quest::gmsay(message, color_id, send_to_world)](#gmsay) | _multiple_
[quest::has_zone_flag(zone_id)](#has_zone_flag) | _uint32_
[quest::incstat(stat_id, value)](#incstat) | _int_
[quest::isdisctome(item_id)](#isdisctome) | _int_
[quest::isdooropen(door_id)](#isdooropen) | _int_
[quest::istaskaappropriate(task_id)](#istaskaappropriate) | _int_
[quest::istaskactive(task_id)](#istaskactive) | _int_
[quest::istaskactivityactive(task_id, activity_id)](#istaskactivityactive) | _int_
[quest::istaskcompleted(task_id)](#istaskcompleted) | _int_
[quest::istaskenabled(task_id)](#istaskenabled) | _int_
[quest::itemlink(item_id)](#itemlink) | _int_
[quest::lasttaskinset(task_set)](#lasttaskinset) | _int_
[quest::level(new_level)](#level) | _int_
[quest::me(message)](#me) | _string_
[quest::movegrp(zone_id, x, y, z)](#movegrp) | _multiple_
[quest::movepc(zone_id, x, y, z [float heading])](#movepc) | _multiple_
[quest::moveto(x, y, z, heading, save_guard_location)](#moveto) | _multiple_
[quest::nexttaskinset(task_set, task_id)](#nexttaskinset) | _int_
[quest::npcfeature(feature, value)](#npcfeature) | _multiple_
[quest::npcgender(gender_id)](#npcgender) | _int_
[quest::npcrace(race_id)](#npcrace) | _int_
[quest::npcsize(size)](#npcsize) | _int_
[quest::npctexture(texture_id)](#npctexture) | _int_
[quest::pause(duration-ms)](#pause) | _int_
[quest::permaclass(class_id)](#permaclass) | _int_
[quest::permagender(gender_id)](#permagender) | _int_
[quest::permarace(race_id)](#permarace) | _int_
[quest::playerfeature(feature, setting)](#playerfeature) | _multiple_
[quest::playergender(gender_id)](#playergender) | _int_
[quest::playerrace(race_id)](#playerrace) | _int_
[quest::playersize(newsize)](#playersize) | _int_
[quest::playertexture(texture_id)](#playertexture) | _int_
[quest::popup(window_title, message, popup_id, buttons, duration)](#popup) | _multiple_
[quest::pvp(mode)](#pvp) | _string_
[quest::qs_player_event(character_id, message)](#qs_player_event) | _multiple_
[quest::qs_send_query(query)](#qs_send_query) | _string_
[quest::rain(weather)](#rain) | _int_
[quest::rebind(zone_id, x, y, z)](#rebind) | _multiple_
[quest::removetitle(title_set_id)](#removetitle) | _int_
[quest::repopzone()](#repopzone) | _none_
[quest::resettaskactivity(task_id, activity_id)](#resettaskactivity) | _int_
[quest::respawn(npc_type_id, grid_id)](#respawn) | _int_
[quest::resume()](#resume) | _none_
[quest::safemove()](#safemove) | _none_
[quest::save()](#save) | _none_
[quest::say(message, language_id)](#say) | _multiple_
[quest::saylink(message, silent, link_name)](#saylink) | _multiple_
[quest::scribespells(max_level, min_level)](#scribespells) | _int_
[quest::selfcast(spell_id)](#selfcast) | _int_
[quest::set_proximity(min_x, max_x, min_y, max_y, min_z, max_z, say)](#set_proximity) | _multiple_
[quest::set_zone_flag(zone_id)](#set_zone_flag) | _uint32_
[quest::setallskill(value)](#setallskill) | _int_
[quest::setanim(npc_type_id, appearance_number)](#setanim) | _int_
[quest::setglobal(key, value, options, duration)](#setglobal) | _multiple_
[quest::setguild(guild_id, guild_rank_id)](#setguild) | _int_
[quest::sethp(mob_health_percentage)](#sethp) | _int_
[quest::setlanguage(skill_id, value)](#setlanguage) | _int_
[quest::setnexthpevent(at_mob_percentage)](#setnexthpevent) | _int_
[quest::setnextinchpevent(at_mob_percentage)](#setnextinchpevent) | _int_
[quest::set_rule(rule_name, rule_value)](#set_rule) | _multiple_
[quest::setskill(skill_id, value)](#setskill) | _int_
[quest::setsky(sky)](#setsky) | _uint8_
[quest::setstat(stat_id, int_value)](#setstat) | _int_
[quest::settarget(target_enum, target_id)](#settarget) | _multiple_
[quest::settime(new_hour, new_min, update_world)](#settime) | _multiple_
[quest::settimer(timer_name, seconds)](#settimer) | _multiple_
[quest::settimerMS(timer_name, milliseconds)](#settimerMS) | _multiple_
[quest::sfollow()](#sfollow) | _none_
[quest::shout(message)](#shout) | _string_
[quest::shout2(message)](#shout2) | _string_
[quest::showgrid(grid_id)](#showgrid) | _int_
[quest::signal(npc_id, wait_ms)](#signal) | _int_
[quest::signalwith(npc_id, signal_id, wait_ms)](#signalwith) | _int_
[quest::snow(weather)](#snow) | _int_
[quest::spawn(npc_type_id, grid_id, int_unused, x, y, z)](#spawn) | _multiple_
[quest::spawn2(npc_type_id, grid_id, int_unused, x, y, z, heading)](#spawn2) | _multiple_
[quest::spawn_condition(zone_short, instance_id, condition_id, value)](#spawn_condition) | _multiple_
[quest::spawn_from_spawn2(spawn2_id)](#spawn_from_spawn2) | _int_
[quest::start(waypoint)](#start) | _int_
[quest::stop()](#stop) | _none_
[quest::stopalltimers()](#stopalltimers) | _none_
[quest::stoptimer(timer_name)](#stoptimer) | _string_
[quest::summonallplayercorpses(char_id, dest_x, dest_y, dest_z, dest_heading)](#summonallplayercorpses) | _multiple_
[quest::summonburiedplayercorpse(char_id, dest_x, dest_y, dest_z, dest_heading)](#summonburiedplayercorpse) | _multiple_
[quest::summonitem(item_id, charges)](#summonitem) | _multiple_
[quest::surname(name)](#surname) | _string_
[quest::targlobal(key, value, duration, npc_id, chararacter_id, zone_id)](#targlobal) | _multiple_
[quest::task_setselector(task_set_id)](#task_setselector) | _int_
[quest::taskexplorearea(explore_id)](#taskexplorearea) | _int_
[quest::taskselector(task_id)](#taskselector) | _int_
[quest::tasktimeleft(task_id)](#tasktimeleft) | _int_
[quest::toggle_spawn_event(event_id, is_enabled, is_strict, reset_base)](#toggle_spawn_event) | _multiple_
[quest::toggledoorstate(door_id)](#toggledoorstate) | _int_
[quest::traindisc(tome_item_id)](#traindisc) | _int_
[quest::traindiscs(max_level, min_level)](#traindiscs) | _int_
[quest::unique_spawn(npc_type_id,grid_id, int_unused, x, y, z, heading)](#unique_spawn) | _multiple_
[quest::unscribespells()](#unscribespells) | _none_
[quest::untraindiscs()](#untraindiscs) | _none_
[quest::updatetaskactivity(task_id, activity_id, count, ignore_quest_update)](#updatetaskactivity) | _multiple_
[quest::varlink(item_id)](#varlink) | _uint32_
[quest::voicetell(client_name, macro_id, race_id, gender_id)](#voicetell) | _multiple_
[quest::we(emote_color_id, message)](#we) | _multiple_
[quest::wearchange(slot, texture_id, hero_forge_model_id, elite_material_id)](#wearchange) | _multiple_
[quest::worldwidemarquee(color_id, priority, fade_in, fade_out, duration, message)](#worldwidemarquee) | _multiple_
[quest::write(file_name, message)](#write) | _string_
[quest::ze(emote_color_id, message)](#ze) | _multiple_
[quest::zone(zone_name)](#zone) | _string_

## Functions

### AssignGroupToInstance

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parmeter:** 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; instance_id _(uint16)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:** 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Assigns a group to an instance. 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Create a scalar variable to store instance_id--GetInstanceID returns int
my $Instance = quest::GetInstanceID($zonesn, $instanceversion); 
quest::AssignGroupToInstance($Instance);
```

### AssignRaidToInstance 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parmeter:** 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; instance_id _(uint16)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Assigns a raid to an instance.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Create a scalar variable to store instance_id
my $Instance = quest::GetInstanceID($zonesn, $instanceversion); #:: GetInstanceID returns int
quest::AssignRaidToInstance($Instance);
```

### AssignToInstance

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; instance_id _(uint16)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Assigns a single player to an instance.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example**

```perl
#:: Create a scalar variable to store instance_id
my $Instance = quest::GetInstanceID($zonesn, $instanceversion); #:: GetInstanceID returns int
quest::AssignToInstance($Instance);
```

### AssignToInstanceByCharID

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; instance_id _(uint16)_, char_id _(uint32)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Assigns a single player to an instance by character ID.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example**

```perl
#:: Create a scalar variable to store instance_id
my $Instance = quest::GetInstanceIDByCharID($zonesn, $instanceversion, $charid); #:: Returns int
quest::AssignToInstanceByCharID($Instance, $charid);
```

### ChooseRandom

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; option1, option2, option3... 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns one of the items listed in its arguments randomly.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Choose a random reward: 1001 - Cloth Cap, 1004 - Cloth Shirt, 1011 - Cloth Pants
quest::summonitem(quest::ChooseRandom(1001, 1004, 1011);
```

### CreateInstance 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; zone_name _(string)_, version _(uint16)_, duration _(uint32)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Creates an instance in the given zone using specified version and duration.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
quest::CreateInstance("mirb", 50, 10800);
```

### DestroyInstance 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; instance_id _(uint16)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Destroys the given instance. 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
quest::DestroyInstance(50);
```

### FlagInstanceByGroupLeader

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; zone _(uint32)_, version _(uint16)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Assigns the group leader's instance to a player 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Zone 237 (mirb), instance 50
quest::FlagInstanceByGroupLeader(237,50);
```

### FlagInstanceByRaidLeader

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; zone _(uint32)_, version _(uint16)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Assigns the raid leader's instance to a player

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Zone 237 (mirb), instance 50
quest::FlagInstanceByRaidLeader(237,50);
```

### FlyMode

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; mode [0-3] _(uint8)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:** 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sets flymode for player where 0 = Off, 1 = On, 2 = Levitate. 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
 #:: Turn fly mode on
quest::FlyMode(1);
```

### GetCharactersInInstance

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; instance_id _(uint16)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:** 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns a hash of character id and instance id

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Instance ID 50
quest::GetCharactersInInstance(50); #:: Returns 50,123456
```

### GetInstanceID

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; zone_name _(string)_, version _(uint16)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:** 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns the instance id of the given zone/verison.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example**

```perl
#:: Create a scalar variable to store instance_id
my $Instance = quest::GetInstanceID($zonesn, $instanceversion); #:: Returns uint16
quest::AssignToInstance($Instance);
```

### GetInstanceIDByCharID

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; zone_name _(string)_, version _(int16)_, char_id _(uint32)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:** 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns the instance ID of the given zone and version by character ID.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example**

```perl
#:: Create a scalar variable to store instance_id
my $Instance = quest::GetInstanceIDByCharID($zonesn, $instanceversion, $charid); #:: Returns uint16
quest::AssignToInstance($Instance);
```


### GetInstanceTimer

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; None.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns the timer for the instance.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example**

```perl
quest::GetInstanceTimer(); #:: Returns uint32
```

### GetInstanceTimerByID

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; instance_id _(uint16)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns the duration timer of the specified instance.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Note: If you do not provide an instance_id in the method it defaults to instance id 0 and returns 0 for time remaining.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example**

```perl
#:: Create a scalar variable to store instance_id
my $Instance = quest::GetInstanceID($zonesn, $instanceversion); #:: Returns uint16
quest::GetInstanceTimerByID($Instance); #:: Returns timer int
```

### GetSpellResistType

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; spell_id _(uint32)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns the [Resist Type](https://github.com/EQEmu/Server/wiki/Resist-Types) of the specified spell.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example**

```perl
quest::GetSpellResistType($spell_id); #:: Returns int
```

### GetSpellTargetType

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; spell_id _(uint32)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns the [Target Type](https://github.com/EQEmu/Server/wiki/Target-Types) of the specified spell.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example**

```perl
quest::GetSpellTargetType($spell_id); #:: Returns int
```

### GetTimeSeconds

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; None.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns unix time in seconds.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
quest::GetTimeSeconds(); #:: Returns int
```

### GetZoneID

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; zone _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns the zone id.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
quest::GetZoneID($zonesn); #:: Returns int
```

### GetZoneLongName

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; zone _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns the long name of the zone.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
quest::GetZoneLongName($zonesn); #:: Returns string
```

### IsBeneficialSpell

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; spell_id _(uint32)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns true if the specified spell is beneficial.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
quest::IsBeneficialSpell($spell_id); #:: Returns 0 or 1
```

### IsEffectInSpell

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; spell_id _(uint32)_, effect_id _(uint32)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns true if the specified spell has the specified [Spell Effect](https://github.com/EQEmu/Server/wiki/Spell-Effect-IDs).

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Check for Spell Effect 23 - Fear
quest::IsEffectInSpell($spell_id, 23); #:: Returns 0 or 1
```

### IsRunning

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; None.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns the running state--0 is walking, 1 is running.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
quest::IsRunning(); #:: Returns 0 or 1
```

### LearnRecipe

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; recipe_id _(uint32)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Makes the client learn a recipe.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Teach recipe_id 2141 - Pickled Bixie
quest::LearnRecipe(2141);
```

### MerchantCountItem

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; npc_id _(uint32)_, item_id _(uint32)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns the number of the specified item in stock at the specified merchant.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Find out how many 12260 - Fuzzlecutter Formula 5000 are in stock at Ping_Fuzzlecutter (9133)
quest::MerchantCountItem(9133, 12260); #:: Returns int
```

### MerchantSetItem

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; npc_id _(uint32)_, item_id _(uint32)_, quantity _(uint32)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Changes the number of the specified items in stock, at the specified quantity, at the specified merchant.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Make sure there is plenty of 12260 - Fuzzlecutter Formula 5000 in stock at Ping_Fuzzlecutter (9133)
quest::MerchantSetItem(9133, 12260, 1000); #:: Quantity 1000
```

### ModifyNPCStat

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; key _(string)_, value _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Changes the specified [npc_types](https://github.com/EQEmu/Server/wiki/npc_types) stat of the specified NPC on the fly--changes are not saved to the npc_types in the DB.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Adjust the runspeed to 1.25
quest::modifynpcstat("runspeed", 1.25);
```

### MovePCInstance

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; zone_id _(uint32)_, instance_id _(uint32)_, x _(float)_, y _(float)_, z _(float)_, heading _(float)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Moves a player to the specified instance of the specified zone at the specified location and heading.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_CLICKDOOR {
    #:: Match door id 3: Frozen Nightmare (mirb) zone in
    if ($doorid == 3) {
        #:: Create a scalar variable to store instance_id--GetInstanceID returns int
        my $InstanceMirB = quest::GetInstanceID("mirb",50);
        #:: Match if an instance exists
        if ($InstanceMirB > 0) {
            #:: Move the player to mirb (237), to their instance, at X - 607, Y - 1503, Z - 33, Heading - 0 (north)
            quest::MovePCInstance(237,$InstanceMirB,607,1503,33,0);
        }
    }
}
```

### RemoveAllFromInstance

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; instance_id _(uint16)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Removes ALL players from an instance by instance ID.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_DEATH_COMPLETE {
     #:: Instance ID is a pre-exported variable
     quest::RemoveAllFromInstance($instanceid);
}
```

### RemoveFromInstance

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; instance_id _(uint16)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Removes the player that triggered the event from an instance by instance ID.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_CLICKDOOR {
     if ($doorid == 1) {
          quest::RemoveFromInstance($instanceid);
     }
}
```

### RemoveFromInstanceByCharID

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; instance_id _(uint16)_, char_id _(uint32)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Removes a client from an instance by character ID.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Create a scalar variable to store instance_id
my $Instance = quest::GetInstanceIDByCharID($zonesn, $instanceversion, $charid); #:: Returns int
quest::RemoveFromInstanceByCharID($Instance, $charid);
```

### SendMail

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; to _(string)_, from _(string)_, subject _(string)_, message _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to send a mail message.

### SetRunning

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; is_running _(bool)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to toggle run/walk state.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SPAWN {
	#:: Set the NPC to run
	quest::SetRunning(1);
}
```

### UpdateInstanceTimer

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; instance_id _(int16)_, duration _(uint32)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to update a zone instance timer by instance id by the number of seconds specified.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_CLICKDOOR {
     #:: When they open door 7...
     if ($doorid == 7) {
          #:: Add one hour of time to the current instance
          quest::UpdateInstanceTimer($instanceid,3600);
     }
}
```

### UpdateSpawnTimer

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; spawn2_id _(uint32)_, updated_time_till_repop _(uint32)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to update a spawn timer by spawn2 ID and time specified in ms.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_DEATH_COMPLETE {
     #:: Set a random timer on Fippy Darkpaw's spawn point
     quest::updatespawntimer(10875,(int(rand(600))+3600)*1000);
}
```

### UpdateZoneHeader

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; key _(string)_, value _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Allows you to manipulate zone header settings on the fly.  The [Quest Manager](https://github.com/EQEmu/Server/blob/c08993b60b7b5328398459a458648a114c3fb331/zone/questmgr.cpp#L3149) lists the following possible strings: ztype, fog_red, fog_green, fog_blue, fog_minclip, fog_maxclip, gravity, time_type, rain_chance, rain_duration, snow_chance, snow_duration, sky, safe_x, safe_y, safe_z, max_z, underworld, minclip, maxclip, fog_density, suspendbuffs.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Set the max clip plane to 500 units
quest::UpdateZoneHeader("maxclip", 500);
```

### activespeakactivity

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; task_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns the Activity ID of the lowest numbered active activity to speak with an NPC in the specified task.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; If you have task id 150:  activity 0--kill three rats, activity 1--talk with NPC, activity 2--kill four fire beetles, activity 3--talk with NPC.

```perl
sub EVENT_SAY {
     #:: Match text for hail, case insensitive
     if ($text=~/hail/i) {
          #:: Create a scalar variable to store the current speak activity for task 150
          $speakactivity = quest::activespeakactivity(150); #:: Returns int
          #:: Match if the player is on the first speak activity
          if ($speakactivity == 1) {
               quest::say("I really hate rats.");
          }
          #:: Match if the player is on the second speak activity
          elsif ($speakactivity == 3) {
               quest::say("I really hate fire beetles.");
          }
     }
}
```

### activespeaktask

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; None.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns the Task ID of the lowest numbered task slot if the player who triggered the event has an active task with an active activity to speak to the NPC (returns 0 if not).

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; If you have task id 150:  activity 0--kill three rats, activity 1--talk with NPC, activity 2--kill four fire beetles, activity 3--talk with NPC.

```perl
sub EVENT_SAY {
     #:: Match text for hail, case insensitive
     if ($text=~/hail/i) {
          #:: Create a scalar variable to store the current task that has a speak activity
          $speaktask = quest::activespeaktask(); #:: Returns int
          #:: Match if there's an active task with a speak activity
          if ($speaktask => 1) {
               quest::say("You have a task to speak with me and its ID is $speaktask.");
          }
          #:: Match if there's NO active task with a speak activity
          else {
               quest::say("You do not have any tasks with a speaking activity at this time.");
          }
     }
}
```

### activetasksinset

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; task_set _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns the number of tasks in the given TaskSet that the player has active.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; You have a TaskSet "20", which consists of three tasks--200, 201, 202.

```perl
sub EVENT_SAY {
     #:: Create a scalar variable to store the number of active tasks in TaskSet 20
     $activetaskcount = quest::activetasksinset(20);  #:: returns int
     #:: Match text for hail, case insensitive
     if ($text=~/hail/i) {
          quest::say("You have $activetaskcount tasks remaining.");
     }
}
```

### addldonloss

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; losses _(int)_, theme_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Adds to loss count for LDON adventures by [LDON Theme](https://github.com/EQEmu/Server/wiki/LDON-Themes).

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Add a loss for Rujarkian Hills theme
quest::addldonloss(1,4);
```

### addldonpoints

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; points _(int)_, theme_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Adds to points count for LDON adventures by [LDON Theme](https://github.com/EQEmu/Server/wiki/LDON-Themes).

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Add 100 points for Rujarkian Hills theme
quest::addldonpoints(100,4);
```

### addldonwin

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; wins _(int)_, theme_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Adds to wins count for LDON adventures by [LDON Theme](https://github.com/EQEmu/Server/wiki/LDON-Themes).

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Add a loss for Rujarkian Hills theme
quest::addldonwin(1,4);
```

### addloot

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; item_id _(uint32)_, charges = 0 _(uint16)_, equip_item = true _(bool)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Add an item with a number of charges to an NPC's loot (does not permanently change the loot table or lootdrop entries).  If 'equipitem' is false (0), the item will not be used by (or shown in the hands of) the NPC.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Add a 5013 - Rusty Short Sword to the NPC's loot, but do not equip the item
quest::addloot(5013,0,0);
```

### addskill

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; skill_id _(int)_, value _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sets the player's skill, by [Skill ID](https://github.com/EQEmu/Server/wiki/Skills), to the value specified.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SAY {
     #:: Match text for train, case insensitive
     if ($text=~/train/i) {
          #:: Call the custom subroutine "Train"
          Train();
     }
}

#:: Custom subroutine
sub Train {
     #:: Send a message to the client in yellow (15) text
     $client->Message( 15, "Your experiences across the realm have infused you with increased power and knowledge..." );
     #:: Set all available skills to maximum for race/class at current level
     foreach my $skill (0 .. 77) {
          #:: Continue the foreach loop using the next skill ID if the client cannot use the skill ID
          next unless $client->CanHaveSkill($skill);
          #:: Create a scalar variable to store the maximum skill Value for the Skill ID
          my $maxSkill = $client->MaxSkill($skill, $client->GetClass(), $ulevel);
          #:: Continue the foreach loop using the next Skill ID if the client has a higher skill Value for the Skill ID
          next unless $maxSkill > $client->GetRawSkill($skill);
          #:: Set the Skill ID to the maximum Value that the client is allowed
          $client->SetSkill($skill, $maxSkill);
     }
     #:: Scribe all spells for current level
     quest::scribespells($ulevel);
}
```

### assigntask

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; task_id _(int)_, npcid _(int)_, enforce_level_requirement = false _(bool)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to assign a task to a client, optionally this can include the NPC ID and whether or not to enforce the level requirement specified in the DB.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Assign Task 102
quest::assigntask(102);
#:: Assign Task 103 with level requirement enforced
quest::assigntask(103, 1);
#:: Assign Task 104 and include the NPC ID
$client->AssignTask(104, $npc->GetID());
#:: Assign Task 105, include the NPC ID with level requirement enforced
$client->AssignTask(105, $npc->GetID(), 1);
```

### attack

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; client_name _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to make the NPC attack a client, by name.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SAY {
     #:: Match text for "mother", case insensitive
     if ($text=~/mother/i) {
          quest::say("How dare you talk about my mother!");
          #:: Attack the client that triggered the event
          quest::attack($name);
     }
}
```

### attacknpc

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; npc_entity_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to make the NPC attack another NPC, by Entity ID.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Create a scalar variable to store the Entity ID of a_large_rat
$aggromob = $entity_list->GetMobID(2011);
#:: Get him.
quest::attacknpc($aggromob);
```

### attacknpctype

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; npc_type_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to make the NPC attack another NPC, by NPC Type ID.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Attack a_large_rat
quest::attacknpctype(2011);
```

### buryplayercorpse

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; character_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Buries and depops a single corpse by Character ID.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SAY {
     #:: Create a scalar variable for storing corpse count
     my $CorpseCount = 0;
     #:: Create a scalar variable for storing the Character ID of the Client that triggered the event
     my $charid = $client->CharacterID();
     if ($text=~/hail/i) {
          #:: Send the client a message in yellow (15) text
          $client->Message(15,"I can [bury a corpse] or [destroy a corpse] that you have unburied.");
     }
     if ($text=~/bury a corpse/i) {
          #:: Match if the client character has a corpse (or corpses)
          if ($CorpseCount > 0) {
               #:: Bury the character's corpse
               quest::buryplayercorpse($charid);
               $client->Message(15,"Very well, burying one of your corpses now.");
          }
          #:: Match if the client character does not have a corpse
          else {
               $client->Message(13,"You have no unburied corpses, begone.");
          }
     }
}
```

### castspell

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; spell_id _(int)_, target_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to make the NPC cast a spell, by ID, on a target, by ID.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Cast spell 12 - Healing, on the user that triggered the event
quest::castspell(12,$userid);
```

### changedeity

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; deity_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to permanently change the client character's deity, by [Deity ID](https://github.com/EQEmu/Server/wiki/Deity-List); kicks the client to character select.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Change the client character's deity to 201 - Bertoxxulous
quest::changedeity(201);
```

### checktitle

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; title_set_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to determine if a player has the specified titleset enabled or not.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Check to see if Title Set 2 (prefix "Arbiter", suffix "Harbinger of the Old World") is enabled
quest::checktitle(2); #:: Returns bool
```

### clear_npctype_cache

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; npc_type_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Clears the NPC Table.

### clear_proximity

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; None.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Clears an NPC's defined proximity.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SPAWN {
     #:: Create a proximity, 50 units across
     quest::set_proximity($x - 25, $x + 25, $y - 25, $y + 25);
}

sub EVENT_ENTER {
     #:: Shout a message when the event is triggered
     quest::shout("Congratulations $name, you have won the race!");
     #:: Clear the proximity since second place is the first loser
     quest::clear_proximity();
}
```

### clear_zone_flag

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; zone_id _(uint32)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to clear the Zone Flag, by ID, of a client character.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Clear the character's Zone Flag (Sleeper's Key) for 128 - The Sleeper's Tomb (sleeper)
quest::clear_zone_flag(128);
```

### clearspawntimers

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; None.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to reset the spawn timers and repop a zone--similar to #repop force.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
quest::clearspawntimers();
```

## collectitems

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; item_id _(int)_, remove_item = true _(bool)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns the number of items by ID that exist in inventory. If remove is true, items are removed as they are counted.  

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SAY {
	#:: Match text for "hail", case insensitive, and the client that triggered the event has a 1001 - Cloth Cap
	if ($text=~/hail/i && plugin::check_hasitem($client, 1001)) {
		quest::emote("steals your cloth cap.");
		quest::collectitems(1001, 1);
	}
}
```

## completedtasksinset

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; task_set _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns the number of tasks in the given Task Set that the player has completed.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SAY {
     #:: Match text for "tasks", case insensitive
     if ($text=~/tasks/i) {
          #:: Create a scalar variable to store the count of completed tasks in task set "200"
          my $TasksComplete = quest::completedtasksinset(200); #:: Returns int
          quest::say("You have completed $TasksComplete tasks.");
     }
}
```

## createBot

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; first_name _(string)_, last_name _(string)_, level _(int)_, race_id _(int)_, class_id _(int)_, gender_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to create a bot with the given parameters.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_ENTERZONE {
     #:: Create a bot named Leroy Jenkins, who is level 50, Human, Paladin, Male
     quest::createBot("Leroy", "Jenkins", 50, 1, 3, 0);
}
```

## createdoor

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; model_name _(string)_, x _(float)_, y _(float)_, z _(float)_, heading _(float)_, object_type = 58 _(int)_, size = 100 _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Creates a new door, with type 58 and size 100 as the defaults.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
quest::createdoor("POKTELE500", -582.532, 2324.96, -47.8143, 120, 58, 100);
```

## creategroundobject

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; item_id _(int)_, x _(float)_, y _(float)_, z _(float)_, heading _(float)_, decay_time _(uint32)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Creates an object on the ground with the given parameters, decay time is ms = 300000 by default.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_WAYPOINT_ARRIVE {
     #:: Create a 12274 - Chalice of Conquest at the NPC's current location
     quest::creategroundobject(12274, $x, $y, $z, $h);
}
```

## creategroundobjectfrommodel

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; model_name _(string)_, x _(float)_, y _(float)_, z _(float)_, heading _(float)_, object_type _(int)_, decay_time _(uint32)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Creates an object on the ground with the given parameters, decay time is ms = 300000 by default.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Create a 17330 - Bag of Supplies at the given location
quest::creategroundobjectfrommodel("IT64_ACTORDEF", 2497, -557, -327, 58, 17330);
```

## createguild

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; guild_name _(string)_, leader_name _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Creates a guild.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SAY{
     if (quest::createguild("Akkadius Fire", $client->GetName())) {
          $client->Message(15, "Guild has been created successfully");
     }
     else{
          $client->Message(15, "Guild creation error");
     }
}
```

## crosszonemessageplayerbyname

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; channel_id _(int)_, name _(string)_, message _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sends a message to a client character on the specified channel.  Useful for Expeditions and Shared Tasks.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
quest::crosszonemessageplayerbyname(15, $name, "Hi.");
```

## crosszonesetentityvariablebyclientname

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; client_name _(string)_, key _(string)_, value _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sets entity variables world-wide for the provided client character.

## crosszonesetentityvariablebynpctypeid

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; npc_type_id _(int)_, key _(string)_, value _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sets entity variables world wide with specified npctype_id.

## crosszonesignalclientbycharid

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; character_id _(int)_, value _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Signals the client by character ID world wide.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Signal the client character who triggered the event with "5000"
quest::crosszonesignalclientbycharid($charid,5000);
```

## crosszonesignalnpcbynpctypeid

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; npc_type_id _(uint32)_, value _(uint32)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Signals all NPC entities world-wide with the specified value.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Signal all 4036 - a_giant_rat with "99"
quest::crosszonesignalnpcbynpctypeid(4036, 99);
```

## debug

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; message _(string)_, debug_level _(uint8)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Allows you to export debug information for an event, at the specified level (1 through 3).

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_ENVIRONMENTAL_DAMAGE {
     quest::debug("EVENT_ENVIRONMENTAL_DAMAGE");
     quest::debug("env_damage is " . $env_damage);
     quest::debug("env_damage_type is " . $env_damage_type);
     quest::debug("env_final_damage is " . $env_final_damage);
}
```

## delglobal

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; key _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Deletes a quest global.  Please consider using [Data Buckets](https://github.com/EQEmu/Server/wiki/Data-Buckets) instead of quest globals.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
quest::delglobal("strongbox");
```

## depop

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; npc_type_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Depops an NPC by npc_type_id, default is 0 (self).

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Depop self
quest::depop();
```

## depop_withtimer

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; npc_type_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Depops an NPC by npc_type_id, default is 0 (self), and restarts the spawn point timer.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Depop self and restart spawn timer
quest::depop_withtimer();
```

## depopall

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; npc_type_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Depops all NPC entities with npc_type_id in the zone.  Default is 0 (self and others like me).

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Depop all 4036 - a_giant_rat
quest::depopall(4036);
```

## depopzone

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; start_spawn_status _(bool)_ 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Depops the zone with the specified parameter.  Default is false (don't start spawn timers).

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Depop the zone and don't start the spawn timers
quest::depopzone();
```

## ding

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; None.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Plays the beautiful ding sound, the trumpet fanfare for your glorious deeds.  Congratulations, winner.  You did it.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Ding!
quest::ding();
```

## disable_proximity_say

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; None.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Disables proximity say for the NPC.  Proximity say must be enabled with quest::set_proximity(); and quest::enable_proximity_say();.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
quest::disable_proximity_say();
```

## disable_spawn2

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; spawn2_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Disables the spawn point specified and depops any NPC entity from that spawn point.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Disable the spawn point for 151562 - spawngroup ID 113004 - npcIDs 15138 (Droon) and 15160 (Proon)
quest::disable_spawn2(151562);
```

## disablerecipe

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; recipe_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Disables the recipe specified by Recipe ID.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Disable recipe 1 - Blessed Fishing Rod
quest::disablerecipe(1);
```

## disabletask

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; task_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Disables a task so that it is not available to a client character.  Useful if you do not want someone to repeat a task.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Match if the player has an active task
if ($task != 0) {
     #:: Create a scalar variable to store the active speak-to activity
     $activity = quest::activespeakactivity($task);
     #:: Mark the activity as complete
     quest::updatetaskactivity($task, $activity);
     quest::say("Well done!");
     #:: Offer the next task, if there is one
     if (!quest::istaskactive($task)) {
          #:: Disable the task so that it cannot be repeated
          quest::disabletask($task);
          #:: Match if there are tasks remaining in the Task Set
          if ($task != quest::lasttaskinset(200)) {
               quest::say("Well done, I have another task if you are willing.");
               #:: Enable the next Task in the Task Set
               quest::enabletask(quest::nexttaskinset(200, $task));
          }
          #:: Match if there are no tasks remaining in the task set
          else {
               quest::say("Thank you for cleansing Qeynos Hills!");
          }
     }
}
```

## doanim

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; animation_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Makes the NPC perform the indicated [Animation](https://github.com/EQEmu/Server/wiki/Animations).

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Perform the Cheer animation
quest::doanim(27);
```

quest::echo

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; emote_color_id _(int)_, message _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Echoes the specified message string, in the specified color, to the client console.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Echo a message in yellow text (15)
quest::echo(15,"Hello, world");
```

## emote

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; message _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Makes the NPC emote the specified message string.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_DEATH_COMPLETE {
     quest::emote("'s corpse says 'How...did...ugh...'");
}
```

## enable_proximity_say

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; None.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Enables proximity say for the NPC--the target would not have to have the NPC targeted to interact if the NPC has a defined proximity and proximity say is enabled.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SPAWN {
     #:: Set the proximity bounds around the NPC on spawn, 30 units across
     $x = $npc->GetX();
     $y = $npc->GetY();
     quest::set_proximity($x-15,$x+15,$y-15,$y+15);
     quest::enable_proximity_say();
}

sub EVENT_PROXIMITY_SAY {
     if ($text=~/Ganelorn Oast/i) {
          quest::say("Ganelorn Oast! For he has single-handedly caught more poachers than any other ranger. He is credited for helping numerous endangered species recover from certain extinction. I suppose I am lucky he is fond of my sister, as I am soon to train under him as an apprentice. Perhaps one day I will even [" . quest::saylink("call upon the flames") . "] in the way that he does.");
     }
     elsif ($text=~/call upon the flames/i) {
          quest::say("Aye, Ganelorn is renowned not only for his abilities as an archer and a master of melee combat, but also for his use of powerful magics. Never before have I seen a forester evoke a fireball of such great force. It would be any ranger's dream to become his pupil just to study that one spell. Ganelorn doesn't train just anyone, though. If you want to learn from him, I'm certain you would have to prove yourself as a forester.");
     }
     if ($text=~/I want to learn/i) {
          quest::say("He is a very busy individual. I believe he is currently in the eastern part of the Karanas trying to track down a poacher. Even if you can track him down, don't get your hopes up.");
          #:: Send a signal 2 to The Greater Faydark >> Lily_Ashwood (54086)
          quest::signalwith(54086, 2, 3);
     }
}
```

## enable_spawn2

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; spawn2_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Enables the specified spawn point.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_DEATH_COMPLETE {
     #:: Enable the spawn timer for 151562 - spawngroup ID 113004 - npcIDs 15138 (Droon) and 15160 (Proon)
     quest::enable_spawn2(151562);
}
```

## enabledtaskcount

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; task_set _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Counts the enabled tasks in the specified Task Set.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Match if there are no enabled tasks in Task Set 10
if (quest::enabledtaskcount(10) == 0) {
     quest::enabletask(50, 51, 52);
}
```

## enablerecipe

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; recipe_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Enables the recipe specified by Recipe ID.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Enable recipe 1 - Blessed Fishing Rod
quest::enablerecipe(1);
```

## enabletask

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; task_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Enables a task.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Match if the player has an active task
if ($task != 0) {
     #:: Create a scalar variable to store the active speak-to activity
     $activity = quest::activespeakactivity($task);
     #:: Mark the activity as complete
     quest::updatetaskactivity($task, $activity);
     quest::say("Well done!");
     #:: Offer the next task, if there is one
     if (!quest::istaskactive($task)) {
          #:: Disable the task so that it cannot be repeated
          quest::disabletask($task);
          #:: Match if there are tasks remaining in the Task Set
          if ($task != quest::lasttaskinset(200)) {
               quest::say("Well done, I have another task if you are willing.");
               #:: Enable the next Task in the Task Set
               quest::enabletask(quest::nexttaskinset(200, $task));
          }
          #:: Match if there are no tasks remaining in the task set
          else {
               quest::say("Thank you for cleansing Qeynos Hills!");
          }
     }
}
```

## enabletitle

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; title_set_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Enables the specified Title Set.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_ITEM_CLICK {
     #:: Match if item 98471 - Mastering Tinkering Master I is clicked
     if ($itemid == 98471) {
          #:: Tinkering Mastery AA ID 575 Rank 1
          $client->GrantAlternateAdvancementAbility(575,1,0);
          #:: Send a message in Yellow (15) text
          $client->Message(15,"You have mastered tinkering!");
          #:: Ding!
          quest::ding();
          #:: Enable tinkering mastery title set
          quest::enabletitle(10);
     } 
}
```

## exp

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; amount _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Gives the amount of [experience](https://github.com/EQEmu/Server/wiki/Experience-by-Level) specified to the client character.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Grant 100 experience points
quest::exp(100);
```

## faction

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; faction_id _(int)_, value _(int)_, temp _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Gives the client character the faction, specified by Faction ID, in the amount specified by value.  Temp is optional, and defaults to 0.  Temp values are:  0 (permanent, with a message), 1 (temporary, without a message), 2 (temporary, with a message), or 3 (permanent, without a message).

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Set faction
quest::faction(192,10); 	#:: +10 League of Antonican Bards
quest::faction(184,10); 	#:: +10 Knights of Truth
quest::faction(135,10); 	#:: +10 Guards of Qeynos
quest::faction(273,-30); 	#:: -30 Ring of Scale
```

## factionvalue

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; None.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns faction values for the client character that triggered the event.  Generally the opposite values of $faction, with 1 being "scowls" and 9 being "ally" ($faction considers 1 to be "ally", and 9 "scowls").

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SAY {
     if ($text=~/hail/i) {     
          #:: Create a scalar variable for storing faction
          my $backwardfaction = quest::factionvalue();  #:: Returns int
          quest::say("Your faction is $faction, but your faction is $backwardfaction");  #:: $faction is pre-exported and returns int
     }
}
```

## failtask

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; task_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Fails the task, by Task ID, for the client character that triggered the event.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Fail Task 216
quest::failtask(216);
```

## firsttaskinset

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; task_set _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns the first task in the specified Task Set.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SAY {
     #:: If the player hasn't completed the last task in the Task Set
     if (!quest::istaskcompleted(quest::lasttaskinset(200))) {
          #:: If the player has no tasks enabled for this task set, enable the first one
          if (quest::enabledtaskcount(200) == 0) {
               quest::say("You have not done any of my tasks before!");
               #:: Enable the first task in Task Set 200
               quest::enabletask(quest::firsttaskinset(200));
          }
     }
}
```

## follow

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; entity_id _(int)_, distance _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to make an NPC follow another NPC, specified by Entity ID.  The distance determines how many units the NPC will follow behind the specified NPC, with a default value of 10; distance is optional.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SPAWN {
     #:: Create a timer that triggers every 10 seconds
     quest::settimer("follow",10);
}

sub EVENT_TIMER {
     #:: Match if the timer is named "follow"
     if ($timer eq "follow") {
          #:: Create a scalar variable to store the NPC Type ID for mob 2161
          my $getmobbynpctype = $entity_list->GetMobByNpcTypeID(2161);
          #:: Create a scalar variable to store the Entity ID of the aforementioned NPC
          my $follow_target = $getmobbynpctype->GetID();
          #:: Follow the NPC at a default distance of 10 units
          quest::follow($follow_target);
          #:: Clean up and stop the timer
          quest::stoptimer("follow");
     }
}
```

## forcedoorclose

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; door_id _(int)_, alt_mode _(bool)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Forces a door, by Door ID, to close.  Alt_Mode is default false.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Close Door ID 31 in Befallen
quest::forcedoorclose(31);
```

## forcedooropen

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; door_id _(int)_, alt_mode _(bool)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Forces a door, by Door ID, to open.  Alt_Mode is default false.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Open Door ID 31 in Befallen
quest::forcedooropen(31);
```

## get_rule
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; rule_name _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns the value of the specified [Rule](https://github.com/EQEmu/Server/wiki/Server-Rules) for the zone you're in.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Get the rule value for rule "Zone:UseZoneController"
sub EVENT_SAY {
	if ($text=~/Hail/i) {
		plugin::Whisper(quest::get_rule("Zone:UseZoneController")); #:: Whispers rule value to client.
	}
}
```

## get_spawn_condition

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; zone_short _(string)_, instance_id _(int)_, condition_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns the value of the specified spawn condition.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Get the Spawn Condition for Condition ID 1, in the default instance of Lesser Faydark
quest::get_spawn_condition("lfaydark", 0, 1);  #:: Returns int
```

## getguildnamebyid

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; guild_id _(uint32)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns the name of the Guild for the specified Guild ID.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_CONNECT {
     #:: Announce the name of the client character that triggered the event in GM Say
     quest::gmsay("$name has connected.", 18, 1);
     #:: Announce the Account Name of the client character that triggered the event in GM Say
     quest::gmsay(" Account Name: " . $client->AccountName() . " - Status: $status", 18, 1);
     #:: Match if the client character has a guild
     if ($uguild_id > 0) {
          #:: Create a scalar variable to store the name of the client character's guild
          my $guildname = quest::getguildnamebyid($uguild_id);
          #:: Announce the client character's information in GM Say
          quest::gmsay("(Character Profile: Level $ulevel $race $class) <$guildname>)", 18, 1);
     }
     #:: Match if the client character does not have a guild
     else {
          #:: Announce the client character's information in GM Say
          quest::gmsay("(Character Profile: Level $ulevel $race $class) <No Guild>", 18, 1);
     }
}
```

## getinventoryslotid

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; identifier _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns the Inventory Slot ID for the specified identifier.  Reference [Perl Inventory Slot Identifiers](https://github.com/EQEmu/Server/wiki/Perl-Inventory-Slot-Identifiers) for appropriate identifier tokens.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Create a scalar variable to store an item ID
my $charmitem = $client->GetItemIDAt(quest::getinventoryslotid("charm"));  #:: returns int
```

## getlevel

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; type _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns the level for the Type specified.  Types can be 0 (self), 1 (group average), 2 (raid average), 3 (raid average, group average, or self), or 4 (self level 2--the highest level attained by self).

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Get the level of the client character
quest::getlevel(0);  #:: Returns int
```

## getplayerburiedcorpsecount

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; character_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns the number of corpses for the specified Character ID that are buried.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Get the number of burried corpses for character ID 12345
quest::getplayerburriedcorpsecount(12345); #:: return int
```

## gettaskactivitydonecount

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; task_id _(int)_, activity_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns the task activity done count, by Task ID and Activity ID, for the client entity.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Find out how many times the client character has killed 10 beetles in Unrest
quest::gettaskactivitydonecount(15,3);  #:: Returns int
```

## givecash

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; copper _(int)_, silver _(int)_, gold _(int)_, platinum _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Gives the specified amount of money to the client that triggered the event.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Create a hash for storing cash - 20 to 100cp
my %cash = plugin::RandomCash(20,100);
#:: Grant a random cash reward
quest::givecash($cash{copper},$cash{silver},$cash{gold},$cash{platinum});
```

## gmmove

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; x _(float)_, y _(float)_, z _(float)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Moves the entity to the specified coordinates.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SPAWN {
     #:: Create a timer that loops each second
     quest::settimer("position",1);
}

sub EVENT_TIMER {
     #:: Create a scalar variable to store the X position of the NPC
     my $x = $npc->GetX();
     #:: Create a scalar variable to store the Y position of the NPC
     my $y = $npc->GetY();
     #:: Match if the timer "position" has looped and the X and Y coordinates are outside the specified range
     if ($timer eq "position" && ($x < -353 || $x > -109 || $y < -549 || $y > -310)) {
          quest::shout("No! I must not leave the time chamber! If I do, I'll age and die!");
          #:: Move the NPC back to the chamber
          $npc->GMMove(-231.464005,-432.937469,202.375946,.125);
     }
}

sub EVENT_DEATH_COMPLETE {
     quest::stoptimer("position");
}
```

## gmsay

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; message _(string)_, color_id _(int)_, send_to_world _(bool)_, guild_id _(uint32)_, minstatus _()_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sends a message to the client console if the parameters are met.  [Color](https://github.com/EQEmu/Server/wiki/Emote-Colors), Send to World, Guild ID, and Minimum Status are all optional, but Color defaults to 0 (white), Send to World defaults to 0 (false), and Minimum Status defaults to 80.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Send white text to all players in the current zone with an admin status of >= 80
quest::gmsay("Text");
#:: Send yellow (15) text to all players in the current zone with an admin status of >= 80
quest::gmsay("Text", 15);
#:: Send yellow (15) text to all players with an admin status of >= 80 in all zones
quest::gmsay("Text", 15, 1);
#:: Send yellow (15) text to all players with an admin status of >= 80 in all zones, who are in a guild with a Guild ID of 30
quest::gmsay("Text", 15, 1, 30);
#:: Send yellow (15) text to all players with an admin status of >= 0 in all zones, who are in a guild with a Guild ID of 30
quest::gmsay("Text", 15, 1, 30, 0);
```

## has_zone_flag

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; zone_id _(uint32)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to verify that a client character has the required zone flag for the specified zone.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_CLICKDOOR {
     if ($doorid == 12) {
          if (quest::has_zone_flag(200) != 1) {  #:: Returns bool
               quest::set_zone_flag(200);
          }
     }
}
```

## incstat

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; stat_id _(int)_, value _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Increases the specified stat by double the specified value.  Stat IDs: STR = 0, STA = 1, AGI = 2, DEX = 3, INT = 4, WIS = 5, CHA = 6. Note: if you're increasing stats, the client will have to zone to see the effect.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Increase STR by 20
quest::incstat(0, 10);
``` 

## isdisctome

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; item_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to check if the specified item, by Item ID, is a discipline tome.  You likely have a plugin for this (plugin::try_tome_handins).

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_ITEM {
     quest::traindisc($item1) if (quest::isdisctome($item1));
     quest::traindisc($item2) if (quest::isdisctome($item2));
     quest::traindisc($item3) if (quest::isdisctome($item3));
     quest::traindisc($item4) if (quest::isdisctome($item4));
}
```

## isdooropen

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; door_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Checks to see if the specified door is open.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_CLICKDOOR {
     my $doorcheck = quest::isdooropen(41);  #:: Returns bool
     if ($doorid == 41 && $doorcheck == 0) {
          quest::forcedooropen(41);
     }
}
```

## istaskaappropriate

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; task_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to see if a task is set for the appropriate level for the client character who initiated the event.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Check if task 200 is appropriate
quest::istaskaappropriate(200);  #:: Returns bool
```

## istaskactive

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; task_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to determine if a task is active, by Task ID.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Check if task 212 is active
quest::istaskactive(212); #:: Returns bool
```

## istaskactivityactive

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; task_id _(int)_, activity_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to determine if a task activity is active, by Task ID and Activity ID.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Check if Activity 9 of Task 212 is active 
quest::istaskactivityactive(212, 9); #:: Returns bool
```

## istaskcompleted

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; task_id (int)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to determine if a task is completed, by Task ID.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Check if task 212 is completed
quest::istaskcompleted(212); #:: Returns bool
```

## istaskenabled

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; task_id (int)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to determine if a task is enabled, by Task ID.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Check if task 212 is enabled
quest::istaskenabled(212); #:: Returns bool
```

## itemlink

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; item_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to send a link of the specified item, by Item ID.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Send an item link for a 1001 - Cloth Cap
quest::itemlink(1001);
```

## lasttaskinset

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; task_set _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns the last task in the specified Task Set.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Find the Task ID of the last task in Task Set 200
quest::lasttaskinset(200); #:: Returns int
```

## level

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; new_level _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sets the level to the specified new level for the client character that triggered the event.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SAY {
     if ($text=~/level/i) {
          #:: Match if user's level is 20 or under
          if ($ulevel <= 20) {
               #:: Give the player one more level
               quest::level($ulevel+1);
          }
          elsif ($ulevel >= 21) {
               $npc->CastSpell(808, $userid);
               quest::say("Begone!");
          }
     }
}
```

## me

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; message _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sends an emote without a name.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
quest::me("This creature has no need for your money.");
```

## movegrp

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; zone_id _(int)_, x _(float)_, y _(float)_, z _(float)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Moves the group of the client character that triggered the event to the specified Zone, by Zone ID, to the location specified.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Match text for "we are ready", case insensitive
if ($text=~/We are ready/i) {
     #:: Move the group to The Plane of Nightmares (ponightmare) at X=1194, Y=1121, Z=208
     quest::movegrp(204,1194,1121,280); 
}
```

## movepc

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; zone_id _(int)_, x _(float)_, y _(float)_, z _(float)_, heading _(float)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Moves the client character that triggered the event to the specified zone, by Zone ID, at the specified location.  Heading is optional, but will default to 0 (North).

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Match text for "travel to butcherblock", case insensitive
if ($text=~/travel to butcherblock/i) {
     #:: Move the character to Butcherblock Mountains (butcher), at X=3168.92, Y=851.92, Z=11.66--the Southern dock
     quest::movepc(68,3168.92,851.92,11.66);
}
```

## moveto

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; x _(float)_, y _(float)_, z _(float)_, heading _(float)_, save_guard_location _(bool)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to move the NPC to the specified location.  Heading and Save Guard Location are optional.  Heading will default to 0 (North), and Save Guard Location will also default to 0, causing the NPC to path back.  Set Save Guard Location to 1 to make the NPC stay at the moveto location.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_ITEM {
     #:: Match a 12278 - Abandoned Orc Shovel
     if (plugin::takeItems(12278 => 1)) {
          #:: 0=Stand, 1=Sit, 2=Duck, 3=Feign Death, 4=Kneel
          $npc->SetAppearance(0);
          #:: Move to the specified location and guard 
          quest::moveto(-395.87, 807.04, 70.53, 0, 1);
     }
     #:: Return unused items
     plugin::returnUnusedItems();
}
```

## nexttaskinset

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; task_set _(int)_, task_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns the next task in the specified Task Set that comes after the specified Task ID.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SAY {
     #:: Create a scalar variable to store a task integer
     $task = quest::activespeaktask();
     #:: Match if there is an active task to speak to the NPC
     if ($task != 0) {
          #:: Match if there are no active tasks for the current speaking task
          if (!quest::istaskactive($task)) {
               #:: Disable the current speaking task
               quest::disabletask($task);
               #:: Match if the current speaking task is NOT the last task in the Task Set
               if ($task != quest::lasttaskinset(200)) {
                    quest::say("Well done, I have another task if you are willing.");
                    #:: Enable the next task in Task Set 200
                    quest::enabletask(quest::nexttaskinset(200, $task));
               }
               else {
                    quest::say("Thank you for cleansing Qeynos Hills!");
               }
          }
     }
}
```

## npcfeature
 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; feature _(string)_, value _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Allows you to temporarily change the specified feature on the NPC to the specified value.  Allowable features are:  race, gender, texture, helm, haircolor, beardcolor, eyecolor1, eyecolor2, hair, face, beard, heritage, tatoo, details, and size.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Change the NPC's size to 10
quest::npcfeature("size", 10);
```

## npcgender

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; gender_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to temporarily change the gender of the NPC as specified:  0 = Male, 1 = Female, 2 = Neuter.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Change the NPC's gender to female
quest::npcgender(1);
```

## npcrace

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; race_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to temporarily change an NPC's [Race](https://github.com/EQEmu/Server/wiki/Race-Types).

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Change the NPC's Race to Golem (17)
quest::npcrace(17);
```

## npcsize

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; size _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to temporarily change the NPC's size.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Change the NPC's size to 17
quest::npcsize(17);
```

## npctexture

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; texture_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to temporarily change the NPC's texture.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Change the NPC's texture to 2
quest::npctexture(2);
```

## pause

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; duration-ms _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Forces the NPC to pause for the specified duration in ms.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Pause for 1 second
quest::pause(1000);
```

## permaclass

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; class_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Permanently changes the class of the client character that triggered the event to the specified class, and disconnects them.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Change class to Warrior
quest::permaclass(1);
```

## permagender

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; gender_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Permanently changes the gender of the client character that triggered the event to the specified gender, and disconnects them.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Change gender 0 = Male, 1 = Female, 2 = Neuter.
quest::permagender(0);
```

## permarace

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; race_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Permanently changes the [Race Type](https://github.com/EQEmu/Server/wiki/Race-Types) of the client character that triggered the event to the specified race, and disconnects them.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Change race to Human
quest::permarace(1);
```

## playerfeature

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; feature _(string)_, setting _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Temporarily changes the player feature to the specified setting.  Acceptable strings are:  race, gender, texture, helm, haircolor, beardcolor, eyecolor1, eyecolor2, hair, face, beard, heritage, tattoo, details, or size.  

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Change race to Human
quest::playerfeature("race", 1);
```

## playergender

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; gender_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Temporarily changes the gender of the client character that triggered the event to the specified gender.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Change gender 0 = Male, 1 = Female, 2 = Neuter.
quest::playergender(0);
```

## playerrace

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; race_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Temporarily changes the [Race Type](https://github.com/EQEmu/Server/wiki/Race-Types) of the client character that triggered the event to the specified race.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Change race to Human
quest::playerrace(1);
```

## playersize

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; newsize _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Temporarily adjusts the size of the client character that triggered the event to the specified size.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Change size to 10
quest::playersize(10);
```

## playertexture

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; texture_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Temporarily changes the texture of the client character that triggered the event to the specified texture.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Change texture to 2
quest::playertexture(2);
```

## popup

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; window_title _(string)_, message _(string)_, popup_id _(int)_, buttons _(int)_, duration _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to create a popup window with the specified parameters. The parameters popup_id, buttons, and duration are optional.  Button parameters are:  0=OK button, 1=Yes/No buttons.  Setting duration to 0 results in a popup that will remain until dismissed.  

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_ENTER {
     #:: Popup window entitled "Teleport", Question: "Teleport to The Plane of Hate?", popup ID 666, Yes/No buttons, remain until dismissed
     quest::popup('Teleport', 'Teleport to The Plane of Hate?', 666, 1, 0);
}

sub EVENT_POPUPRESPONSE {
     if ($popupid == 666) {
          #:: Teleport the player to The Plane of Hate
          quest::movepc(186,-393,656,3);
     }
}
```

## pvp

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; mode _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Toggles the PVP setting for the client character that triggered the event.  String can be on, or off.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Turn pvp on
quest::pvp("on");
#:: Turn pvp off
quest::pvp("off");
```

## qs_player_event

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; character_id _(int)_, message _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Adds a record to table `qs_player_events` with the specified parameters.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
quest::qs_player_event($charid,"Triggered an event with this API call in it.")
```

## qs_send_query

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; query _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Send a raw query to the QueryServ process.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
quest::qs_send_query("SELECT * FROM `qs_player_events` WHERE `event_desc` LIKE '%level%' LIMIT 0,1000;");
```

## rain

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; weather _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Changes the rainy weather to the specified setting:  0=none, 1=rain.  See also quest::snow().

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_ZONE {
     if ($name=~/turmoiltoad/i) {
          #:: Turn on the rain for those left behind
          quest::rain(1);
     }
}
```

## rebind

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; zone_id _(int)_, x _(float)_, y _(float)_, z _(float)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Binds the client character that triggered the event to the specified zone (by Zone ID) at the specified location.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Change bind point to Rivervale, X=0, Y=0, Z=3.13
quest::rebind(19, 0.00, 0.00, 3.13);
```

## removetitle

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; title_set_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Removes the specified Title Set from the client character that triggered the event.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Remove Title Set 2 (prefix "Arbiter", suffix "Harbinger of the Old World")
quest::removetitle(2);
```

## repopzone

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; None.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Repops the zone and re-enables spawn timers.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Repop the zone
quest::repopzone();
```

## resettaskactivity

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; task_id _(int)_, activity_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sets the done count to 0 for the specified Task ID

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Reset the activity done count for task 202
quest::resettaskactivity(202);
```

## respawn

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  npc_type_id _(int)_, grid_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Respawns the specified NPC by npc_type ID on the specified grid.  This is similar to quest::spawn2(), but without the specified x, y, z, heading parameters.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Spawn Fippy Darkpaw again
quest::respawn(2001);
```

## resume

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; None.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to resume pathing on a grid that has been stopped.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Resume pathing on grid
quest::resume();
```

## safemove

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; None.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Moves the client character that triggered the event to the safe coordinates of the current zone.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Move to safe
quest::safemove();
```

## save

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; None.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Saves the character data for the client character that triggered the event.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Save Save Save
quest::save();
```

## say

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; message _(string)_, language_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to make your NPC speak.  [Language](https://github.com/EQEmu/Server/wiki/Languages) ID is optional--if not specified, the NPC will speak in common tongue.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
quest::say("Hello.");
#:: Now in Barbarian
quest::say("Hello.", 1);
```

## saylink

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; message _(string)_, silent _(bool)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to create a say link.  The silent parameter bools false by default, and is optional. 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
quest::say("This is [" . quest::saylink("purple text") . "] that you can click.");
```

## scribespells

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; max_level _(int)_, min_level _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to add spells to the spell book of the client character that triggered the event. 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Scribe all spells up to current level
quest::scribespells($ulevel,1);
```

## selfcast

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; spell_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to cause client characters to cast the specified spell on themselves.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Not with your hand, with MY hand!
quest::selfcast(521);
```

## set_proximity

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; min_x _(float)_, max_x _(float)_, min_y _(float)_, max_y _(float)_, min_z _(float)_, max_z _(float)_, say _(bool)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to create a proximity around an NPC.  Necessary to define for both EVENT_ENTER and EVENT_PROXIMITY_SAY (bool the say parameter to true to use this event).  Z min/max and enabling proximity say are both optional.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SPAWN {
     #:: Grab the NPC's location
     $x = $npc->GetX();
     $y = $npc->GetY();
     $z = $npc->GetZ();
     #:: Enable proximity 30 units across, 30 units high, and turn ON proximity say
     quest::set_proximity($x-15, $x+15, $y-15, $y+15, $z-15, $z+15, 1);
}

sub EVENT_PROXIMITY_SAY {
	#:: Match say message for "hail", /i for case insensitive
	if ($text=~/hail/i) {
		quest::say("Hello, $name!");
	}
}

sub EVENT_ENTER {
	#:: Say "hello" when someone nears
	quest::say("Hello, $name!");
}
```

## set_zone_flag

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; zone_id _(uint32)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to set a zone flag for the client character that triggered the event.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SAY {
     if ($text=~/Darkness Beckons/i &&  defined $qglobals{pop_pon_construct} &&  defined $qglobals{pop_pon_hedge_jezith}) {
          $client->Message(1,"Very well mortal... you shall pass into the Lair of Terris Thule");
          $client->Message(2,"You now have access to the Lair of Terris Thule!");
          quest::set_zone_flag(221);
     }
}
```

## setallskill

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; value _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sets all [Skills](https://github.com/EQEmu/Server/wiki/Skills) to the specified value.  You might want to consider a slightly more pinpoint approach like that found in the [Skill Maxer](https://github.com/EQEmu/Server/wiki/Buff-your-Players#Skill_Maxer_PERL) bot.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Set every possible skill to 300--you probably shouldn't do this.
quest::setallskill(300);
```

## setanim

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; npc_type_id _(int)_, appearance_number _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to make the NPC, specified by npc_type ID, to do the specified animation.  Parameters for the appearance are:  0=Stand, 1=Sit, 2=Duck, 3=Feign Death, 4=Kneel

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Make Fippy Darkpawn FD (he's going to die anyhow)
quest::(2001, 3);
```

## setglobal

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; key _(string)_, value _(string)_, options _(int)_, duration _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to set a quest global.  **Consider using [Data Buckets](https://github.com/EQEmu/Server/wiki/Data-Buckets) instead.**  Note that the name of the global is case sensitive.

**Option** | **NPC ID** | **Player** | **Zone**
---------- | ---------- | ---------- | ----------
0 | Current  | Current  | Current
1 | All  | Current  | Current
2 | Current  | All  | Current
3 | All  | All  | Current
4 | Current  | Current  | All
5 | All  | Current  | All
6 | Current  | All  | All
7 | All  | All  | All

**Duration** | **Type** | **Example**
---------- | ---------- | ----------
S | Seconds | S15 = 15 Seconds
M | Minutes | M30 = 30 Minutes
H | Hours   | H12 = 12 Hours
D | Days    | D90 = 90 Days
Y | Years   | Y5 = 5 Years
F | Forever | Never expires.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Set the qglobal "Example", to a value of "1", for all NPCs and zone, and last forever
quest::setglobal("Example", 1, 5, "F");
```

## setguild

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; guild_id _(int)_, guild_rank_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sets the specified guild, by Guild ID, and the specified guild rank, by Rank ID, for the client character that triggered the event.  Ranks are:   0=Member, 1=Officer, 2=Leader.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Add to guild 24
quest::setguild(24,0);
```

## sethp

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; mob_health_percentage _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to set the percentage (0 to 100) of health for the NPC.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Restore HP to 50 percent
quest::sethp(50);
```

## setlanguage

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; skill_id _(int)_, value _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to set the specified [Language](https://github.com/EQEmu/Server/wiki/Languages) to the specified skill level (0 to 100).

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_ENTERZONE {
	#:: Set common tongue to 1 for any new player that is not human
	if ($race ne "Human") {
		if (!defined $qglobals{"newbiecommon"}) {
			$client->SetLanguageSkill(0, 1);
			quest::setglobal("newbiecommon", 1, 5, "F");
		}
	}
}
```

## setnexthpevent

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; at_mob_percentage _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to set an HP event (to trigger EVENT_HP).  When the NPC's health decreases to reach this threshold, the event will be triggered.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SPAWN {
     #:: Trigger EVENT_HP at 90 percent
     quest::setnexthpevent(90);
}

sub EVENT_HP {
     #:: Match if HP is 90 percent
     if ($hpevent == 90) {
          quest::shout("My hit points have reached 90 percent!");
          #:: Trigger EVENT_HP at 80 percent
          quest::setnexthpevent(80);
     }
     elsif ($hpevent == 80) {
          quest::shout("My hit points have reached 80 percent!");
     }
}
```

## setnextinchpevent

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; at_mob_percentage _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to set an HP event (to trigger EVENT_HP).  When the NPC's health increases to reach this threshold, the event will be triggered.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SPAWN {
     #:: Trigger EVENT_HP at 90 percent
     quest::setnexthpevent(90);
}

sub EVENT_HP {
     #:: Match if hit points decrease to 90 percent
     if ($hpevent == 90) {
          quest::shout("My hit points have reached 90 percent--you better keep trying!");
          #:: Trigger EVENT_HP at 91 percent
          quest::setnextinchpevent(91);
     }
     #:: Match if hit points increase to 91 percent
     if ($inchpevent == 91) {
          quest::shout("You are no match for my power!");
          quest::sethp(100);
     }
}
```

## set_rule
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; rule_name _(string)_, rule_value _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to set the specified [Rule](https://github.com/EQEmu/Server/wiki/Server-Rules) to the specified value.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Set Character:MaxLevel to 100 for the current zone.
quest::set_rule("Character:MaxLevel", 100);
```

## setskill

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; skill_id _(int)_, value _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to set the specified [Skill](https://github.com/EQEmu/Server/wiki/Skills) to the specified value.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Set baking to 100
quest::setskill(60, 100);
```

## setsky

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; sky _(uint8)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sets the parameter for the sky (0 to 255)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Turn the sky red
quest::setsky(250);
```

## setstat

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; stat_id _(int)_, value _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sets the specified stat to the specified value (0 to 252).  Stats are:  STR=0, STA=1, AGI=2, DEX=3, INT=4; WIS=5, CHA=6.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Set STR to 250
quest::setstat(0, 250);
```

## settarget

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; target_enum _(string)_, target_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sets the target, by Target ID, for the specified target_enum (either npc_type ID or entity ID).

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SPAWN {
     my @clist = $entity_list->GetClientList();
     foreach my $c (@clist) {
          #:: Tell Fippy to kill!
          quest::settarget(2001, $c);
     }
}
```

## settime

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; new_hour _(int)_, new_min _(int)_, update_world _(bool)_ 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sets the time for the zone or the world to the specified hour and minute.  Update world is optional, but defaults to true--setting it to false makes the time change only apply to the current zone.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Make it 5 o'clock somewhere
quest::settime(17,0);
#:: No--make it 5 o'clock everywhere!
quest::settime(17);
```

## settimer

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; timer_name _(string)_, seconds _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sets a timer (in seconds) that will loop until you stop it.  Gets caught by EVENT_TIMER.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SPAWN {
     #:: Set a timer that loops every 300 seconds (5 min)
     quest::settimer("despawn", 300);
}

sub EVENT_TIMER {
     if ($timer eq "despawn") {
          #:: Stop the timer from looping over and over
          quest::stoptimer("despawn");
          #:: Depop
          quest::depop();
     }
}
```

## settimerMS

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; timer_name _(string)_,  milliseconds _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sets a timer (in milliseconds) that will loop until you stop it.  Gets caught by EVENT_TIMER.  Note that the Lua timer function is in milliseconds as well.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SPAWN {
     #:: Set a timer that loops every 300000 milliseconds (5 min)
     quest::settimerMS("despawn", 300000);
}

sub EVENT_TIMER {
     if ($timer eq "despawn") {
          #:: Stop the timer from looping over and over
          quest::stoptimer("despawn");
          #:: Depop
          quest::depop();
     }
}
```

## sfollow

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; None.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to stop quest::follow();.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Stop following
quest::sfollow();
```

## shout

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; message _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Makes the NPC shout a message to the zone.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
quest::shout("Let it all out!");
```

## shout2

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; message _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Makes the NPC shout a message to the world.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
quest::shout2("Let it all out!");
```

## showgrid

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; grid_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Displays the pathing grid specified by Grid ID.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Show grid 20
quest::showgrid(20);
```

## signal

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; npc_id _(int)_, wait_ms _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sends a signal to an NPC, specified by NPC ID, after a wait period of the specified milliseconds.  Wait is optional and defaults to 0ms.  Compare to quest::signalwith().  Signals trigger EVENT_SIGNAL.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SAY {
	#:: If faction is indifferent or better
	if ($faction < 4) {
		if ($text=~/hail/i) {
			quest::say("Greetings, my friend! You may rest here if you like. There are many dangers in this land. May Tunare watch over you when you depart our camp.");
			#:: signal 70005 - Elmion Hendrys after a 5ms pause
			quest::signal(70005,5);
		}
	} 
	else {
		quest::say("You have some nerve to approach a loyal member of the Paladins of Tunare! Run, while you can!");
	}
}
```

## signalwith

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; npc_id _(int)_, signal_id _(int)_, wait_ms _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sends a signal to an NPC, specified by NPC ID, with a specified Signal ID, after a wait period of the specified milliseconds.  Wait is optional and defaults to 0ms.  Compare to quest::signalwith().  Signals trigger EVENT_SIGNAL.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_WAYPOINT_ARRIVE {
	if ($wp==12) {
		#:: Send a signal "2" to Steamfont Mountains >> Charlotte (56108), after 1ms
		quest::signalwith(56108,2,1);
	}
	if ($wp==18) {
		#:: Send a signal "3" to Steamfont Mountains >> Charlotte (56108), after 1ms
		quest::signalwith(56108,3,1);
	}
}
```

## snow

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; weather _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Changes the snowy weather to the specified setting:  0=none, 1=snow.  See also quest::rain().

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_ZONE {
     if ($name=~/turmoiltoad/i) {
          #:: Turn on the snow for those left behind
          quest::snow(1);
     }
}
```

## spawn

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; npc_type_id _(int)_, grid_id _(int)_, int_unused _(int)_, x _(float)_, y _(float)_, z _(float)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Spawns an NPC by NPC Type ID, on the specified grid, by Grid ID.  The unused int corresponds to guildwarset--use 0 for this value as it is presently unused. 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Spawn Fippy_Darkpaw (2001) on grid 103 at the specified location
quest::spawn(2001, 103, 0, 481.20, 1210.80, 3.10);
```

## spawn2

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; npc_type_id _(int)_, grid_id _(int)_, int_unused _(int)_, x _(float)_, y _(float)_, z _(float)_, heading _(float)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Spawns an NPC by NPC Type ID, on the specified grid, by Grid ID.  The unused int corresponds to guildwarset--use 0 for this value as it is presently unused. Similar to quest::spawn(), with the addition of a heading parameter.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Spawn Fippy_Darkpaw (2001) on grid 103 at the specified location, facing East
quest::spawn2(2001, 103, 0, 481.20, 1210.80, 3.10, 90);
```

## spawn_condition

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; zone_short _(string)_, instance_id _(int)_, condition_id _(uint16)_, value _(int16)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sets the condition and value for the zone spawn condition.  Instance ID is optional and defaults to 0.  You might use this to stop certain NPCs from spawning during a raid event.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SPAWN {
	#:: Set the condition to 3 value 0 to stop a_doomfire_chaosfiend spawn points
	quest::spawn_condition($zonesn, $instanceversion, 3, 0);
}
```

## spawn_from_spawn2

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; spawn2_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to force a spawn_2 point to spawn an NPC even if disabled, or if it already has an NPC spawned.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SPAWN {
     #:: Create a timer that loops every 10 seconds called "fippy")
     quest::settimer("fippy", 10);
}

sub EVENT_TIMER {
     #:: Match timer "fippy"
     if ($timer eq "fippy") {
          #:: Spawn ANOTHER Fippy, which will create another timer, spawn ANOTHER Fippy...chaos ensues.
          quest::spawn_from_spawn2(10875);
     }
}
```

## start

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; grid_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to start an NPC on the specified pathing grid.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SIGNAL {
	#:: Match if signal from steamfont/Jogl_Doobraugh.pl is "1"
	if (($signal == 1) && (($x == -495) || ($x == -734)) && (($y == -154) || ($y == 114))) {
		quest::emote("Beep.. Beep.. Beep..");
		quest::pause(60);
	}
	#:: Match if signal from steamfont/Jogl_Doobraugh.pl is "2"
	if ($signal == 2) {
		#:: Start path grid 178
		quest::start(178);
	}
	#:: Match if signal from steamfont/Jogl_Doobraugh.pl is "3"
	if ($signal == 3) {
		#:: Start path grid 179
		quest::start(179);
	}
}
```

## stop

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; None.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to stop an NPC.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_TIMER {
	#:: Match "CargoTimer" every five seconds
	if ($timer eq "CargoTimer") {
		#:: Match if the quest was not a failure and the time is 8 AM
		if (!defined($qglobals{CargoClockwork}) && ($zonehour == 8)) {
			#:: Set a qglobal in case of quest failure
			quest::setglobal("CargoClockwork",1,1,"H2");
			#:: Start path grid 177 - path to the windmills
			quest::start(177);
		}
		#:: Match if at the spawnpoint (WP 0) and if delivery was completed
		if ($x == 700 && $y == -1783 && $delivery == 1) {
			#:: Stop pathing on path grid 177
			quest::stop();
			#:: Reset the delivery state
			$delivery = 0;
		}
	}
}
```

## stopalltimers

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; None.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Stops all the timers currently running from the script.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Stop all the timers
quest::stopalltimers();
```

## stoptimer

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; timer_name _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Stops the specified timer from looping.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SPAWN {
     #:: Set a timer "despawn" to loop every 300 seconds (5 min)
     quest::settimer("despawn", 300);
}

sub EVENT_TIMER {
     #:: Stop the timer "despawn"
     quest::stoptimer("despawn");
     #:: Depop
     quest::depop();
}

sub EVENT_COMBAT {
     #:: Stop the timer if we enter combat
     if ($combat_state == 1) {
          quest::stoptimer("despawn");
     }
     #:: Start the timer once combat is finished
     else {
          quest::settimer("despawn", 300);
     }
}

sub EVENT_DEATH_COMPLETE {
     #:: Stop the timer "despawn" if I die
     quest::stoptimer("despawn");
}
```

## summonallplayercorpses

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; char_id _(int)_, dest_x _(float)_, dest_y _(float)_, dest_z _(float)_, dest_heading _(float)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Summons all character corpses, by Char ID, to the specified location.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SAY {
     if ($text=~/corpses/i) {
          quest::say("Summoning all of your corpses now.");
          #:: Summon all player corpses to the current location, facing North
          quest::summonallplayercorpses($charid, $x, $y, $z, 0);
     }
}
```

## summonburiedplayercorpse

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; char_id _(uint32)_, dest_x _(float)_, dest_y _(float)_, dest_z _(float)_, dest_heading _(float)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Summons all buried character corpses, by Char ID, to the specified location.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SAY {
     $corpse = quest::getplayerburiedcorpsecount($charid);
     if ($text=~/corpses/i && $corpse > 0) {
          #:: Summon all buried player corpses to the current location, facing North
          quest::summonburiedplayercorpse($charid, $x, $y, $z, 0);
     }
}
```

## summonitem

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  item_id _(int)_, charges _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Summons the specified item, by Item ID, with the specified number of charges, to the cursor of the client character that triggered the event.  Charges is the number of charges, or the count of the item, and is optional.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_ITEM {
	#:: Match 66gp and a 13990 - Bale of Hay
	if (plugin::takeItemsCoin(0,0,66,0, 13990 => 1)) {
		quest::say("'Whatsssss thisssss? You sssseek my blessssssssing? Heh heh heh... Very well... CAZIC-THULE! Take this fruit of Karana into horror'sss dark embrace. Fear and death made manifesssssst. A harvesssst of terror! Here, take your gift of blood and sssstraw. Use its dark powersssss in the name of the Fear Lord!' ");
		#:: Give a 14320 - Sack of Cursed Hay
		quest::summonitem(14320);
		#:: Ding!
		quest::ding();
		#:: Give a small amount of experience
		quest::exp(300);
		#:: Set faction
		quest::faction(18, 10);		#:: + Beta Neutral
	}
	#:: Return unused items
	plugin::returnUnusedItems();
}
```

## surname

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; name _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Changes the surname of the client character that triggered the event to the provided string.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Set last name to "Toad"
quest::surname("Toad");
```

## targlobal

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; key _(string)_, value _(string)_, duration _(string)_, npc_id _(int)_, chararacter_id _(int)_, zone_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sets a quest global with the given parameters to a character anywhere in the world.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Set a global "Example" with a value of "5" for 30 minutes
quest::targlobal("Example", "5", "M30", 2001, $charid, $zoneid);
```

## task_setselector

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; task_set_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sets the Task Set, by provided Task Set ID.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Set task set 202
quest::task_setselector(202);
```

## taskexplorearea

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; explore_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to mark any explore activities (type 5), which have the numeric value Explore ID in their Goal ID field, and for which the Zone ID of the activity is either 0 or this zone, as completed.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Mark Task 21 complete
quest::taskexplorearea(21);
```

## taskselector

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; task_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to bring up the Task Selector Window with the specified tasks available for selection (from 1 to 40 task_id(s)). Note that when the task selector is brought up via this method, no check is made as to whether the character has the tasks enabled.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_SAY {
     if ($text=~/hail/i) {
          quest::say("Heyo! Looking for an exciting [task] to fill the time?");
     }
     if ($text=~/task/i) {
          #:: Select task 103
          quest::taskselector(103);
     }
}
```

## tasktimeleft

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; task_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Returns the amount of time left, in seconds, before the specified task runs out.  -1 is returned if there is no time limit, or if the player does not have the task.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Create a scalar variable to store the amount of time left for Task ID 22
$timeremaining = quest::tasktimeleft(22);  #:: Returns int
if ($timeremaining => 1) {
     quest::say("You have $timeremaining seconds left--better hurry!");
}
else {
     quest::say("Sorry $name, but you're out of time!");
}
```

## toggle_spawn_event

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; event_id _(uint32)_, is_enabled _(bool)_, is_strict _(bool)_, reset_base _(bool)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to toggle the enabled state of a specified [Spawn Event](https://github.com/EQEmu/Server/wiki/spawn_events), by Event ID.  The parameters for is_enabled, is_strict, and reset_base are all false by default.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_DEATH_COMPLETE {
     #:: Turn the depop spawn_event back on
     quest::toggle_spawn_event(65, 1, 0, 0);
}
```

## toggledoorstate

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; door_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Toggles the open/closed state of the specified door.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_CLICKDOOR {
     my $tds = quest::isdooropen(41);
     my $bds = quest::isdooropen(42);
     if (($doorid == 41 && !$tds) || ($doorid == 42 && !$bds)) {
          quest::toggledoorstate(38);
          quest::toggledoorstate(39);
          quest::toggledoorstate(40);
     }
}
```

## traindisc

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; tome_item_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Trains the discipline of the specified Tome ID for the client character that triggered the event.  Generally you will simply use the plugin:  plugin::try_tome_handins(\%itemcount, $class, 'Ranger');--part of the contents of which are in the example below.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
if (@tomes > 0) {
	if ($isclass eq $expectclass) {
		foreach my $i(@tomes) {
			quest::traindisc($i);
		}
	}
}
```

## traindiscs

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; max_level _(int)_, min_level _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to train all disciplines for the class up to the specified max_level, if that level is less than rule Character:MaxLevel, or the character is a GM.  The parameter for min_level defaults to 1.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Train disciplines up to level 70
quest::traindiscs(70,1);
```

## unique_spawn

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; npc_type_id _(int)_, grid_id _(int)_, int_unused _(int)_, x _(float)_, y _(float)_, z_ (float)_, heading _(float)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Similar to the quest::spawn() command, except that it will not spawn the specified NPC if the same npc_type ID is already in the zone.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
sub EVENT_DEATH_COMPLETE {
	my $random_result = int(rand(100));
	if ($random_result >= 94) {
		#:: Spawn a Steamfont Mountains >> Minotaur_Hero (56152)
		quest::unique_spawn(56152,177,0,-1294,1360,-103);
	}
	elsif ($random_result >= 88 && $random_result < 94) {
		#:: Spawn a Steamfont Mountains >> Minotaur_Lord (56161)
		quest::unique_spawn(56161,0,0,-2179,1319,-101.2);
	}
	quest::say("I die soon! Meldrath, help me!");
}
```

## unscribespells

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; None.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Unscribes all spells for the client character that triggered the event.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Unscribe all spells
quest::unscribespells();
```

## untraindiscs

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; None.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Untrains all disciplines for the client character that triggered the event.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Untrain all disciplines
quest::untraindiscs();
```

## updatetaskactivity

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; task_id _(int)_, activity_id _(int)_, count _(int)_, ignore_quest_update _(bool)_ 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to increment the done count of the specified task is active.  The parameter for ignore_quest_update is optional, and defaults to false; the parameter for count default to 1 (increase count by 1).

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Update Task ID 219 activity 9, by 1 count
quest::updatetaskactivity(216,9);
```

## varlink

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; item_id _(uint32)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to create an item link that can be used in a variable.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Create a scalar variable to store an item link for a 1001 - Cloth Cap
my $Reward = quest::varlink(1001);
```

## voicetell

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; client_name _(string)_, macro_id _(int)_, race_id _(int)_, gender_id _(int)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Plays the specified audio message on the client of the character that triggered the event.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Send voice macro "Agree" to the client
quest::voicetell($name, 1);
```

## we

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; emote_color_id _(int)_, message _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sends an emote message to the world in the specified color.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Send yellow (15) text
quest::we(15, "Hello world!");
```

## wearchange

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; slot _(uint8)_, texture_id _(uint16)_, hero_forge_model_id _(uint32)_, elite_material_id _(uint32)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to change the texture/model of visible [Slots](https://github.com/EQEmu/Server/wiki/Inventory-Slots).  The parameters for hero_forge_model and elite_material_id default to 0.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Change the appearance of the character's weapon
quest::wearchange(13, 3);
```

## worldwidemarquee

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; color_id _(uint32)_, priority _(uint32)_, fade_in _(uint32)_, fade_out _(uint32)_, duration _(uint32)_, message _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Used to send a worldwide marquee message with the specified parameters.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Send a worldwide marquee message in yellow (15), 
quest::worldwidemarquee(15, 1, 1, 1, 1000, "Hello World!");
```

## write

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; file_name _(string)_, message _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Writes the specified message string to the specified file name.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
quest::write("HandIn/$npc_name$zonesn.txt","[$timestamp] : $name the $ulevel has handed in $Item1, $Item2, $Item3, $item4 into $npc_name, and gotten $RewardID.");
```

## ze

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; emote_color_id _(int)_, message _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sends a zone-wide emote message in the specified color.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Send a zone-wide emote in yellow (15)
quest::ze(15,"welcomes the world.");
```

## zone

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Parameter(s):**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; zone_name _(string)_

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Usage:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sends the client character that triggered the event to the specified zone (by zone short name).

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Example:**

```perl
#:: Send the player to the West Commonlands
quest::zone(commons);
```