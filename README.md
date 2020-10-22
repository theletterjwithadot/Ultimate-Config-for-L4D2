# Ultimate L4D2 Config by J. (autoexec)

[TOC]

## Disclaimer

- The config has been tested for years with multiple players and has proven to be very useful
- The config here is given "AS IS" with no warranty
- The config changes quite a handful of [cvars](https://developer.valvesoftware.com/wiki/List_of_L4D2_Cvars) in the game as such, please perform your own backup if you would like to rollback to your previous config
- Individual's mileage may vary

## Reviews

> *I was using other incomplete/outdated configs that I found online before I had this ultimate config. My gameplay has drastically been improved by it.*
>
> *Audio is significantly clearer and I am able to hear the direction of the SI better. There is also glow adjustments that made it distinct and also differentiate the importance of each action in the game (white for SI ghost, red for SI incapacitated Survivor, purple for biled players). The null-cancelling movement keys also makes a difference but takes some time to get used to in order to take full advantage of it when juking tank rocks. The mouse adjustments was another item that took time to get used to but once I have gotten used to it, aiming accurately became second nature.* 
>
> *Another helpful function of the ultimate config was the server aliases that allows me to reconnect to the proper IP address of each server. This saves a lot of time as I do not have to search for the IP or ask around for the IP anymore. Since the alias takes care of me disconnecting and then connecting back to the server, it is almost instant.*
>
> *The one feature I commonly use is “F5” which is to help clear the survivor looking stuck in the saferoom or invisible SI. It does the “record 1; stop” command but in a single press instead of typing it.* 
>
> *There are plenty more features that are in this configuration that I have not yet mentioned, my final verdict for this custom configuration is that this is a MUST-HAVE config for both new and experienced players. You will not regret it.*

[Maverick](http://www.steamcommunity.com/profiles/76561198017890288 "Maverick")

> *LISTEN UP EVERYONE!*
>
> *I wanna start this review by stating that this IS the ultimate config for L4D2. This config has audio fixes that’ll give you “EAR-PORN” (IN THE AUTHORS’S OWN WORDS) - which is a fact.*
>
> *Glow fixes and aliases that will help you with server connections, mouse and keyboard input and many more that’ll help you with your gameplay. These are fixes that are very much needed for L4D2. I’ve been using old configs and launch options that I felt helped improve my gameplay until I was approached by my dear friend, the author of the ultimate config, to try/test it and give him suggestions and my review on it.* 
>
> *But damn! There was no suggestions I could give because it’s damn near perfect. I now feel that I had been using the wrong configs all these while. I won’t get into details of what this config does as the J. has already included instructions in the config he wrote.* 
>
> *What I will tell you is that, after a versus L4D2 player for so long being, I give my stamp of awe and approval for his work after testing/using it for a few weeks. Rating this ultimate config 12 outta 10 stars #cantlivewithoutit*

[daemon9s](http://www.steamcommunity.com/profiles/76561198308768316 "daemon9s")

## Preamble
- Many players do not have the basic setup for Left 4 Dead 2 which hinders them from playing well in the competitive servers especially those running on above the default server tick rate of 30
- This config is meant to provide a player with the needed adjustments and also with additional features that assists and optimizes their gameplay
- My goal of sharing this config is to get more players to have the optimal settings configured for this game so that everyone can have a better gaming experience all together

## Backing up current config
1. Go to your Left 4 Dead 2 installation directory `.../Steam/steamapps/common/Left 4 Dead 2/left4dead2/`
2. Create a copy of the folder `cfg` and rename it to `cfg.bak`
3. This will be your backup in the event that you would like to revert back to your original settings
   - Simply delete `cfg` folder and rename `cfg.bak` to `cfg`

## Instructions
 1. Read through the config to understand what is happening
 2. Copy the files and folders into your game directory:
`.../Steam/steamapps/common/Left 4 Dead 2/left4dead2/`
 3. Setup launch options of L4D2: `Right-click Left 4 Dead 2 >> Properties >> Set Launch Options`
  4. Add the following line into the box: `-lv -high +mat_queue_mode 2 +precache_all_survivors 1 -novid -console -noipx -nod3d9ex -nojoy -noforcemaccel -noforcemparms +mat_motion_blur_percent_of_screen_max 0 +clientport 27619`
      - Remove `-lv` if you do not prefer to play in low violence mode
 6. Setup video settings as per given below if you have a potato computer like mine (you may use your higher settings for items in **bold** if you have a beast)

| Setting                     | Value                         | Remarks                                                      |
| --------------------------- | ----------------------------- | ------------------------------------------------------------ |
| Aspect Ratio                | As per your your screen size  |                                                              |
| Resolution                  | As per your native resolution |                                                              |
| Display Mode                | Full screen                   |                                                              |
| **Film Grain Amount**       | None                          | For screen clarity                                           |
| **Anti-Aliasing Mode**      | None                          | No reason to have this enabled. If you have a powerful system, you can set this to max. |
| **Filtering Mode**          | Trilinear                     | No reason to run higher than this                            |
| Wait For Vertical Sync      | Disabled                      | Having VSync enabled locks your FPS to your screen's refresh rate that causes input lag |
| Shader Detail               | Low                           | If you have a powerful system, you can set this to max       |
| Effect Detail               | High                          | This is to ensure that you can see Tank rocks from a distance |
| **Model/Texture Detail**    | Low                           | If you have a powerful system, you can set this to max       |
| Multicore Rendering         | Enabled                       | Uses all available CPU cores for the game                    |
| Paged Pool Memory Available | High                          | More memory is assigned to the game which results in the game loading maps slightly faster |

  7. Launch game and open console and run the following command: `unbindall; exec config_default.cfg; exec autoexec.cfg`
      - Please note that the command above **resets the game config**. All custom binds/mappings **will be removed**. You will have to manually add or change your custom binds/mappings after this command.

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

### helper.cfg

    .../cfg/ultimateconfig/helper.cfg

Typing `help` in console will print out this file that displays all the available commands for quick and easy reference

### config_custom.cfg

    .../cfg/ultimateconfig/config_custom.cfg

Whatever additional config that you want to add should go here. Instead of changing the `ultimateconfig.cfg`, copy the cvar that you want to change and paste it here with the desired value. This is so that in future, it is easier to update these configs.

## Breakdown of ultimateconfig.cfg
### Reset Config [Disabled]
- Reset the game configuration to the default configuration before we make changes

- As it resets the configuration and applies only what is in this config, whatever extra custom config that a user has done manually will not be saved

- Commented out as not everyone know how to deal with this


### General Client Settings
- Just basic client cvars, enabling console, disabling joystick and Steam controller


### Subtitles
- Set up subtitles - quite useful as you can use the dialogues to identify what is happening/going to happen


### Video
- Increase game brightness (adjust the value if the game is too bright)
- Reduce unnecessary animations that eat up few FPS

### Audio
- Disable game music to hear SI better
- Setup audio for clarity


### Mic
- Basic mic setup, nothing fancy


### Network
- Setup network settings for competitive mode


### Rates & Lerps
- Aliases for rates, lerps and interp ratio - extremely useful to change lerp in an instant

### Crosshair
- Setup crosshair to be white with black border (colorblind mode)
- The crosshair is most visible in this mode
- There is also aliases to change crosshair color

### Mouse
- Disabling all sorts of mouse filters to give the game the raw mouse movement


### Keyboard
- A must-have null-cancelling movement script for movement keys


### Glows
- Glows are self-explanatory


### Net Graph
- Displays crucial information of whether the server you are in is having any issues with rates, chokes or loss

### Binds
- Useful binds for competitive modes (do not forget to uncomment the line if you want to use those binds)
- The most useful one is `F5` which is to get rid of those "invisible SI, survivor stuck in saferoom" issues

### Aliases
- Aliases to shorten commands


### Toggles
- Useful toggles


### Server Connect Binds
- Servers in the Asia region has more than one IP to connect to
- For convenience sake, all servers and their alternate IPs are set in aliases so as to join them quickly instead of doing the whole "what is the VPN for this server? Copy-paste-connect" thing
- Read through the aliases to get familiar with the aliases used

### Final Launch Parameters
- Setting up the lerp, rates and interp to use here


### Execute Custom Config
- Any additional settings you added in `config_custom.cfg` will be executed


### Write Changes To Config
- Write the config to the game