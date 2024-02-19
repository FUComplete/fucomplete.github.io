---
layout: default
title: File Replacer
nav_order: 2
parent: Setup
---

# File Replacer
{: .text-yellow-300 .fw-500 .text-center .fs-8 .lh-default .no_toc }

## Table of contents
{: .no_toc .text-delta }

- TOC
{:toc}

---

## Setting up Mods
{: .text-yellow-300 .fw-700 .text-center }
<br>

In the folder where you extracted the zip from [Step 1](/docs/setup.html/#step-1-download-latest-build-of-fucomplete), copy your mods to the `mods` folder. 

Open `FUCTool` and go to the `File Replacer` tab, you should see your mods listed in the table below.

{: .note }
If you do not see your mods listed, please make sure the files are correctly name, the files are **case sensitive**.

If your mods are listed correctly, press the `Generate NATIVEPSP` button to generate the folder. This folder will need to be copied to the `FUCDAT` folder located in your SAVEDATA

```
  .
  └───PSP
      └───SAVEDATA
          ├───FUCDAT
          │   └───NATIVEPSP
          ├───ULES01213
          ├───ULUS10391
          └───ULJM05500
```
{: .lh-0 }



| <a href="/assets/images/fuctool_mods1.png" target="_blank"><img src="/assets/images/fuctool_mods1.png"></a> | <a href="/assets/images/fuctool_mods2.png" target="_blank"><img src="/assets/images/fuctool_mods2.png"></a> |
|:---:|:---:|
| Copy mods to `mods` folder, you should see them in the table below | Press `Generate NATIVEPSP` and you should have a `NATIVEPSP` folder ready to place in `FUCDAT`. |

---

## Enabling Mods
{: .text-yellow-300 .fw-700 .text-center }
<br>

There are 2 ways to enable mods:

* Editing your `CONFIG.BIN` in `FUCTool` and set the `File Replacer` option to `Enable`.
* Enable in-game by going to `Options` from `Main Menu` and enable `File Replacer`.

Once enabled, restart the game for changes to take effect.

| <a href="/assets/images/options_menu.png" target="_blank"><img src="/assets/images/options_menu.png"></a> | <a href="/assets/images/fuctool_mods3.png" target="_blank"><img src="/assets/images/fuctool_mods3.png"></a> |
|:---:|:---:|
| Go to `Options` under `Main Menu` and enable `File Replacer`.<br>**Restart your game.** | You should now see your mods working  |