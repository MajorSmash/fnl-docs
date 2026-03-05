---
doc_type: "SET_TOPIC"
title: "MAKING VORTEX"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/866576173534412860"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2021-07-19"
---

SET TOPIC: **MAKING VORTEX** / **HEIGHT MAPS**
Please keep in mind: ninja core is a 2D fluidsim. Two ways to make this data a 3D CONE:
(1) Replace the FLAT *TraceMesh *with a CONE-shaped tracemesh, and map the simulation on this. Here is how to replace *TraceMesh*:
 https://discord.com/channels/850913821240983553/851482546100633601/855447762479611904
.
(2) Use the sim density as ELVATION (HEIGHT) MAP for one of the three volumetric visualization methods (*fog, clouds, smoke*)
.
