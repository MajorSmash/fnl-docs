---
doc_type: "SET_TOPIC"
title: "WATER LEVEL / BUOYANCY"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1017832482109923368"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2022-09-09"
---

SET TOPIC: **WATER LEVEL / BUOYANCY**
*1. can we make large waves via ninja?*
Ninja is a 2D sim, all 3D (meshes, volumes, particle clouds) are generated via height extrusion. The larger the extrusion is, the more obvious: we are faking  🙂 --- email me, so I could send you a copy for testing! (andras dot ketzer at gmail)
.
*2. Can we make objects float via ninja?*
Ninja does not have a native buoyancy function. Water height is defined by a constant offset + a sim buffer (usually pressure). The sim buffer is a RenderTarget --- it is sampled on the GPU, so particles, particle meshes and vertex shaders natively use this. Of course, the buffer could be sampled by super slow CPU methods in blueprints. This is feasible, if we sample only a few discrete points! --- Alternatively, you could sample scene depth (water-surface is SingleLayerWater, writes depth) --- and you could turn depth to WorldSpace coords in the material - and output that for the CPU ---- *(Additionally: there is a Niagara based method toexpose GPU data to the CPU: NiagaraScript'/Niagara/Modules/ExportParticleData/ExportParticleDataToBlueprint' - so, by sampling a RenderTarget, as TextureObject in niagara, it could be exposed to a BP )*
.
3. *Waves "height"*: https://discord.com/channels/850913821240983553/850913821827792940/1097830836209983489
