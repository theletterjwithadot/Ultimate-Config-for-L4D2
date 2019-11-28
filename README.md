# Ultimate L4D2 Config by J.

- [Ultimate L4D2 Config by J.](#ultimate-l4d2-config-by-j)
  * [Reviews](#reviews)
  * [Disclaimer](#disclaimer)
  * [Purpose](#purpose)
  * [Backing up old config](#backing-up-old-config)
  * [Instructions](#instructions)
  * [The files](#the-files)
    + [CSGO Font](#csgo-font)
    + [autoexec.cfg](#autoexeccfg)
    + [ultimateconfig.cfg](#ultimateconfigcfg)
  * [Breakdown of ultimateconfig.cfg](#breakdown-of-ultimateconfigcfg)
    + [Reset Config](#reset-config)
    + [General Client Settings](#general-client-settings)
    + [Subtitles](#subtitles)
    + [Video](#video)
    + [Audio](#audio)
    + [Mic](#mic)
    + [Network](#network)
    + [Rates & Lerps](#rates---lerps)
    + [Crosshair](#crosshair)
    + [Mouse](#mouse)
    + [Keyboard](#keyboard)
    + [Glows](#glows)
    + [Netgraph](#netgraph)
    + [Binds](#binds)
    + [Aliases](#aliases)
    + [Toggles](#toggles)
    + [Server Connect Binds](#server-connect-binds)
    + [Final Launch Parameters](#final-launch-parameters)
    + [Custom Configs](#custom-configs)
    + [Write Changes To Config](#write-changes-to-config)

## Reviews

> I was using other incomplete/outdated configs that I found online before I had this ultimate config. My gameplay has drastically been improved by it.
> 
> Audio is significantly clearer and I am able to hear the direction of the SI better. There is also glow adjustments that made it distinct and also differentiate the importance of each action in the game (white for SI ghost, red for SI incapacitated Survivor, purple for biled players). The null-cancelling movement keys also makes a difference but takes some time to get used to in order to take full advantage of it when juking tank rocks. The mouse adjustments was another item that took time to get used to but once I have gotten used to it, aiming accurately became second nature. 
>  
> Another helpful function of the ultimate config was the server aliases that allows me to reconnect to the proper IP address of each server. This saves a lot of time as I do not have to search for the IP or ask around for the IP anymore. Since the alias takes care of me disconnecting and then connecting back to the server, it is almost instant.
>
> The one feature I commonly use is “F5” which is to help clear the survivor looking stuck in the saferoom or invisible SI. It does the “record 1; stop” command but in a single press instead of typing it. 
> 
> There are plenty more features that are in this configuration that I have not yet mentioned, my final verdict for this custom configuration is that this is a MUST-HAVE config for both new and experienced players. You will not regret it.

*[Maverick](http://www.steamcommunity.com/profiles/76561198017890288 "Maverick")*


>LISTEN UP EVERYONE!
>
>I wanna start this review by stating that this IS the ultimate config for L4D2. This config has audio fixes that’ll give you “EAR-PORN” (IN THE AUTHORS’S OWN WORDS) - which is a fact.
>
>Glow fixes and aliases that will help you with server connections, mouse and keyboard input and many more that’ll help you with your gameplay. These are fixes that are very much needed for L4D2. I’ve been using old configs and launch options that I felt helped improve my gameplay until I was approached by my dear friend, the author of the ultimate config, to try/test it and give him suggestions and my review on it. 
>
>But damn! There was no suggestions I could give because it’s damn near perfect. I now feel that I had been using the wrong configs all these while. I won’t get into details of what this config does as the J. has already included instructions in the config he wrote. 
>
>What I will tell you is that, after a versus L4D2 player for so long being, I give my stamp of awe and approval for his work after testing/using it for a few weeks. Rating this ultimate config 12 outta 10 stars #cantlivewithoutit

*[daemon9s](http://www.steamcommunity.com/profiles/76561198308768316 "daemon9s")*


## Disclaimer
The config has been tested for more than a year with multiple players and has proven to be very useful.
The config here is given "AS IS" with no warranty.
The config changes quite a handful of [cvars](https://developer.valvesoftware.com/wiki/List_of_L4D2_Cvars) in the game as such, please perform your own backup if you would like to rollback to your previous config.

## Purpose
Many players do not have the basic setup for Left 4 Dead 2 which hinders them from playing well in the competitive servers especially those running on above the default server tickrate of 30.
This config is meant to provide a player with the needed adjustments and also with additional features that assists and optimizes their gameplay.
My goal of sharing this config is to get more players to have the optimal settings configured for this game so that everyone can have a better gaming experience all together.

## Backing up old config
 1. Go to your Left 4 Dead 2 installation directory `.../Steam/steamapps/common/Left 4 Dead 2/left4dead2/`
 2. Create a copy of the folder `cfg` and rename it to `cfg.bak`
 3. This will be your backup

## Instructions
 1. Read through the config to understand what is happening
 2. Drop the folders into your game directory:
`.../Steam/steamapps/common/Left 4 Dead 2/left4dead2/`
 3. Setup launch options of L4D2 - Right-click Left 4 Dead 2 >> Properties >> Set Launch Options
 4. Add the following line into the box: `-lv +mat_queue_mode 2 +precache_all_survivors 1 -novid -console -noipx -nod3d9ex -nojoy -noforcemaccel -noforcemparms +mat_motion_blur_percent_of_screen_max 0 +clientport 27619`
 5. Remove `-lv` if you want all the gore and violence
 6. Setup video settings as per given below if you have a potato computer like mine (you may use your own settings for items in **bold** if you have a beast computer)

| Setting                     	| Value                                                    	|
|-----------------------------	|----------------------------------------------------------	|
| Aspect Ratio                	| As per yours                                             	|
| Resolution                  	| Use native resolution                                    	|
| Display Mode                	| Full screen                                              	|
| **Film Grain Amount**       	| None                                                     	|
| **Anti-Aliasing Mode**      	| None                                                     	|
| **Filtering Mode**          	| Trilinear                                                	|
| Wait For Vertical Sync      	| Disabled                                                 	|
| **Shader Detail**           	| Low                                                      	|
| Effect Detail               	| High (This is to ensure you can see tank rocks from far) 	|
| **Model/Texture Detail**    	| Low                                                      	|
| Multicore Rendering         	| Enabled                                                  	|
| Paged Pool Memory Available 	| High                                                     	|

 7. Launch game and open console and run the following command once: `unbindall; exec config_default.cfg; exec autoexec.cfg`
 8. Change any binding that you do manually (like binding different key to zoom, changing crouch key, etc) in the game settings
 
## The files

### CSGO Font
    .../addons/CSGO Font.vpk
A font pack that makes the game menu and texts nicer and clearer to read.

### autoexec.cfg
    .../cfg/autoexec.cfg
The autoexec.cfg runs a command that is needed to make the CSGO Font addon to work. Ensure that you change the resolution in

> alias reloadfont "mat_setvideomode **1920 1080** 1; mat_setvideomode **1920 1080** 0"

to match your resolution. It is also where the ultimateconfig.cfg is called to be executed.

### ultimateconfig.cfg
    .../cfg/ultimateconfig/ultimateconfig.cfg
This is where the rest of the magic happens.

## Breakdown of ultimateconfig.cfg
### Reset Config
Reset the game configuration to the default configuration before we make changes.
Commented out as not everyone know how to deal with this.
As it resets the configuration and applies only what is in this config, whatever extra custom config that a user has done manually will not be saved.

### General Client Settings
Just basic client cvars, enabling console, disabling joystick and Steam controller.

### Subtitles
Sets up the subtitles for the game.
Quite useful.

### Video
Increase game brightness (adjust the value if the game is too bright).
Reduce unnecessary animations that eat up few FPS.

### Audio
Disable music volume to hear SI better.
Setup audio to have better clarity.
Comment out `windows_speaker_config` if you have different speaker setup than headphone/stereo and set it up in the game.

### Mic
Basic mic setup.
Nothing fancy.

### Network
Setup network settings for competitive mode.

### Rates & Lerps
Aliases for rates, lerps and interp ratio.
Extremely useful to change lerp in an instant.

### Crosshair
Setup crosshair to be white with black border (colorblind mode).
The crosshair is most visible in this mode.
There is also aliases to change crosshair color.

### Mouse
Disabling all sorts of mouse filters to give the game the raw mouse movement.

### Keyboard
A must-have null-cancelling movement script for movement keys.

### Glows
Glows are self-explanatory.

### Netgraph
Displays crucial information of whether the server you are in is having any issues with rates, chokes or loss.
It also shows your ping to the server.

### Binds
Useful binds for competitive modes (do not forget to uncomment the line if you want to use those binds).
The most useful one is `F5` which is to get rid of those "invisible SI, survivor stuck in saferoom" issues.

### Aliases
Aliases to shorten commands.

### Toggles
Useful toggles.

### Server Connect Binds
Servers in the Asian region has more than one IP to connect to.
As such, for convenience sake, all servers and their alternate IPs are set in aliases so as to join them quickly instead of doing the whole "what is the VPN for this server? Copy-paste-connect" thing.
Read through the aliases to get familiar with the aliases used.

### Final Launch Parameters
Setting up the lerp, rates and interp to use here.

### Custom Configs
Any additional configs you want to add can be added here.

### Write Changes To Config
Write the config to the game.