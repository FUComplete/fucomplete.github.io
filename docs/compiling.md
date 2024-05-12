---
layout: default
title: Compiling
nav_order: 5
---

# Compiling
{: .text-yellow-300 .fw-500 .text-center .fs-8 .lh-default .no_toc }

{: .note }
>This compiling guide is targeted towards WSL/Linux users.
>
>If using WSL, I suggest setting up [ArchWSL](https://github.com/yuk7/ArchWSL).
>
>If using Linux, the following info below is for Arch Linux, so you may have to adapt the package requirements if you are using a different distribution.

---

### Prerequisites
{: .no_toc .text-yellow-300 .fw-700 }

#### Files
{: .text-yellow-300 .fw-700 }
* P2G.iso (unpatched ISO)
* FUC.iso (patched ISO)
* deceboot ([download](https://www.romhacking.net/utilities/1225/))
{: .pl-6 .lh-tight }

#### Dependencies (Arch Linux)
{: .no_toc .text-yellow-300 .fw-700 }
* base-devel
* cdrtools
* cmake
* git
* python
* python-pip 
* python-setuptools
* p7zip
* wget 
{: .pl-6 .lh-tight }

---

### Setup
{: .text-yellow-300 .fw-700 }

{: .warning }
You will need at least **5GB** of free space.

Download the [source](https://github.com/FUComplete/Patch/archive/refs/heads/main.zip) and extract. Inside the extracted directory create a `iso` and `tools` folder and place `FUC.iso` and `P2G.iso` inside the `iso` folder. place `deceboot` archive (filename should be `deceboot_0_3.zip`) inside the `tools` folder.

Your directory structure should look like this after you've placed everything accordingly.

```
.
├───.git
├───data
├───iso
│   ├───P2G.iso
│   └───FUC.iso
├───modloader
├───mods
├───patches
└───tools
    └───deceboot_0_3.zip
.gitignore
build_iso.sh
build.sh
events_builder.sh
main.asm
README.md
setup.sh
ULJM05500.ini
```
{: .lh-0 }

Once done open a terminal to the path of the source directory and execute `./setup.sh`. This will take a while.

---

### Build
{: .text-yellow-300 .fw-700 }

#### Compile/Patch ISO_ROOT
{: .no_toc .text-yellow-300 .fw-700 }

Before you compile, you can place any additional mods you want to apply to `DATA.BIN` in the `builds/data_in` folder with their name as their file ID.

To compile the asm patches and patch `ISO_ROOT`, run `./build.sh`. 

{: .note }
You can test modloader changes with current release ISO by placing `PRELOAD.BIN`, `MODLOAD.BIN` and `CONFIG.BIN` located in `build/ISO_ROOT/FUC` folder into your SAVEDATAs `FUCDAT` folder.

#### Build ISO
{: .no_toc .text-yellow-300 .fw-700 }

Once you are happy with your changes, run `./build_iso.sh` to generate a ISO. This will be found at `build/FUC_Debug.ISO`