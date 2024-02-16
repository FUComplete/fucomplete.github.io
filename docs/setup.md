---
layout: default
title: Setup
nav_order: 2
---

# Setup
{: .text-yellow-300 .fw-500 .text-center .fs-8 .lh-default .no_toc }

---

### Step 1: Download latest build of FUComplete
{: .text-yellow-300 .fw-700 .pb-2 }

1. Download the latest patch from [here](https://github.com/FUComplete/Patch/releases/latest).
2. Once downloaded, extract the zip to a folder. Keep note of where this folder is for the next steps.
{: .pl-6 }

---

### Step 2: Obtaining the ISO
{: .text-yellow-300 .fw-700 }

![SetupLogo](/assets/images/setup_pspgame.png)

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

---

### Step 3: Patching the ISO
{: .text-yellow-300 .fw-700 }

<!-- ### How do I apply the patch? What do I need?
{: .text-yellow-300 .fw-700 .lh-default .pb-4 }

{: .note }
> Please make sure that your copy of **Monster Hunter Portable 2nd G** matches one of the following md5 hashes:
> ```
> UMD: 1f76ee9ccbd6d39158f06e6e5354a5bd
> PSN: cc39d070b2d2c44c9ac8187e00b75dc4
> ```
> {: .lh-tight }

Make sure you use either a UMD dump or PSN version of **Monster Hunter Portable 2nd G** and download the [latest release](https://github.com/FUComplete/Patch/releases/latest)... extract the zip file into a folder.

Run `FUCTool`, it should be on the "Patcher" tab. Press the `Select` button and select your ISO, it'll check to make sure the ISO is valid and will be ready to patch.

There are 2 checkboxes you can tick:
1. `Keep patched DATA.BIN outside of the ISO (for modders).`
  - Tick this option if you plan to edit files or develop mods.
2. `PSP Go internal storage remapping (PSP Go only).`
  - Tick this option **ONLY**{: .text-red-000 } if you plan to install the ISO onto PSP Go's internal memory. **DO NOT**{: .text-red-000 } enable this if you plan to install the game anywhere else.

Once you've decided, press the `Patch ISO` button. Once done you should see a `Patching done` message as well as where the patched image is saved.

---

### I don't have a PC, can I apply the patch on Android? 
{: .text-yellow-300 .fw-700 .lh-default .pb-4 }

There is no Android native version of `FUCTool`... so no, you will need a PC to apply the patch.

--- -->