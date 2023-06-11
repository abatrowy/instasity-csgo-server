instasity
![https://img.shields.io/badge/game-csgo-green](https://store.steampowered.com/app/730/CounterStrike_Global_Offensive/)
![Language](https://img.shields.io/badge/language-SP-red)
-
my old project for counter strike: global offensive server that has 23 different gamemodes.

i given up because of cs2 release and [latency problems](https://i.imgur.com/IeM8Orx.png)

how it works?
-
server is automatic, it will load settings and config for every choosen gamemode with map.


important:
-
- before joining server, you have to set cl_downloadfilter "all", sv_allowupload_1 (there's a plugin to force it)
- 80% of polish support. (mostly plugins were translated by myself)


## preferable startup parameters

```bash
 srcds_run -console -game csgo -usercon +game_type 0 +game_mode 1 -nohltv -tickrate 128 -maxplayers 12 -maxplayers_override 12 +ip 188.165.19.26 -port 27425 +sv_setsteamaccount "AF8ABFF1AED19965AC6799FD3FEDE008" -exec server.cfg -insecure +mapgroup mg_bomb +mapgroup mg_active +map surf_monstergreen_pb
```

this server contains:
-
- full working RTV, first vote is for gamemode and second vote is for map. (!rtv)
- knifes, gloves, stickers customization (!knife, !gloves, !sticker)
- custom models (!models)
- custom matchmakming rank on scoreboard (!mm)
- custom pins on scoreboard (!pin)
- custom mvp sound (!mvp)
- option to disable music on every map with volume option (!music)
- fortnite dances (!t, !tance, !dance)
- hitmarkers (!hit)
- skybox chooser (!sky)
- quake (!quake)
- custom c4 sounds (!c4)
- kda reset (!rs)
- thirdperson (!tp)
- statistics - kills, deaths, time played on a server (!lvl)
- welcome, join, disconnect sounds (https://github.com/abatrowy/announcements-plugin)
- custom command server menu (!ustawienia)

custom decals on map:
-
[![Watch the video](https://i.imgur.com/vKb2F1B.png)](https://youtu.be/K9q2QH5nEps)

gamemodes with features:
-
__awp:__
- if there's 1v1, the vote for noscope battle begins
- after 3 rounds, there's gonna be noscope round with custom sound.
-  ghost mode if u die with noclip function (!duch)

__only mirage:__
- anti rush plugin
- parachute (hold E)
- random defuse color cable (4 available)
- bomb timer, with custom sounds
- ghost mode if u die with noclip function (!duch)

__1v1 arena:__
- gun choose menu (!gun, !weapon)
- heavy, awp, noscope scout, headshot round selection

__gungame__
- customizable weapon gains, after 20 kills last one who kills with knife - wins.

__retakes__
- autoplant
- site detector with custom sound
- gun menu (!gun, !weapon)

__ffa__
- type "hs" in chat to enable only headshot 
- gun menu (!gun, !weapon)

__hide and seek__
- just a default hide and seek, without any plugins.

__prophunt__
- hint with custom sounds (!whistle)
- custom model menu (!model)

__base builder__
- party mode (!party)
- store menu (!shop)
- respawn if stuck (!r)

__golf__
- customizable golf holes (!golfedit)

__jailbreak__
- custom menu (click "," or just write !menu)
- prison/guards custom models (!models)
- warden (!warden)
- guards gun selection (!guns)
- marker menu (!marker)
- last request (!lr)
- event days (!vd)
- dice (!dice, !kostka)
- parachute (hold E)
- ghost mode if u die with noclip function (!duch)

__minigames__
- default minigames with bunnyhop and accuracy support
- ghost mode if u die with noclip function (!duch)

__minigames course__
-  auto move to T 
- anti block and anti velocity plugins providing to fix velocity movement
- ghost mode if u die with noclip function (!duch)

__deathrun__
- free run (!fr)
- random terrorist will be chosen every round
- menu with level system. allowing to buy abilities
- velocity custom HUD
- anti block and anti velocity plugins providing to fix velocity movement
- ghost mode if u die with noclip function (!duch)

__super powers__
- 15 random super powers every round of spawn. including also message on chat
- ghost mode if u die with noclip function (!duch)

__surf__
- hud with stages, timer, velocity
- replay bot
- WR/map server
- zones

__surfrpg__
- nospread support
- higher velocity support
- anti buyzone kill
- 5s protection from getting spawnkill
- no fall damage
- 1v1 noscope duel
- random defuse color cable (4 available)
- ghost mode if u die with noclip function (!duch)

__bhop__
- hud with stages, timer, velocity
- replay bot
- WR/map server
- zones

__hns__
- custom velocity HUD
- custom menu with noclip, saving and loading positions
- no fall damage 

__hns rpg__
- random grenades, including freeze grenade with decoy
- anti flash for CT
- custom velocity HUD
- ghost mode if u die with noclip function (!duch)

__kz (longjump)__
- custom HUD with velocity
- menu with noclip, saving and loading positions
- no fall damage

__kz climb__
- hud with stages, timer, velocity
- no fall damage
- replay bot
- WR/map server

__duckhunt__
- random sniper will be chosen every round.
- ghost mode if u die with noclip function (!duch)

__unusual custom 4fun maps__
- just a default 4 fun maps, without any plugins.
- ghost mode if u die with noclip function (!duch)



__obviously i wrote stuff that i remember, there's might be something for sure i dont remember lol.__

things i've fixed before releasing this project publicly:
-
- server startup logic (including startup plugins etc etc)
- server optimization
- random kicks from server (most common: "you may only connect to this server from a lobby"
- random crashes, freezes
- gamebreaking bugs
- menu models
- arms while wearing custom skin/model
- mp3 downloading and missing models
- bomb planting (weird hostage bug that i struggled 5 days straight how to fix that)
- rtv
- random spawns
- problems with cvars
- plugins that emited 7 sounds in a row (added cooldown)

things TO DO:
-
- fix latency lag spike
- fix surf timer plugin / database
- fix kz climb plugin / database
- super powers: wallhack doesn't work.
- improve basebuilder shop (its broken currently)

Q&A:
-
__will this get me token banned? (GSLT)__
- yes, you can prevend this by removing 3rd party plugins which is against valve rules 

__will i update this project in a future to cs2?__
- 95% no, im tired of this game so that's why i realesed this.

__will i help you run this server on your own?__
- nope.

