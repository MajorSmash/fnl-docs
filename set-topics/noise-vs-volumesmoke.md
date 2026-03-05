---
doc_type: "SET_TOPIC"
title: "NOISE vs VOLUMESMOKE"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/915897403880652810"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2021-12-02"
---

SET TOPIC: **NOISE vs VOLUMESMOKE**
This post is comparing 2D / 3D noises - in a performance / visual quality tradeoff situation
.
Facts: 
(1) In terms of volume rendering, *NinjaTools *<:NinjaTools:851394765647118346>  and *NinjaLive *<:NinjaLive:851418299853045810>  are using similar technology
(2) Raw desity sometimes looks too simple when visualised via VolumeSmoke
(3) We could use noise to add details to the Smoke
(4) In the case of VolumeSmoke, we could do this two ways: 3D noise -- or -- 2D noise
.
(a) We could add 3D volumetric noise to the raw sim data IN THE VOLUMESMOKE MATERIAL - but that is really performance heavy.
(b) In NinjaLive 1.5 / NinjaTools 1.6 a new technique has been demonstrated: we are setting up an output material that adds 2D noise (a detail map) to the raw sim output, and we channel this "noised" density to the VolumeSmoke.
.
Please have a look at below listed levels / read the level placed texts / watch the related tut vidS explaining it:
.
Live Tutorial Level 30 stage 5C: 2D noise -- See: 
https://youtu.be/f2Sqjzf4KKg?list=PLVCUepYV6TvPYbofpEf_ghznfihM-yt-B&t=713
Live Tutorial Level 30 stage 5B: 3D noise -- See: 
https://youtu.be/2Tg2QfB1wC0?list=PLVCUepYV6TvPYbofpEf_ghznfihM-yt-B&t=133
.
Tools "Usecases_VolumeSmoke" level stage 6B: 2D noise -- See: 
https://youtu.be/D0rAQR7CAIA?list=PLVCUepYV6TvPnVELcyGoSDhpoLO7PyT6_&t=383 
https://youtu.be/D0rAQR7CAIA
Tools "Usecases_VolumeSmoke" level stage 6C: 3D noise
.
