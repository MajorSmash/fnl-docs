---
doc_type: "SET_TOPIC"
title: "A."
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/850913821827792940/1214502562229915649"
source_channel: "general"
author: "andrasketzer"
date: "2024-03-05"
---

🖐️ Thanks for reaching out!
1. "the dirty water look" depends on two factors (A,B)

**A.** adjusting params in the output material (change water color and transparency, adjust flow-detail map - all user editable) - see the upper and and lower half of this picture: https://cdn1.epicgames.com/ue/product/Screenshot/14-1920x1080-3aede98df83d73b1c3bb7b94aee3e9eb.jpg?resize=1&w=1920 - same simulation - two differently adjusted output materials.
In case you wonder what output materials are: please start with the "introduction to ninja" tutorial: https://www.youtube.com/watch?v=vXalfRAnXak
*(+ See usecase levels 14 A,B,C for the various output material setups)*

**B.** adding floating debris (using niagar mesh particles) on top top of the water. See Usecase levels: 11 + 14-A,B,C
Sample vid: https://youtu.be/UbhPiT_bRR0?t=10

*Related topics, regarding coastline/riverbank and wave height:*
SET TOPIC: COASTLINES, RIVERBANKS: https://discord.com/channels/850913821240983553/851482546100633601/1204727485716107295
SET TOPIC: WAVE HEIGHT: https://discord.com/channels/850913821240983553/851482546100633601/1115311693103366194
(brielfy: ninja is a 2D sim, drinving waves by extrusion: this is limiting wave-size, no large concave waves could be achieved - only convex shapes)
