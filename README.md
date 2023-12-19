# Ultimate L4D2 Config (autoexec) by J.

* [Disclaimer](#disclaimer)
* [Preamble](#preamble)
* [Backing up current config](#backing-up-current-config)
* [Instructions](#instructions)
* [Reviews](#reviews)
* [Acknowledgments / Gratitude / Attribution](#acknowledgments--gratitude--attribution)

## Disclaimer

- This configuration has undergone extensive testing over the years with numerous players, consistently proving its utility.
- Please note that the provided configuration is offered "AS IS" without any warranty.
- Given that the configuration makes significant changes to various [cvars](https://developer.valvesoftware.com/wiki/List_of_L4D2_Cvars) in the game, it's advisable to create your own backup if you wish to revert to your previous setup.
- Keep in mind that individual experiences with the configuration may vary.

## Preamble
- Numerous players face challenges in Left 4 Dead 2 due to lacking the essential setup, thereby impacting their performance on competitive servers, particularly those operating at tick rates beyond the default 30.
- This config is designed to equip players with the necessary adjustments and additional features, enhancing their gameplay experience by offering assistance and optimization.
- By sharing this config, my objective is to encourage more players to adopt optimal settings for the game, fostering a collective improvement in everyone's gaming experience.

## Backing up current config
1. Navigate to your Left 4 Dead 2 installation directory located at `.../Steam/steamapps/common/Left 4 Dead 2/left4dead2/`.
2. Right-click on the 'cfg' folder and select `Send to >> Compressed (zipped) folder`.
3. This compressed folder serves as your backup should you wish to return to your original settings:
   - To revert, delete the current `cfg` folder, then extract the zipped `cfg` folder back into the directory mentioned in step 1.
   - Launch your game, and your settings will be restored to their previous configuration.

## Instructions
1. **Read through each config file to understand what is happening**
2. Copy the files and folders into your game directory located at: `.../Steam/steamapps/common/Left 4 Dead 2/left4dead2/`.

3. Configure Left 4 Dead 2 launch options: Right-click `Left 4 Dead 2` >> `Properties` >> `Set Launch Options`.
4. Input the following line into the box: `-lv -novid -console -useforcedmparms -noforcemaccel -noforcemspd +clientport 27666`.
   - Optionally, omit `-lv` if you prefer not to play in low violence mode.
5. Adjust video settings based on the specifications below, especially if your computer has performance constraints (utilize higher settings for items in **bold** if you have a powerful system).
6. An informative Reddit post delves into the impact of each setting on FPS, offering insights for customizing your preferences. Refer to the detailed article [here](https://www.reddit.com/r/l4d2/comments/vmhq82/left_4_dead_2_performance_guide_2022/).

| Setting                     | Value                         | Remarks                                                      |
| --------------------------- | ----------------------------- | ------------------------------------------------------------ |
| Aspect Ratio                | As per your screen size  |                                                              |
| Resolution                  | As per your native resolution |                                                              |
| Display Mode                | Full screen                   |                                                              |
| **Film Grain Amount**       | None                          | For screen clarity.                                          |
| **Anti-Aliasing Mode**      | None                          | No reason to have this enabled. If you have a powerful system, you can set this to max. |
| **Filtering Mode**          | Trilinear                     | No reason to run higher than this.                           |
| Wait For Vertical Sync      | Disabled                      | Having VSync enabled locks your FPS to your screen's refresh rate that causes input lag. |
| **Shader Detail**           | Low                           | If you have a powerful system, you can set this to max.      |
| Effect Detail               | High                     | This is to ensure that you can see Tank rocks from a distance. Render max distance possible. |
| **Model/Texture Detail**    | Low                           | If you have a powerful system, you can set this to max.      |
| **Multicore Rendering**     | Enabled                       | Uses all available CPU cores for the game (Disable this if you have an old computer or facing FPS issues even with this config). |
| Paged Pool Memory Available | High                          | More memory is assigned to the game, which results in the game loading maps slightly faster. If your system is running out of RAM, reduce this value. |

7. Launch the game and access the console, then execute the command: `exec config_default.cfg; exec autoexec.cfg`.
   - It's crucial to recognize that this command **resets the game configuration**, leading to the **removal of all custom binds and mappings**. You'll need to add/modify your custom binds and mappings manually post-execution.

8. Modify any bindings that are manually set (such as altering the zoom key, changing the crouch key, etc.) in the game settings.

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

## Acknowledgments / Gratitude / Attribution
The development of this configuration draws inspiration from various other configurations and valuable input provided by community members. Their collective contributions have played a pivotal role in shaping and refining this configuration into its current state.

**Distinctive Contributions**
- Derpduck ([SI Color Correction](https://steamcommunity.com/sharedfiles/filedetails/?id=830201245))
- Urik ([Font](https://steamcommunity.com/workshop/filedetails/?id=279970909))

**Inspiration and Adaptation**

- asfn
- baka
- blade
- brunnerh
- bunnerh
- canadarox
- CarnageHeart
- Cedric
- dawkins
- dieckmann215
- don
- draxios
- eram
- erza
- fakiyo
- fig newtons'
- grizz
- hfmkwi
- infested_soul
- Kaizen
- kekkeri
- linfosoma
- ljboi
- m0de
- mason
- MatthewClair
- MeBad
- Midnight_Studios
- miu
- mystrdat
- ningning
- nova.
- prodigysim
- prsto
- purple
- pushpop
- shade
- simi
- Sir
- speshul
- Xbye
- xclusionnl
- zeon
- =[SFS]= def+1 -TPF- a.k.a. =[SFS]= rokkit lawnchair -TPF-
- [AoC] Revalks L4D Script

**Testers/Thank Yous**

- alexander
- anna
- Boomer
- bubba
- Chatic Good
- Daemon9s
- Dec
- Ervi
- FBoyz Clan
- Kirvi
- Kiwi
- ma0o0o
- Maverick
- Max ღ
- Maxines
- Mr. Pink
- purps
- Scar
- Target
- TASbot

**Special Thanks**

- AlliedModders
- ChatGPT
- GameBanana
- Github
- Google
- L4D Community Autoexec
- L4Dnation
- Left4Dead Fandom
- markdown-toc
- PCGamingWiki
- StackEdit