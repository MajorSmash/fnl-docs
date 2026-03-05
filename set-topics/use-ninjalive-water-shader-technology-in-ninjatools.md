---
doc_type: "SET_TOPIC"
title: "use NinjaLIVE water shader-technology in NinjaTOOLS"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1286602051882717297"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2024-09-20"
---

SET TOPIC: **use NinjaLIVE water shader-technology in NinjaTOOLS**
.
**METHOD-1**: use what we already have in the two ninja projects / no material editing
This level in LIVE is demonstrating how to use a SECOND sim input to generate tiling waves over a surface:
*/FluidNinjaLive/UseCases/Levels/Usecase_004A_DoubleSim_TilingWaves_LIVE18*
The second sim is read from a RenderTarget (see yellow arrow on the below screenshot) --- Let us examine the used Material Instance (*MI_Water_SingleLayer_Tile_Simulated*): the SECOND (external) sim data is is read through the TILEMAP option.
.
