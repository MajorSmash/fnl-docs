---
doc_type: "SET_TOPIC"
title: "SCALING AND MOVING A MUSHROOM CLOUD"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1460943284401868800"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2026-01-14"
---

SET TOPIC: **SCALING AND MOVING A MUSHROOM CLOUD**, under Live 1.9
1. Opening Level "*VolumeGeneric5_LargeScaleExamples_NoFluidSim*"
2. Selecting Actor "*VolumeCloud_MultiLayer_Mushroom1*"
3. Opening up Material Instance "*MI_VolumeGeneric_LayerHost_CVOL_MushroomAndCone*" from the Actor Details Panel
4. There are TWO Material Layers in the material -  we are accesing them opening the "layer paramaters" tab on the material instance panel ---> *MLI_VolumeGeneric_Layer_CVOL_Cone*  +   *MLI_VolumeGeneric_Layer_CVOL_Mushroom*
5. We ignore the "*Cone*" layer for now, for the sake of simplicty.
6. We are opening up "*MLI_VolumeGeneric_Layer_CVOL_Mushroom*" by double clicking on it - so we end up on the material instance layer panel
7. Looking up the "*Density*" Parameter Group

SCALING-DOWN: via the "*DensityScale-UVW*" param  (note: *larger value means more scaling-down!*)
POSITION: via the *U-offset, V-offset, W-offset* parameters

Method: we adjust a parameter, then **PRESS SAVE on the layer**, in order to UPDATE the results in the viewport.
See below video ⬇️
.
