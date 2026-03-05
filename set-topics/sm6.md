---
doc_type: "SET_TOPIC"
title: "SM6"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1073189325237407804"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2023-02-09"
---

Hello, sorry for the automatic translation.
After moving to UE5.1 and enabling SM6, suddenly the GPU load increased.
It's CanvasDrawTiles that's going up.
Checking with Usecase001, it is about 15ms.
The confirmed environment is GeForce2080Super.
Investigating the cause with RenderDoc, I found that the load of M_Pressure was high.
Further investigation revealed that the custom HLSL of MF_SeparableMultiKernelDiffusion increased the load.
Adding static to the array like the image improved the GPU load.
I don't know the exact cause, but I will let you know.
Thank you very much.😀
