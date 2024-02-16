---
layout: default
title: Changelog
nav_order: 5
---

# **Changelog**
{: .text-yellow-300 .fw-500 .text-center .fs-8 .lh-default .no_toc }

## Table of contents
{: .no_toc .text-delta }

- TOC
{:toc}

---

## FUComplete v1.4.0
{: .text-yellow-300 .fw-700 .text-center }

### Enhancements/Additions
{: .text-yellow-300 .fw-700 }

* FUCTool updated
  - Patcher
    * Added PSP Go internal storage support. 
      - ***NOTE:*** only use if placing ISO on PSP Go's internal storage.
  - Config
    * Updated strings to reflect the changes to File Replacer.
    * Added `Guildhall Full Chest (Offline)` and `Guildhall Drink Buff` as toggle-able options.
  - File Replacer
    * Updated File Replacer to deal with the changes to NATIVEPSP, allowing dynamic file sizes.
* [FUComplete Online Config Editor](https://fucomplete.github.io/)
  - You can now edit/generate configuration files via web browser. Supports both 1.3.1 and 1.4.0. (Thanks [SilverJolteon](https://github.com/silverjolteon))
* Modloader rewrite
  - Code cleaned up and moved most of preload outside the main binary, allowing for more control during the preload initialization phase. 
     * All assets related to modloader such as config, code and initial NATIVEPSP generation are all auto generated on game start if the do not exist.
  - Changed directory where modloader assets are stored from `ms0:/FUC` to `ms0:/PSP/SAVEDATA/FUCDAT` to simplify location and ease of management.
  - File size limits removed in NATIVEPSP, now you can load larger files... *within reason.*
* Quality of Life
  - Added hold to gather/carve.
  - Can toggle ON/OFF File Replacer in the Options Menu from Main Menu.
{: .pl-6 }

### Fixed
{: .text-yellow-300 .fw-700 }

* Player could spin in place at chests other than guildhall/room, fixed to only work in guildhall/room.
* The option `Background Loading` if enabled would prevent file replacer from loading modified stages. Disabled and now changed to a `File Replacer` toggle.
{: .pl-6 }

### Notes
{: .text-yellow-300 .fw-700 }

* Really just want to give a shoutout to Kurogami2134 and SilverJolteon...
  - [Kurogami2134](https://github.com/Kurogami2134) for showing his work on PMO export and sending me some example exports to test with... Honestly if they never showed their work I'd probably would have never updated this patch.
  - [SilverJolteon](https://github.com/silverjolteon) for creating the online config editor. I know a lot of people will appreciate it, especially android users.
{: .pl-6 }

---

## FUComplete v1.3.1
{: .text-yellow-300 .fw-700 .text-center }

### Enhancements/Additions
{: .text-yellow-300 .fw-700 }

* FUCTool updated
  - Added early kill lao/shen as a toggle
  - Updated file replacer to be a bit more sane to use.
* When setting save region to JP and starting a new game, it will use the correct region ICON0
{: .pl-6 }

### Fixed
{: .text-yellow-300 .fw-700 }

* Removed extra text that was overflowing the number of players text in the online training hall quest requests selection.
* Some files were getting skipped in file replacer, now fixed.
{: .pl-6 }

---

## FUComplete v1.3.0a (HOTFIX)
{: .text-yellow-300 .fw-700 .text-center }

### Fixed
{: .text-yellow-300 .fw-700 }

* Changing equipment in Farm/Kitchen would break interactions with gathering nodes and kitchen table. Only offline hall can have full chest access now.
{: .pl-6 }

---

## FUComplete v1.3.0
{: .text-yellow-300 .fw-700 .text-center }

### Enhancements/Additions
{: .text-yellow-300 .fw-700 }

* Patcher replaced with `FUCTool`. 
  - New UI based app to handle applying patches, editing the configuration file, setting up file replacer and injecting custom quests into savedata.
* Modloader support added to the game.
  - Added a preloader/loader to allow patching of code and files on boot or when it is called on.
* File replacer _(nativePSP)_.
  - Similar to Monster Hunter World, file replacer allows replacing of individual files stored in the `nativePSP` folder for easier modding. A `file.bin` inside handles a whitelist of files to replace.
* Configuration file support.
  - Allows toggling of patch features that were once either xdelta patches or were cwcheat codes. These options are:
    * File replacer path (`disc0`/`ms0`)
    * Savedata region (`JP`/`NA`/`EU`)
    * Dos Audio
    * True raw/ele/status
    * Field of View 
      - Sets the player FoV in quest, options are `Default`, `Minor`, `Moderate` and `Extreme`
    * Starting vertical camera position
      - Sets vertical camera position, can set the value between 1 (lowest) thru 5 (highest)
    * Minimap scale
      - Similar to the previous CWCheat code, can set minimap size/scale between `Default`, `75%` and `50%`. If `75%` or `50%` are chosen the loading screen minimap will also be scaled down
    * Hunting Horn Rework
      - Hunting horns note mechanics now mimic that of Frontier, where notes only reset on staff if you sheath or have a forced sheathed interaction.
      - Left and right swing MV/KO values have been restored to their F2 levels, 31 MV and 18 KO, up from 27 MV and 15 KO.
      - The hilt jab poke attack now does cutting damage.
* Replaced `Data Install` toggle with a quest bank toggle. This allows you to switch between the built-in event quests or up to 18 custom quests stored on savedata.
* Faster pickup from supply chests.
* Increased draw distance of NPCs in village.
* Can now buy certain items in bulk to chest:
  - Binoculars
  - Powercharm
  - Armorcharm
  - BBQ Spit
* Full chest access in all areas with a chest.
  - Online/Offline hall has a check where if you are offline you have full chest access, and if you are online it's the normal chest.
* Lao-Shan Lung, Ash Lao-Shan Lung and Shen Gaoren quests that are on Fortress have their HP thresholds removed, allowing for pre area 5 kills.
  - Note: If playing with unpatched players, be aware that area host controls HP thresholds. This means if an unpatched player is first to end the area, you will have a vanilla interaction and can't early kill them.
    * TLDR: If you want early kill, make sure you or a patched player are first to enter the areas.
* Status display settings in quest are now persistent between quests.
* Guildhall table now features a drink buff.
  - This gives a flat HP/Stamina boost based on the number of active chefs in your kitchen.
    * HP - Each active chef gives 10 HP.
    * Stamina - Active chefs 1-4 give 25 stamina, with 5 active chefs giving 50 stamina.
* JP region savedata now supported.
* Game `ICON0` replaced so people know the difference between patch and unpatched. _(Thanks Asterisk!)_
{: .pl-6 }

### Fixed
{: .text-yellow-300 .fw-700 }

* Item wheel now matches the same size/position as FU.
* Sharpness indicator and glow now uniform and fixed.
* Guildcard UI elements fixed to avoid string overflows and better alignment of various elements.
  - Note: If your name uses full-width characters it will still likely overflow but its just a visual bug...
* Input delays in equipment shops fixed.
* Various button input and localization string errors fixed.
* Fixed dummied strings to display proper names when using HPD. 
* Guildhall Shop NPC positioning fixed so feet don't clip into the floor.
* Wandering Chef NPC positioning fixed, no longer floats in the air and is more visible on game start.
* Hair preview was not being auto previewed, now fixed.
* Guildcard comments under list now uses the proper OSK.
* Gallery descriptions are now properly aligned. 
* System level messages now display properly in English on PSP/Vita.
* Guildcard send/receive messages fixed and aligned properly.
{: .pl-6 }

### Removed
{: .text-yellow-300 .fw-700 }

* JP language support
  - Might look into adding support back in... but because of the amount of changes, it's removed for now.
* Removed various cwcheat codes as they are now part of the patch.
{: .pl-6 }

---

## FUComplete v1.2.1
{: .text-yellow-300 .fw-700 .text-center }

### Enhancements/Additions
{: .text-yellow-300 .fw-700 }

* Patcher now lets you choose what region save you would like to load.
  - After selecting `en` when prompted for language you can now choose one of the following:
    - `us` if your save is `ULUS10391`
    - `eu` if your save is `ULES01213`
{: .pl-6 }

### Fixed
{: .text-yellow-300 .fw-700 }

* F2 related events were not giving out their respective Japanese exclusive tickets. These quests were:
  - Village *(Elder)*
    * 4★ Hermitaur Buffet
    * 5★ Small Shadow over the Swamp
    * 5★ Congalala Territorial Fight
  - Village *(Nekoht)*
    * 7★ Whack a Shakalaka
    * 9★ Diablos, the Demon King
  - Guildhall
    * 4★ Go Fish Goldenfish! 
    * 5★ Two Little Shadows
    * 5★ A Horde of Congalalas
    * 8★ Two Queens
    * 8★ One-Horned Demon King
    * 8★ Phantasmic Battle
* Guildcard default message had an extra character causing a weird "double space" between 2 words.
* Updated some string translations.
{: .pl-6 }

---

## FUComplete v1.2
{: .text-yellow-300 .fw-700 .text-center }

### Enhancements/Additions
{: .text-yellow-300 .fw-700 }

* Event/Challenge quests now load in a more vanilla manner.
* Bonus DLC checks patched, now it's on by default.
* Auto enable equipment previews in shops.
* Patch is now cross-play compliant. This means modded can post event quests and unmodded can join them.
{: .pl-6 }

### Fixed
{: .text-yellow-300 .fw-700 }

* When playing event quests previously, weapon usage and quest completes on guildcard would not display accurately.
* Quest pages in guildhall would not show as cleared even when all quests are completed.
{: .pl-6 }

### Removed
{: .text-yellow-300 .fw-700 }

* Download and Data Install options are removed from main menu. This is because the Download option is no longer necessary and Data Install is broken.
* Removed crossplay block.
* Removed QInject.
{: .pl-6 }

---

## FUComplete v1.1
{: .text-yellow-300 .fw-700 .text-center }

### Enhancements/Additions
{: .text-yellow-300 .fw-700 }

* Increase quest limit in savedata to 15, up from 6.
* Added all Challenge/Fiesta quests, this means ***all*** 52 quests are now part of the patch. Please use `QInject` to add them to your save.
* New QoL codes 
  * **Guildhall QoL (EMU ONLY)**: Replaces NPC near questboard with smithy menu *(offline)*, Felyne by Treshi now is a new peddler *(online)* and you now have full access to chest features *(offline)*.
  * **True Raw/Ele/Status**: "Debloats" the values on weapons to show their true numbers.
  * **HUD Off Above 40 HP**: A port of a similar P3rd code, hides your HUD when above 40 HP.
  * **Enable Cross-play**: Allows cross-play between vanilla and modded. Please read about compatibilty issues before going online.
* Added PSN version support
* Added JP lang support
{: .pl-6 }

### Fixed
{: .text-yellow-300 .fw-700 }

* Tigrex training exercises now loads the correct quest.
* "Quest Level" now reporting the "★" rank on G1-G3 quests.
* Various text alignements have been addressed.
* Options menu now has proper font scaling and alignment.
* Guildcard "note" now uses up the full width of the box.
* The felyne on your guildcard no longer shares its ears with melynx.
* Save importing another FU save now works.
* New item "!" graphic renders properly.
* Bowgun shells in HUD correctly aligned.
* Palico skill learn/unlearn point cost/return displays proper value.
* "Dropping" a carryable now displays the correct message.
* Minimap rescale code has the "monster ping" correctly aligned with the map.
{: .pl-6 }

### Removed
{: .text-yellow-300 .fw-700 }

* The "Quest Victory" and "Seen" audio have been reverted to their original counterparts. They may make a return later but for now are removed from the `DosAudio` patch.
{: .pl-6 }

---

## FUComplete v1.0
{: .text-yellow-300 .fw-700 .text-center }

* Initial release of FUComplete patch.
{: .pl-6 }
