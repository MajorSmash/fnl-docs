---
doc_type: "SET_TOPIC"
title: "measuring FPS"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/994208956887080990"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2022-07-06"
---

SET TOPIC: **measuring FPS** in the runtime Live 1.7 demo exe:
.
1. the console works in the demo using the ` character
2. two commands needed: "t.MaxFPS 999" (unlocks 60 FPS limiter) and "stat FPS" (displays FPS) 
.
*Playable minidemo link: https://kynolin.itch.io/fluidninja-live-17-demo (150 Mbytes, exe)*
.
Measuring FPS in the UE project:
1. select NinjaLive_Utilities Actor on the level (green N)
2. change MaxFPS from 60 to 999 at the Actor Details Panel
3. Go to the viewport top right rolldown menu, and chose "show FPS"
