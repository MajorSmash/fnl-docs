---
doc_type: "SET_TOPIC"
title: "WATER PERFORMANCE"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/887319749233606696"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2021-09-14"
---

SET TOPIC: **WATER PERFORMANCE**
Komplex "water features" have been added to ninja, because the native UE water system, introduced in UE version 4.26 is not very fast - the "boat scene" (see UseCase 3 - https://youtu.be/-OvCw4Y4480 ) runs 70-80 FPS on RTX 2080. Ninja water tech, introduced in UseCase 6 (see: https://youtu.be/XfGXwYxKYIE) runs around 160-220 FPS.
Performance could be further optimized: the current water base material uses a *special Material Domain* - that merges the properties of translucent and opaque materials (both reflective, and see-through) - and this adds up to ~570 instructions per pixel. When used in simple translucent OR simple opaque mode, the we get below 250 IPP, which is quite good. By using opaque domain and switching of some containers on the demo level, we could get above 300 FPS.
