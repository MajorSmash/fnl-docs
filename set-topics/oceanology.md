---
doc_type: "SET_TOPIC"
title: "OCEANOLOGY"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/994560648979681362"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2022-07-07"
---

SET TOPIC: **OCEANOLOGY**
.
**UPDATE** (April 2023): ninja vs oceanology - a **complete guide for merging the two systems**:
 https://discord.com/channels/850913821240983553/850913821827792938/1099591606300061766
.
 successfully integrated Oceanology and FluidNinja  🤩 : https://www.loom.com/share/49727409f7014bca9ec2c07ef23efcf8
 also got nice results: https://discord.com/channels/850913821240983553/850913821827792940/1140898253462843414
.
Recently, we have started to experiment how to add ninja sim on top of world-scale patterns.
Our first test with UE native water was successful: https://youtu.be/-OvCw4Y4480
Later on  has successfully combined ninja with oceanology: https://www.youtube.com/watch?v=6i8qZWo6wps
.
**LIVE 1.7 vs OCEANOLOGY**
1.  Before Live 1.7, ninja was already capable to export simulation buffers to RenderTargets -- and you could use these RenderTargets in your Oceanology materials. Export could be enabled at:
*/NinjaLiveComponent /LiveGeneric /WriteInternalSimBuffersToExternal*
See this post: https://discord.com/channels/850913821240983553/851482546100633601/1070700203318972458
.
2. In Live 1.7, a new feature has been added: ninja simulation area position and size could be automatically exported to a Material Param Collection, which is essential for correctly placing ninja sim in your OC material / OC worldspace. The option is located at:
*/NinjaLiveComponent /LiveGeneric /SetInternalParamsToMaterialParamCollection*
.
