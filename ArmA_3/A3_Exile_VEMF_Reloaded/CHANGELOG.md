## VEMF Changelog

#### `v0740.30`
*Server-side* <br />
**[ADDED]** Option to prevent AI from having TWS (thermal) scopes <br />
**[CHANGED]** Order of config settings from being a total mess to being alphabetically sorted. <br />
<br />

#### `v0740.27`
*Server-side* <br />
**[ADDED]** More advanced ammo distribution system for AI units <br />
**[FIXED]** Sometimes no .50 cals at missions <br />
**[FIXED]** "Error: no vehicle" when killing AI with Helicopter <br />
**[CHANGED]** A few comments in config.cpp to improve clearness<br />
<br />

#### `v0740.19`
*Server-side* <br />
**[ADDED]** Option to enable/disable respect punishment for roadkilling AI <br />
**[ADDED]** Option to remove "toolbelt" items like GPS, Radio, Map and Compass from AI <br />
**[ADDED]** New options class to control AI cleanup-related settings <br />
**[ADDED]** AI units now randomly have random weapon attachments <br />
**[NEW]** Config.cpp does NOT use -1 anymore to disable things. It is now 0 instead.<br />
**[CHANGED]** Config.cpp option comments <br />
**[CHANGED]** On roadkill, kill message shows [Roadkill] instead of vehicle used <br />
**[IMPROVED]** Overall code performance and use of newer commands <br />
**[FIXED]** Mines are not working <br />
**[REMOVED]** fn_random.sqf, replaced by selectRandom command https://community.bistudio.com/wiki/selectRandom <br />
<br />

#### `v0740.6`
*Server-side* <br />
**[CHANGED]** BIS_fnc_param replaced by new param command <br />
**[CHANGED]** Blacklist method for locations. Seperate classes for each map for easier use <br />
<br />
*Client-side* <br />
No Changes. <br />
<br />

#### `v0732.8`
*Server-side:* <br />
**[ADDED]** AI static spawns <br />
**[ADDED]** fn_aiKilled: now shows the name of vehicle used to road-kill an AI <br />
**[ADDED]** fn_checkLoot: RPT log message if loot validation is enabled but no debug allowed <br />
**[IMPROVED]** Descriptions and naming of config values <br />
**[IMPROVED]** fn_aiKilled: now shows killer [weapon, range] victim <br />
**[IMPROVED]** fn_log: is now faster and much more simple <br />
**[FIXED]** fn_aiKilled: if killer using vehicle gun, it shows the primaryweapon of the killer instead of the vehicle turret as the weapon used <br />
**[CHANGED]** Mission complete logs now show the name of location in which the mission was <br />
**[CHANGED]** Name of pbo is now all lowercase <br />
<br />
*Client-side:* <br />
**[CHANGED]** mission notification messages now have VEMFr as tag instead of the old VEMF tag <br />
<br />

#### `v0730.21`
**[REMOVED]** Medikit and toolkit from loot crate(s) <br />
<br />

#### `v0730.20`
**[ADDED]** Option to control the classname of the AI units <br />
**[ADDED]** Automatic detection of AI unit's side to make sure they get put into a correct group type <br />
<br />

#### `v0730.15`
**[ADDED]** Option enable/disable the ability to lift loot crate <br />
<br />

#### `v0730.14`
**[FIXED]** Loss of respect when using vehicle turret <br />
**[FIXED]** Server-side script error caused by killTheLights <br />
<br />

#### `v0730.2`
**[NEW]** refreshed mission notification with new animations <br />
**[FIXED]** difficult to see quickly if mission message means new one or a defeated one <br />
**[FIXED]** network load peak and fps lag when mines are placed by mission <br />
**[CHANGED]** server-side message broadcasting to accommodate for including the notification type in the broadcast <br />
<br />

#### `v0729.1`
**[CHANGED]** increased detection speed of players for triggering missions from 200 to 250 <br />
**[REMOVED]** any usage of playableUnits command <br />
**[REMOVED]** any checks for the player's side <br />
**[FIXED]** old stuff in fn_checkLoot.sqf <br />
**[FIXED]** mission amount can go beyond the limit <br />
**[FIXED]** fn_playerCount.sqf: unreliable detection of player amount <br />
**[FIXED]** VEMF_Reloaded started anyway without the actual amount of minimal players to be ingame <br />
**[IMPROVED]** fail-safe "if checks" in fn_missionTimer.sqf <br />

#### `v0728.6`
**[FIXED]** Instabilities in spawning/despawning of missions <br />
**[FIXED]** First mission does not timeout <br />
**[ADDED]** Option to blacklist certain buildings using their classnames <br />
**[NEW]** Each DynamicLocationInvasion mission type has its own marker color <br />
<br />

#### `v0727.15`
**[FIX ATTEMPT]** Missions not spawning anymore under very specific conditions <br />
<br />

#### `v1.0727.13`
**[FIXED]** fn_loadInv not working for the bad guys <br />
**[FIXED]** random missions not working if mission announcements were disabled <br />
<br />

#### `v1.0727.11`
**[FIXED]** Missions stop spawning after a certain amount of time <br />
<br />

#### `v1.0727.9`
**[ADDED]** Option to disable/enable mission announcements <br />
<br />

#### `v1.0727.3`
**[CHANGED]** Exile_VEMF is now called Exile_VEMF_Reloaded because the original creator of VEMF is proceeding on VEMF <br />
**[ADDED]** S.W.A.T. AI <br />
**[ADDED]** Option to send kill messages only to the killer (@KillingRe) <br />
<br />

#### `v1.0725.6`
**[NEW]** Option to control deletion of .50 cals when mission done <br />
**[IMPROVED]** Respect reward system <br />
**[FIXED]** Players getting respect if AI kill other AI <br />
<br />

#### `v1.0724.1`
**[NEW]** Option to control distance between each mission <br />
**[CHANGED]** Server-side folder is now called Exile_VEMF <br />
<br />

#### `v1.0723.1 HOTFIX`
**[FIXED]** fn_aiKilled.sqf: error Undefined variable in expression unit <br />
<br />

#### `v1.0722.15`
**[NEW]** Player now get reputation for killing AI. Dynamically increases depending on kill distance <br />
**[FIXED]** Unstable fn_random.sqf <br />
<br />

#### `v1.0721.15`
**[NEW]** AI will now spawn in houses <br />
**[NEW]** Mounted (bipod) .50 cals in/on houses if enabled <br />
**[ADDED]** Option to enable/disable AI "Cop mode" <br />
**[CHANGED]** fn_spawnAI.sqf to allow spawning in houses <br />
**[TWEAKED]** fn_loadInv.sqf <br />
<br />
#### `v1.0721.1`
**[FIXED]** fn_spawnAI.sqf: Suspending not allowed in this context, line 72 <br />
<br />

#### `v1.0720.6`
**[NEW]** Automatic removal of loot crate marker when player gets close <br />
**[ADDED]** Option to enable/disable mission markers <br />
**[ADDED]** Ability to put `maxGlobalMissions` on -1. Disables the mission limit <br />
**[ADDED]** Exile default safe zones to mission blacklist positions <br />
**[ADDED]** Option to enable/disable loot crate markers <br />
**[ADDED]** Option to enable/disable loot crate parachute spawn <br />
**[ADDED]** Option to enable/disable loot crate visual smoke/chemlights <br />
**[ADDED]** Option to enable/disable loot crate spawn sound (once) <br />
**[ADDED]** Logging of successfull removal/exploding of mines <br />
**[ADDED]** Code changes to fn_missionTimer.sqf to allow ignoring of global mission count <br />
**[ADDED]** Code changes to DLI mission to prevent removal of non-existing mission marker <br />
**[CHANGED]** several config options from negative to positive <br />
**[CHANGED]** Default debug mode from 2 to 0 (errors only) <br />
**[CHANGED]** AI difficulty config now less lines <br />
**[CHANGED]** AI Veteran and Harcore difficulty increased <br />
**[CHANGED]** Mines are now switched off by default <br />
**[CHANGED]** Default mine removal mode is now explode <br />
**[CHANGED]** fn_loadLoot.sqf: now empties the crate instead of the mission itself <br />
**[FIXED]** Error in expression fn_findPos.sqf <br />
**[FIXED]** Error in expression fn_loadInv.sqf with specific set of config settings <br />
<br />

#### `v1.0719.10`
**[ADDED]** Option to enable/disable the placement of a marker on the loot crate <br />
**[ADDED]** Attempt to fix the floating crate problem <br />
**[ADDED]** Fail-safety for fn_checkPlayerPresence.sqf <br />
**[ADDED]** Fail-safety for fn_placeMines.sqf <br />
**[ADDED]** Fail-safety for fn_spawnAI.sqf <br />
**[CHANGED]** Default value of `validateLoot` from 1 to -1 <br />
**[REMOVED]** Option to enable/disable sound on the loot crate <br />
**[FIXED]** Mines not removing or exploding <br />
**[FIXED]** Structure error in fn_findPos.sqf <br />
<br />
#### `v1.0718.11`
**NOTE:** VEMFclient code has been changed! <br />
**[ADDED]** AI difficulty presets<br />
**[CHANGED]** Default cleanMines setting changed from 2 to 1 <br />
**[CHANGED]** fn_broadCast.sqf for new broadcast system <br />
**[CHANGED]** fn_loadLoot.sqf: fail-safety removed <br />
**[CHANGED]** fn_spawnAI.sqf: implementation of AI difficulty presets <br />
**[CHANGED]** Veteran AI difficulty lowered. Too close to aimbots <br />
**[FIXED]** Duplicate spawns on locations <br />
**[FIXED]** Player getting side ENEMY for attacking AI <br />
**[FIXED]** Loot crate not falling down <br />
**[FIXED]** Loot crate not making a sound <br />
<br />
#### `v1.0717.7`
**[FIXED]** No loot in crate <br />
**[FIXED]** AI not shooting at player <br />
<br />

#### `v1.0716.14`
**[NEW]** VEMF ported to Exile :) <br />
<br />
