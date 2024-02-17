---
layout: default
title: Setup
nav_order: 2
has_children: true
has_toc: false
---

# Setup
{: .text-yellow-300 .fw-500 .text-center .fs-8 .lh-default .no_toc }

---

### Step 1: Download latest build of FUComplete
{: .text-yellow-300 .fw-700 }

1. Download the latest patch from [here](https://github.com/FUComplete/Patch/releases/latest). You only need to download the `FUComplete_*.zip` file where `*` is the version number.
2. Once downloaded, extract the zip to a folder. Keep note of where this folder is for the next steps.
{: .pl-6 }

---

### Step 2: Obtaining the ISO
{: .text-yellow-300 .fw-700 }

![SetupLogo](/assets/images/setup_pspgame.png)
{: .pb-8 }

### Requirements:
{: .text-yellow-300 .fw-700 }

* A PSP with Custom Firmware
* *At least* a 1GB Memory Stick
* Monster Hunter Portable 2nd G
* A USB cable to transfer
* PSP Filer v6.6 ([Download](https://archive.org/download/filer6.6/filer6.6.zip))
{: .pl-6 .pb-2 }

#### Copy PSP Filer to PSP
{: .text-yellow-300 .fw-700 }

1. Extract PSP Filer zip to a folder and open the `release/GAME` folder and copy the `Filer` folder.
2. Connect your PSP to the computer using the USB cable.
3. Open your memory stick, and paste the `Filer` folder to `PSP/GAME`.
4. Disconnect your PSP from the computer.
{: .pl-6 }

#### Dumping UMD (PSP Filer) 
{: .text-yellow-300 .fw-700 }

1. Launch `PSP Filer` on your PSP.
2. Once in `PSP Filer`, Press the triangle button to open a menu, then press right trigger button to start `UMD ripping`.
3. It will pull up a keyboard with the name `ULJM-05500.iso` in the text field. If you wish to rename it do so now, otherwise press `Start` to start dumping.
4. Once you see the message `ripping completed` you can press X to resume and exit PSP Filer.
{: .pl-6 }

| <a href="/assets/images/pspfiler_1.png" target="_blank"><img src="/assets/images/pspfiler_1.png"></a> | <a href="/assets/images/pspfiler_2.png" target="_blank"><img src="/assets/images/pspfiler_2.png"></a> |
|:---:|:---:|
| Open menu with `Triangle`<br>and press `R Trigger`. | Set ISO name and press<br>`Start` to begin dumping. |
| <a href="/assets/images/pspfiler_3.png" target="_blank"><img src="/assets/images/pspfiler_3.png"></a> | <a href="/assets/images/pspfiler_4.png" target="_blank"><img src="/assets/images/pspfiler_4.png"></a> |
| Let it finish dumping... | Finished dumping. |

#### Copy ISO to PC
{: .text-yellow-300 .fw-700 }

1. Connect your PSP to the computer using the USB cable.
2. Open your memory stick, go to `ISO` folder and transfer your dumped ISO to your computer.
3. Disconnect the PSP from the computer.
{: .pl-6 }

{: .note }
After copying the ISO to your computer, you can check to make sure it dumped properly by making sure it matches this md5 checksum: `1f76ee9ccbd6d39158f06e6e5354a5bd`

---

### Step 3: Patching the ISO
{: .text-yellow-300 .fw-700 }

1. Go to the folder that you extracted in [Step 1](#step-1-download-latest-build-of-fucomplete) and launch `FUCTool.exe`. It should open up on the `Patcher` tab.
2. Press the `Select` button and select the ISO you transfered to your computer from [Step 2](#step-2-obtaining-the-iso). You should see the following:
    
    ```
    INFO | Checking ISO...
    INFO | Valid ISO file.
    ```
    {: .lh-0 }
Your ISO is ready for patching.
    
    {: .note }
    >If you see this when you select your ISO:
    >```
    >INFO | Checking ISO...
    >ERROR | Invalid ISO, your dump should match one of the following md5 hashes:
    >ERROR | UMD: 1f76ee9ccbd6d39158f06e6e5354a5bd
    >ERROR | PSN: cc39d070b2d2c44c9ac8187e00b75dc4
    >```
    >{: .lh-0 }
    > Please go back to [Step 2](#step-2-obtaining-the-iso) and redump your UMD and validate that the ISO matches the UMD hash or if you dumped your PSN copy to ISO make sure it matches the PSN hash.
3. There are 2 checkboxes that can be ticked before applying the patch:
    1. `Keep patched DATA.BIN outside of the ISO (for modders).`
        - Tick this option if you plan to edit files or develop mods.
    2. `PSP Go internal storage remapping (PSP Go only).`
        - Tick this option **ONLY**{: .text-red-000 } if you plan to install the ISO onto PSP Go's internal memory.<br>**DO NOT**{: .text-red-000 } enable this if you plan to install the game anywhere else.
4. Once you have decided, press the `Patch ISO` button to begin patching. Please note that it can take a while.
5. You will know that patching is done when you see `Patching done` and will say where the ISO is located with `_FUC` added at the end of the filename.
{: .pl-6 }

| <a href="/assets/images/fuctool_patching.png" target="_blank"><img src="/assets/images/fuctool_patching.png" width="75%"></a> |
|:---:|
| Patching done. |

---

### Step 4: Start the game!
{: .text-yellow-300 .fw-700 .pb-2 }

Now with the game patched, you should at least boot the game once to generate all the necessary base mod files and config in SAVEDATA.

| <a href="/assets/images/mod_savedata.png" target="_blank"><img src="/assets/images/mod_savedata.png" width="75%"></a> |
|:---:|
| After booting the game once you should see `FUComplete Config and Mods` savedata present |

Afterwards, you can start the process of [adjusting your config](/docs/fuctool/config.html), [make use of file replacer to load additional mods](/docs/fuctool/file_replacer.html) and [injecting custom quests to play](/docs/fuctool/custom_quests.html). 
