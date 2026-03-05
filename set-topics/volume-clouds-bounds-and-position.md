---
doc_type: "SET_TOPIC"
title: "VOLUME CLOUDS - BOUNDS AND POSITION"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/859536075475124251"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2021-06-29"
---

SET TOPIC: **VOLUME CLOUDS - BOUNDS AND POSITION** ☁️ 
In the case of VolumeClouds, bounds and position are defined within the material (no mesh needed), using UVW coordinate offset and scaling. 
For Volumetrics **V2** Clouds, see: https://discord.com/channels/850913821240983553/850913821827792940/1364618883230863360
For Volumetrics **V1**: (1) Select "VolumetricCloud" Actor on Level, (2) Go to Actor Details Panel, and double-click on "Cloud Material" - so it will open up the actually used Cloud Material Instance. (3) In the Material, locate *CloudU-Offset, V-offset* and BasePlane**Altitude** params.
.
