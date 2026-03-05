---
doc_type: "SET_TOPIC"
title: "SIM EDGES AND CLAMPING"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1204356975706640454"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2024-02-06"
---

🖐️ welcome!
Like *Kynolin* said: these "lines in the distance" are the result of texture clamping -- and we can avoid this, by setting the "texture edges" (that is: simulation buffer edges!) to **black**.
There are two places where we could modify sim area edge:
.
**1.** In the Preset Manager:
.
