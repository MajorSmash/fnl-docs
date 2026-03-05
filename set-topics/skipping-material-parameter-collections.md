---
doc_type: "SET_TOPIC"
title: "SKIPPING MATERIAL PARAMETER COLLECTIONS"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1233438910420488232"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2024-04-26"
---

SET TOPIC: **SKIPPING MATERIAL PARAMETER COLLECTIONS**
1. in some cases, ninja uses MPCs (Material Parameter Collections) to forward positional parameters to an Output Material.
2. too bad, MPCs do not support double vectors (as of UE 5.4) - so they are not LWC (large world) compatible
3. workaround: MP Collections are like a bridge between a blueprint and a material. And we can directly forward the params to the material, without MPC - all we need is a blueprint that GETS the dynamic material instance from ninja, and SETS the params to the matertial
4. ninja stores the final, in-game-used output material instances in 3 variables: *"OutputMaterial", "SecondaryOutputMaterial" and "TerrtiaryOutputMaterial" * and we need to query these variable in-game with our blueprint
