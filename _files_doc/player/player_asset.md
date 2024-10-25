---
layout: default
title: Player Assets
nav_order: 2
has_toc: false
---

# Player Assets
{: .text-yellow-300 .fw-700 }

---

| [![Faces](../../assets/images/face.png)](pl_face.html)<br>Faces | [![Outfits](../../assets/images/outfit.png)](pl_outfits.html)<br>Outfits | [![Armors](../../assets/images/body_armor.png)](pl_armors.html)<br>Armors | [![Weapons](../../assets/images/weapon.png)](pl_weapons.html)<br>Weapons |
{: .text-yellow-300 .fw-700 .text-center }

---

## Models
{: .text-yellow-300 .fw-700 }

Models have some strict guidelines due to hardcoded memory allocations.

{: .note }
The name/folder structure of the files was kept consistent with the original file name/folder structure from Capcom... this is why legs are named `reg` and head/hair are swapped.

### Max File Size
{: .text-yellow-300 .pb-3 }

{: .warning }
When modding the game, do not go over the max file size... if you do your model will either corrupt or crash the game.

| <span style="color:#ffeb82">Type</span>  | <span style="color:#ffeb82">Max Size<br>(bytes)</span> | <span style="color:#ffeb82">Location</span> | 
|:-------:|:-------------------:|:--------------------------------------------------:|
| Weapons |        22528        |                  data_root/weapon                  |
| Arms    |        22528        |  data_root/player/f/arm<br>data_root/player/m/arm  |
| Body    |        30720        | data_root/player/f/body<br>data_root/player/m/body |
| Face    |        10240        | data_root/player/f/face<br>data_root/player/m/face |
| Head    |        18432        | data_root/player/f/hair<br>data_root/player/m/hair |
| Hair    |        16384        | data_root/player/f/head<br>data_root/player/m/head |
| Leg     |        32768        |  data_root/player/f/reg<br>data_root/player/m/reg  |
| Skin    |         6144        | data_root/player/f/skin<br>data_root/player/m/skin |
| Waist   |        22528        |  data_root/player/f/wst<br>data_root/player/m/wst  |

### Max Vanilla Vert/Tri
{: .text-yellow-300 }

| <span style="color:#ffeb82">Type</span> | <span style="color:#ffeb82">Max Vertices</span> | <span style="color:#ffeb82">Max Triangle</span> |
|:-----:|:------------:|:------------:|
|  Head |      459     |      474     |
|  Body |      999     |      811     |
|  Arm  |      756     |      668     |
| Waist |      712     |      585     |
|  Leg  |     1006     |      856     |

### Max Theoretical Vert/Tri
{: .text-yellow-300 .pb-3 }

{: .warning }
The max theoretical comes from successfully imported armors that exceed vanilla however have not been fully tested... You have been warned. 

| <span style="color:#ffeb82">Type</span> | <span style="color:#ffeb82">Max Vertices</span> | <span style="color:#ffeb82">Max Triangle</span> |
|:-----:|:------------:|:------------:|
|  Head |      487     |      501     |
|  Body |     1025     |      966     |
|  Arm  |      710     |      738     |
| Waist |      826     |      782     |
|  Leg  |      861     |      878     |
