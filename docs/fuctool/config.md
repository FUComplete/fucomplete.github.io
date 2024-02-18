---
layout: default
title: Configuration
nav_order: 1
parent: Setup
---

# Configuration
{: .text-yellow-300 .fw-500 .text-center .fs-8 .lh-default .no_toc }

{: .warning }
>Please make sure you boot the game at least **once** to generate the necessary base files as mentioned in [Step 4](/docs/setup.html#step-4-start-the-game) of Setup.

## Table of contents
{: .no_toc .text-delta }

- TOC
{:toc}

---

## Updating `CONFIG.BIN`
{: .text-yellow-300 .fw-700 .text-center }
<br>

When the game loads, it reads your configuration file (`CONFIG.BIN`) and applies the various features/QoL based on what you set.

There are 2 ways to edit your `CONFIG.BIN`:

* FUCTool's Config Editor
* [FUComplete Online Config Editor](/assets/config_editor.html)
{: .pl-6 }

| <a href="/assets/images/fuctool_config.png" target="_blank"><img src="/assets/images/fuctool_config.png"></a> | <a href="/assets/images/foce_config.png" target="_blank"><img src="/assets/images/foce_config.png"></a> |
|:---:|:---:|
| FUCTool Config Editor | FUComplete Online Config Editor |

Once you are happy with your settings, press `Save` and copy your new `CONFIG.BIN` to `FUCDAT` in SAVEDATA. 

{: .note }
Please see [So I’ve updated my config, Where does `CONFIG.BIN` go?](/docs/faq.html#so-ive-updated-my-config-where-does-configbin-go) if you are still unsure where to place it.

Below explains what each option does as well as what the default setting is.

---

## Options
{: .text-yellow-300 .fw-700 .text-center }

### File Replacer
{: .text-yellow-300 .fw-700 .pb-2 }

**When enabled:** Allows loading of modded files from `NATIVEPSP`. This is also toggleable in-game from `Main Menu` under `Options`. For more information on how to use this feature fully, please see the [File Replacer](/docs/fuctool/file_replacer.html) section.

**Default is `Disable`**

---

### Save Region
{: .text-yellow-300 .fw-700 .pb-2 }

Sets what region save should be loaded, so you can continue using your existing save with the patch.

* `ULJM05500` - Monster Hunter Portable 2nd G (JP) save
* `ULUS10391` - Monster Hunter Freedom Unite (NA) save
* `ULES01213` - Monster Hunter Freedom Unite (EU) save
{: .pl-6 }

**Default is `ULUS10391`**

---

### True Raw/Ele/Status Display
{: .text-yellow-300 .fw-700 .pb-2 }

**When enabled:** Shows the "true" values of a weapons raw, element and status.

| <a href="/assets/images/config_editor/true_raw_d.png" target="_blank"><img src="/assets/images/config_editor/true_raw_d.png"></a> | <a href="/assets/images/config_editor/true_raw_e.png" target="_blank"><img src="/assets/images/config_editor/true_raw_e.png"></a> |
|:---:|:---:|
| Disabled | Enabled |

This is purely visual and removes the need to calculate the true values of a weapon.

**Default is `Disable`**

---

### Dos Audio
{: .text-yellow-300 .fw-700 .pb-2 }

**When enabled:** Replaces various battle themes with their Dos counterparts. 

These themes are:

* [Jungle](https://youtu.be/wP1Tiq74gWs)
* [Desert](https://youtu.be/Hjf1QfiTBbY)
* [Swamp](https://youtu.be/ZRQT-QYB0_I)
* [Snowy Mountain](https://youtu.be/7T0Vp7okMhE)
* [Volcano](https://youtu.be/vHSCNxTjX1c)
* [Tower](https://youtu.be/f5ZNBm9EuEc)
{: .pl-6 }

**Default is `Disable`**

---

### Field of View
{: .text-yellow-300 .fw-700 .pb-2 }

Allows adjusting your *viewport* or how much of the games *"world"* you can see.

| <a href="/assets/images/FoV.webp" target="_blank"><img src="/assets/images/FoV.webp"></a> |
|:---:|
| Default - Minor - Moderate - Extreme |

**Default is `Default`**

---

### Starting Vertical Camera Position
{: .text-yellow-300 .fw-700 .pb-2 }

Sets the starting vertical camera position when you embark on a quest.

| <a href="/assets/images/vert_cam_setting.webp" target="_blank"><img src="/assets/images/vert_cam_setting.webp"></a> |
|:---:|
| 1 (Lowest) - 2 - 3 - 4 (Default) - 5 (Highest) |

**Default is `4 (Default)`**

---

### Minimap Size
{: .text-yellow-300 .fw-700 .pb-2 }

Sets a scaling modifier for minimap size. If either 75% or 50% are selected the loading screen map is also scaled down.

| <a href="/assets/images/Minimap.webp" target="_blank"><img src="/assets/images/Minimap.webp"></a> |
|:---:|
| Default - 75% - 50% |

**Default is `Default`**

---

### Hunting Horn Tweak
{: .text-yellow-300 .fw-700 .pb-2 }

**When enabled:** Have modified Hunting Horn mechanics with the following changes:

* Note mechanics work similar to Frontier, where notes only clear if you sheath your weapon or have a forced sheathed interaction.
* Left and right swing MV/KO values increased to match P2/F2 values. 31 MV and 18 KO, up from 27 MV and 15 KO.
* Hilt jab poke attack now does cutting damage instead of impact.
{: .pl-6 }

**Default is `Disable`**

---

### Early kill /LaoShen (Fortress)
{: .text-yellow-300 .fw-700 .pb-2 }

**When enabled**: Lao-Shan Lung, Ash Lao-Shan Lung and Shen Gaoren quests that are on Fortress have their HP thresholds removed, allowing for pre area 5 kills.

{: .note }
If you play with unpatched players and want the early kill, make sure **you or another patched player** are the first to enter areas. This is because area host is in control of the HP mechanics.

**Default is `Disable`**

---

### Guildhall Full Chest (Offline)
{: .text-yellow-300 .fw-700 .pb-2 }

**When enabled:** Allows changing equipment in the Guildhall item chest.

{: .note}
This only works **OFFLINE**

**Default is `Disable`**

---

### Guildhall Drink Buff
{: .text-yellow-300 .fw-700 .pb-2 }

**When enabled**: Can get a quick Health and Stamina boost without leaving the Guildhall, based on how many active Felyne Chefs you have working in your kitchen.

* For each active chef in your kitchen:<br>Receive +10 max Health (max +50 at 5 chefs)
* For 1-4 active chef in your kitchen:<br>Receive +25 max Stamina (max +50 at 5 chefs)
{: .pl-6 }

**Default is `Disable`**
