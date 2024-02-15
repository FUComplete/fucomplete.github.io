---
layout: default
title: FAQ
nav_order: 3
---

# FAQ
{: .text-yellow-300 .fw-500 .text-center .fs-8 .lh-default .no_toc }

## Table of contents
{: .no_toc .text-delta }

- TOC
{:toc}

---

### How do I apply the patch? What do I need?
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

---

### Why use Portable 2nd G as a base and not Freedom Unite? 
{: .text-yellow-300 .fw-700 .lh-default .pb-4 }

Due to issues with finding translators for the various langauges and having memory limit issues, it was decided to move to Portable 2nd G as I didn't have to worry about more than one language and I had significantly more memory to play with.

---

### Is this allowed on Hunsterverse?
{: .text-yellow-300 .fw-700 .lh-default .pb-4 }

Yes, it's allowed.

<img src="/assets/images/hv_approved.png">

<a href="https://discord.com/channels/288170871908990976/541678672113958922/1207710203684978739" target="_blank">From MightyZack himself.</a>

---

### What are the default settings of `CONFIG.BIN`?
{: .text-yellow-300 .fw-700 .lh-default .pb-4 }

Default settings are as follows:
```
File replacer:                  Disabled 
Save Region:                    ULUS10391
True Raw/Ele/Stat:              Disabled 
Dos Audio:                      Disabled 
Field of View:                  Default  
Vert Cam Start Pos:             Default  
Minimap Scale:                  Default  
HH Tweak:                       Disabled 
Early Lao/Shen Kill:            Disabled 
Guildhall Full Chest (Offline): Disabled 
Guildhall Drink Buff:           Disabled 
```
{: .lh-tight }

---

### So I've updated my config, Where does `CONFIG.BIN` go?
{: .text-yellow-300 .fw-700 .lh-default .pb-4 }

Go to your `SAVEDATA` and locate the folder named `FUCDAT`, copy over and overwrite the old `CONFIG.BIN` with your updated one.

```
  .
  └───PSP
      └───SAVEDATA
          ├───FUCDAT
          │   └───CONFIG.BIN
          ├───ULES01213
          ├───ULUS10391
          └───ULJM05500
```
{: .lh-0 }

---

### When I run the game on my PSP/Vita, village lags/runs slow... how do I fix this?
{: .text-yellow-300 .fw-700 .lh-default .pb-4 }

* Please set your CPU clock speed to `333/166` by pressing `Select` at VSH menu and changing the option `CPU CLOCK GAME` to `333/166`. 

| <img src="/assets/images/vsh_menu.png"> |
|:---:|
| VSH Menu |

---

### Why do my quest files not show up on FUCTool?
{: .text-yellow-300 .fw-700 .lh-default .pb-4 }

Quest files must be either `.mib` or `.pat` and have to be **decrypted**. 

---

### Why do I get "Old savedata detected" on PPSSPP after adding/removing quests from save? Does it cause any problems?
{: .text-yellow-300 .fw-700 .lh-default .pb-4 }

1. It won't cause problems, once you save in-game the error message will go away.
2. SED is used to handle the encryption side of things which seems to use an older method of save encryption.
