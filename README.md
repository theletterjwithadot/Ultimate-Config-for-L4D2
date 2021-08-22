# Ultimate L4D2 Config (autoexec) by J.

- [Disclaimer](#disclaimer)
- [Preamble](#preamble)
- [Backing up current config](#backing-up-current-config)
- [Instructions](#instructions)
- [The files](#the-files)
  - [autoexec.cfg](#autoexeccfg)
  - [ultimateconfig.cfg](#ultimateconfigcfg)
  - [config_custom.cfg](#config_customcfg)
  - [helper.cfg](#helpercfg)
  - [binds_config.cfg](#binds_configcfg)
  - [binds_pressed.cfg](#binds_pressedcfg)
  - [binds_unpressed.cfg](#binds_unpressedcfg)
  - [CSGO Font w Console](#csgo-font-w-console)
  - [Color Correction](#color-correction)
- [Reviews](#reviews)

## Disclaimer

- The config has been tested for years with multiple players and has proven to be very useful
- The config here is given "AS IS" with no warranty
- The config changes quite a handful of [cvars](https://developer.valvesoftware.com/wiki/List_of_L4D2_Cvars) in the game as such, please perform your own backup if you would like to rollback to your previous config
- Individual's mileage may vary

## Preamble
- Many players do not have the basic setup for Left 4 Dead 2 which hinders them from playing well in the competitive servers especially those running on above the default server tick rate of 30
- This config is meant to provide a player with the needed adjustments and also with additional features that assists and optimizes their gameplay
- My goal of sharing this config is to get more players to have the optimal settings configured for this game so that everyone can have a better gaming experience all together

## Backing up current config
1. Go to your Left 4 Dead 2 installation directory `.../Steam/steamapps/common/Left 4 Dead 2/left4dead2/`
2. Right-click `cfg` folder and click `Send to >> Compressed (zipped) folder`
3. This will be your backup in the event that you would like to revert back to your original settings
   - Simply delete `cfg` folder and extract the zipped `cfg` folder

## Instructions
 1. **Read through each config file to understand what is happening**
 2. Copy the files and folders into your game directory:
`.../Steam/steamapps/common/Left 4 Dead 2/left4dead2/`
 3. Setup launch options of L4D2: `Right-click Left 4 Dead 2 >> Properties >> Set Launch Options`
  4. Add the following line into the box: `-lv -noborder -high +mat_queue_mode 2 +precache_all_survivors 1 -novid -console -noipx -nod3d9ex -nojoy -noforcemaccel -noforcemparms +mat_motion_blur_percent_of_screen_max 0 +clientport 27619`
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
      - Please note that the command above **resets the game config**. **All custom binds/mappings will be removed**. You will have to manually add or change your custom binds/mappings after this command.

 8. Change any binding that you do manually (like binding different key to zoom, changing crouch key, etc) in the game settings

## The files

### autoexec.cfg
    .../cfg/autoexec.cfg
The `autoexec.cfg` runs a command that is needed to make the CSGO Font addon to work. Ensure that you change the resolution in

> alias reloadfont "mat_setvideomode **1920 1080** 1; mat_setvideomode **1920 1080** 0"

to match your resolution. It is also where the `ultimateconfig.cfg` is called to be executed.

### ultimateconfig.cfg
    .../cfg/ultimateconfig/ultimateconfig.cfg
This is where the rest of the magic happens.

### config_custom.cfg

    .../cfg/ultimateconfig/config_custom.cfg

Whatever additional config that you want to add should go here. Instead of changing the `ultimateconfig.cfg`, copy the cvar that you want to change and paste it here with the desired value. This is so that in future, it is easier to update these configs.

### helper.cfg

    .../cfg/ultimateconfig/additional_files/helper.cfg

Typing `help` in console will print out this file that displays all the available commands for quick and easy reference.

### binds_config.cfg

    .../cfg/ultimateconfig/additional_files/binds_config.cfg

Main file that handles dynamic binds. Comment out the execution line in `ultimateconfig.cfg` if you do not wish to use this (right at the bottom).

### binds_pressed.cfg

    .../cfg/ultimateconfig/additional_files/binds_pressed.cfg

These are the binds when ALT key is pressed. These are binds that I made as i have to say these frequently. You can change this as to how you want. Each bind basically has 5 different sentences (thus "dynamic binds").

### binds_unpressed.cfg

    .../cfg/ultimateconfig/additional_files/binds_unpressed.cfg

These are the binds when ALT key is not pressed. These are binds that I made as i have to say these frequently. You can change this as to how you want. Each bind basically has 5 different sentences (thus "dynamic binds").

### CSGO Font w Console 

    .../addons/CSGO Font.vpk

A font pack that makes the game menu and texts cleaner also also enlarges console text to make it more readable than the default font size.

### Color Correction

    .../materials/correction/ghost.pwl.raw
    .../materials/correction/ghost.raw
    .../materials/correction/infected.pwl.raw
    .../materials/correction/infected.raw

These files adjust the orange and blue tint for Special Infected, making it lighter. Credits to [Derpduck](http://www.steamcommunity.com/profiles/76561198038478485) for creating these files.

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
