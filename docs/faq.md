---
layout: default
title: FAQ
nav_order: 4
---

# FAQ
{: .text-yellow-300 .fw-500 .text-center .fs-8 .lh-default .no_toc }

## Table of contents
{: .no_toc .text-delta }

- TOC
{:toc}

---

### Why use Portable 2nd G as a base and not Freedom Unite? 
{: .text-yellow-300 .fw-700 .lh-default .pb-4 }

Due to issues with finding translators for the various languages and having memory limit issues, it was decided to move to Portable 2nd G as I didn't have to worry about more than one language and I had significantly more memory to play with.

---

### Does this work on a PSP/Vita or is this emulator only? 
{: .text-yellow-300 .fw-700 .lh-default .pb-4 }

FUComplete is fully compatible with real hardware. As such there are no "emulator only" features.

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

{: .note }
This implies you are on a **Custom Firmware** (CFW) on a PSP or running **Adrenaline** on a Vita.

Please set your CPU clock speed to `333/166` by pressing `Select` at VSH menu and changing the option `CPU CLOCK GAME` to `333/166`. 

| <a href="/assets/images/vsh_menu.png" target="_blank"><img src="/assets/images/vsh_menu.png" width="75%"></a> |
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
2. `SED` is used to handle the encryption side of things which seems to use an older method of save encryption.
