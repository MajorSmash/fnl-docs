---
doc_type: "SET_TOPIC"
title: "NINJALIVE vs iOS / macOS / APPLE"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/999837847202832405"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2022-07-22"
---

SET TOPIC: **NINJALIVE vs iOS / macOS / APPLE**
Approximately 0.4% of our users is working on iOS, we have confirmations that ninja could be run and compiled --- but it is not so easy as on PC and android --- for example: the new HLSL based pressure solver (introduced in Live 1.3) causes iOS crash --- users have to force ninja to use the old pressure solver. ---- Some shaders also behave weird: with flowmaps, the (-1)-to-(+1) value ranges are clamped to 0-1 under iOS. --- So briefly: it seems like we have a couple of minor and medium flaws under iOS.
