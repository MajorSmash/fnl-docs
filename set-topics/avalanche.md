---
doc_type: "SET_TOPIC"
title: "AVALANCHE"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/850913821827792940/886505149760143431"
source_channel: "general"
author: "andrasketzer"
date: "2021-09-12"
---

SET TOPIC: **AVALANCHE**
, thanks for reaching out!
(1) here comes a few very early, crappy test from proto-ninja, 2019: https://youtu.be/mFak-FSFBr0, https://youtu.be/VllQ4vRVVyA, https://youtu.be/FP7makggsb8
(2) in the above cases, physics objects are used as simulation density input - but, there are many ways to go - texture offset, animated material, or particles (see Level3 demonstrating sim inputs, and how to set them up)
The point is the right DYNAMICS of input field: heterogen density, slightly bouncy, some parts are faster, at the end the front line is slowing down, so, the remaining part catches up.
(3) once the 2D sim looks fine, we set up a rotated VolumeSmoke container to make our 2D data extruded/volume-like. See Level 30 and Manual Chapter 24. Eg.: https://youtu.be/2Tg2QfB1wC0?list=PLVCUepYV6TvPYbofpEf_ghznfihM-yt-B&t=598, https://youtu.be/LKzLv6yvN8U?t=8
(4) Additionally, we could drive particles (avanlenche debris) using sim velocity (Level 20 A-B). Eg: https://youtu.be/v8d0CalL9oA?list=PLVCUepYV6TvPYbofpEf_ghznfihM-yt-B&t=942
