---
doc_type: "SET_TOPIC"
title: "SPLINE GENERATOR vs UE 5.1"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1046770378107797585"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2022-11-28"
---

SET TOPIC: **SPLINE GENERATOR vs UE 5.1**
Under UE 5.1, the river-mesh spline generator is becoming less responsive (laggy) in the editor, while editing the spline control-points - IF we are cloning very high resolution meshes along the spline. We could turn it responsive again, by temporarily using low-res meshes. Step-by-step:
(1) Select the Spline, (2) Look up Actor Details panel /SplineGenerator /StaticMeshComponent, (3) Replace the high resolution pre-tessellated mesh (eg. SM_plane_500x500) with a simple (eg. SM_plane_100x100) - while editing. Once done: add back the high-res geo.
