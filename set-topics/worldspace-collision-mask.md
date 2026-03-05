---
doc_type: "SET_TOPIC"
title: "WORLDSPACE COLLISION MASK"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1117460719298945084"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2023-06-11"
---

SET TOPIC: **WORLDSPACE COLLISION MASK**
1. Collision Masking is a useful feature - demonstrated on Tutorial Level 3 / Stage 9 - and in this video:
https://youtu.be/v8d0CalL9oA?list=PLVCUepYV6TvPYbofpEf_ghznfihM-yt-B&t=638
2. Colli.Masking is, by default, LOCAL space (non world-space)
3. Here comes a TWEAK to make it WorldSpace. We need to modify two assets: *NinjaLiveComponent* Blueprint + *M_CompositeAndGradient* Material
I am including screenshots, showing the modification sites - AND - text files, to copy-paste the node-graph into your assets (UE 5.1)
.
UPDATE: a related post from  - describing how he implemented the above **WorldSpace Collision Mask** method in his project: https://discord.com/channels/850913821240983553/850913821827792940/1117964210350084176 + https://discord.com/channels/850913821240983553/850913821827792940/1117965205280923688 + https://discord.com/channels/850913821240983553/850913821827792940/1124141438955946055
.
