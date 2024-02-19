---
layout: default
title: Custom Quests
nav_order: 3
parent: Setup
---

# Custom Quests
{: .text-yellow-300 .fw-500 .text-center .fs-8 .lh-default .no_toc }

{: .warning }
Just as a precaution, **ALWAYS** backup your save before injecting quests just in case something goes wrong.

## Table of contents
{: .no_toc .text-delta }

- TOC
{:toc}

---

## Injecting Quests
{: .text-yellow-300 .fw-700 .text-center }
<br>

In the folder where you extracted the zip from [Step 1](/docs/setup.html/#step-1-download-latest-build-of-fucomplete), copy your custom quests to the `quests` folder. 

Open `FUCTool` and go to the `Custom Quests` tab, you should see your quests listed in the left table.

{: .note }
If you do not see your quests listed in the left table, please make sure your quests are **decryted** and either `.mib` or `.pat`. 

Press the `Select` button and select your save folder, it will be in `SAVEDATA` and will be one of the following IDs

* `ULUS10391`
* `ULES01213`
* `ULJM05500`
{: .pl-6 }

Once you select your save folder you can now begin to backup/inject quests.

* **To backup quests**: Click on each quest you wish to backup in the right table and press the `<---` button.
* **To inject quests**: Click on each quest you wish to inject in the left table and press the `--->` button.
{: .pl-6 }

Once you are happy, hit the `Save` button to inject the quests.

{: .warning }
Please **DO NOT** try to resave while you have the game running, this will corrupt your save. **ALWAYS** have the game closed and reload your save when you inject quests.

| <a href="/assets/images/fuctool_cq1.png" target="_blank"><img src="/assets/images/fuctool_cq1.png"></a> | <a href="/assets/images/fuctool_cq2.png" target="_blank"><img src="/assets/images/fuctool_cq2.png"></a> |
|:---:|:---:|
| Open your save in `SAVEDATA` | Select the quests you wish to inject |
| <a href="/assets/images/fuctool_cq3.png" target="_blank"><img src="/assets/images/fuctool_cq3.png"></a> | <a href="/assets/images/fuctool_cq4.png" target="_blank"><img src="/assets/images/fuctool_cq4.png"></a> |
| Press the `--->` button to queue the quests for injection. | Press `Save` to write the quests to savedata. |

---

## Loading Custom Quests In-game
{: .text-yellow-300 .fw-700 .text-center }
<br>

{: .note}
>When you start your game you may see a message like this pop-up on PPSSPP. 
>![OldSave](/assets/images/fuctool_cq_errormsg.png)
> If you do, you can remove it by saving in-game and you'll no longer see the message.

To play your custom quests, go to the Guildhall, open your options menu and under `Savedata Quests` toggle the option `ON`. Once enabled talk to a quest giver and open the "Events" tab... you should see your injected quests.

| <a href="/assets/images/fuctool_cq_toggle.png" target="_blank"><img src="/assets/images/fuctool_cq_toggle.png"></a> | <a href="/assets/images/fuctool_cq_events_tab.png" target="_blank"><img src="/assets/images/fuctool_cq_events_tab.png"></a> |
|:---:|:---:|
| Toggle `ON` the `Savedata Quests` option. | Go to `Events` and you should see your custom quests listed. |