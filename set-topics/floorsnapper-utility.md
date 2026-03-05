---
doc_type: "SET_TOPIC"
title: "FLOORSNAPPER UTILITY"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1098227067579011153"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2023-04-19"
---

SET TOPIC:** FLOORSNAPPER UTILITY** - EXCLUSIVE vs INCLUSIVE METHODS
1. The Floorsnapper Utility is a blueprint, made to ALIGN objects (eg. simulation and volume containers) with the floor (ground, landscape... etc)
2. The workings in general are explained here: https://youtu.be/3cBo9pHUXUA?list=PLVCUepYV6TvMXN8HQjLU9wKz-G_6JvJsF&t=629
3. Specifically, the methods of finding floor NORMALS are explained here: https://youtu.be/3cBo9pHUXUA?list=PLVCUepYV6TvMXN8HQjLU9wKz-G_6JvJsF&t=1030
.
As the video, and the blueprint placed helper texts explain, there are EXCLUSIVE and INCLUSIVE methods to identify which objects we would like to detect "as floor". Exclusive methods are easy to set up - but these require us to TAG each object we would like to exclude. Not recommended for a thousand-object Level. Inclusive methods IGNORE every object by default, and include (detect, accept) only the ones that we manually set to be included - usually, only the Landscape.
One of the inclusive methods (A2) requires us to set-up a custom line-trace channel, with a default response as IGNORE. And then, select the landscape object, and set its collision RESPONSE to "not ignore" (BLOCK) the custom Line Trace. The below two screenshots illustrate these two key steps:
.
