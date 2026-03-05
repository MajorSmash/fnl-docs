---
doc_type: "SET_TOPIC"
title: "GLOBAL GROUND FOG"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/850913821827792940/873322846045237268"
source_channel: "general"
author: "andrasketzer"
date: "2021-08-06"
---

SET TOPIC: GLOBAL GROUND FOG
Thanks for reaching out!
Ninja is using local containers to deliver fluidsim. Three ways to make this global:
(1) via TILING (using local fluidsim repeated in a global field) see: https://youtu.be/uH2DRdKruaU
(2) via WORLD OFFSET (adding local fluidsim to a global non-fluid field) see:
https://youtu.be/uH2DRdKruaU
(3) via CONTAINER ARRAYS (placing local containers in large arrays heavily relying on LOD) see this vid at 9-12 mins: https://youtu.be/2Tg2QfB1wC0
.
In terms of fluid-visualization technology: (A) UE native VolumeFog could be a good choice - no self shadows, frustrum aligned grid -- (B) while VolumeSmoke looks better. See Manual chapter 24 comparing available volumetric systems.
