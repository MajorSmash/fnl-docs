---
doc_type: "SET_TOPIC"
title: "FOG OF WAR"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/850913821827792940/1408018340294688818"
source_channel: "general"
author: "andrasketzer"
date: "2025-08-21"
---

Welcome! ----- SET TOPIC: FOG OF WAR

*1.   Picking the right volume type:*
Ninja supports 4 volume types --- three of these utilize native unreal technology, with all the features / and limitations.
Let us exclude Cloud Volumes (CVOL) - as, these are meant for different purposes, also exclode Smoke and Heterogeneous Volumes (SVOL, HVOL) as these are meant and optimized for high detail closeups.
The only remaining volume type, optimal for your needs, is FOG Volume, FVOL. Read more about ninja volumes in Manual Chapter 24: https://discord.com/channels/850913821240983553/850925841793941565/855091427393273866

*2.   FVOL visibility *
FVOL visibility is influenced by MANY factors - most of these are independent from ninja. Pls have a look at this post: https://discord.com/channels/850913821240983553/851482546100633601/860217413761237023
Once you've made sure that non-ninja factors are maximized (UE is forced to show FVOL in large distances), let us move on to ninja-controlled factors.

3. Ninja VolumeFog technolog v1 is demonstrated on *LEVEL NinjaLive_Level23_VolumeFog*
Pls visit STAGE-2 / select ACTOR VoluCube_Example --- this example demonstrates a simple mesh, filled with fog - no fluidsim involved at all - ideal for testing ---- Material Instance "MI_VolumeFog_Cylinder" / check DistanceFade Param Group
BaseMaterial: "M_VolumeFog"
