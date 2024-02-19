---
layout: default
title: What's Changed
nav_order: 3
---

<!-- <span class="label" style="background-color: #2c84fa; color: white;">Config</span> -->
<!-- <span class="label" style="background-color: #7253ed; color: white;">Config</span> -->

# What's Changed?
{: .text-yellow-300 .fw-500 .text-center .fs-8 .lh-default .no_toc }

{: .note}
Anything with <span class="label" style="background-color: #7253ed; color: white;">Config</span> next to it means it is a configurable option. See [Configuration](/docs/fuctool/config.html) for more details.

## Table of contents
{: .no_toc .text-delta }

- TOC
{:toc}

---

### Features:
{: .text-yellow-300 .fw-700 .pb-2 }

* The 38 events and 14 challenges are now built into the game. Savedata quest store limit has been raised to 18, up from 6.
* The option to toggle `Data Install` now has a new function: It now allows switching between the integrated event quests and any custom quests added to savedata.
* The option to toggle `Background Loading` now has a new function: It now switches `File Replacer` ON/OFF.
* All Bonus DLC are enabled by default.
* Easily switch between what region save to load. <span class="label" style="background-color: #7253ed; color: white;">Config</span>
* Auto equipment previews in shops enabled by default without the requirement of a data install.
* Mod support via Modloader, allowing for things such as:
    * Configurable settings via the `CONFIG.BIN`.
    * `File Replacer` allowing loading of modded files from `NATIVEPSP` (think of it like nativePC from Monster Hunter World).
    * Can easily update/extend modloader code.
    * All data consolidated into its own mod savedata.
* Able to buy in bulk to chest the Binoculars, Powercharm, Armorcharm and BBQ Spit. Useful for decoration crafting.
* Can switch between Freedom Unite battle themes and Dos battle themes. <span class="label" style="background-color: #7253ed; color: white;">Config</span>
* ICON0 updated so you can easily tell the difference between patched/unpatched.
{: .pl-6 .lh-tight }

### Quality of Life:
{: .text-yellow-300 .fw-700 .pb-2 }

* Guildhall table now has a *"drink buff"*. - Can get a quick Health and Stamina boost without leaving the Guildhall, based on how many active Felyne Chefs you have working in your kitchen. Press `Circle` to activate while sitting at the table. <span class="label" style="background-color: #7253ed; color: white;">Config</span>
    * For each active chef in your kitchen:<br>Receive +10 max Health (max +50 at 5 chefs)
    * For 1-4 active chefs in your kitchen:<br>Receive +25 max Stamina (max +50 at 5 chefs)
* You can change your equipment in the Offline Guildhall. <span class="label" style="background-color: #7253ed; color: white;">Config</span>
* Faster pickup speed from supply chests.
* Display true raw/element/status of weapons. <span class="label" style="background-color: #7253ed; color: white;">Config</span>
* Adjustable Field of View. <span class="label" style="background-color: #7253ed; color: white;">Config</span>
* Set starting vertical camera position. <span class="label" style="background-color: #7253ed; color: white;">Config</span>
* Adjust minimap scale. <span class="label" style="background-color: #7253ed; color: white;">Config</span>
* Can hold the button to gather/carve. 
{: .pl-6 .lh-tight }

### Gameplay/Mechanic:
{: .text-yellow-300 .fw-700 .pb-2 }

* Any quest with Lao-Shan Lung, Ash Lao-Shan Lung or Shen Gaoren on Fortress have their HP thresholds removed, allowing for a pre area 5 kill. <span class="label" style="background-color: #7253ed; color: white;">Config</span>
* Hunting Horn Tweaks rework the weapon slightly to make it more approachable and rebuff it back to P2/F2 levels. <span class="label" style="background-color: #7253ed; color: white;">Config</span>
  - Note mechanics work similar to Frontier, where notes only clear if you sheath your weapon or have a forced sheathed interaction.
  - Left and right swing MV/KO values increased to match P2/F2 values. 31 MV and 18 KO, up from 27 MV and 15 KO.
  - Hilt jab poke attack now does cutting damage instead of impact.
{: .pl-6 .lh-tight }

### Fixes:
{: .text-yellow-300 .fw-700 .pb-2 }

* Fixed various localization errors and updated menus to match.
* Adjusted item wheel to match FU
* Sharpness indicator and glow now uniform and fixed.
* Fixed draw region of the "!" sprite to display properly.
* Felyne on guildcard no longer has melynx ears.
* Bowgun shells in HUD are now correctly aligned.
* Guildcard elements fixed to avoid string overflows and better alignment.
* Status display settings (the settings for enabling/disabling HUD in quest) are now persistent between quests.
* Guildhall Shop NPC position fixed, feet no longer clip through the floor and now has a shadow.
* Wandering Chef NPC position fixed, no longer floats in the air and is more visible on game start.
* Dummied strings for non-monsters now display properly when using HPD hack.
{: .pl-6 .lh-tight }
