---
doc_type: "SET_TOPIC"
title: "PERFORMANCE"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1052942202596233276"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2022-12-15"
---

🖐️ 
1. Unreal uses "canvas" as an area to draw composit textures. For example: NinjaTools is baking the flipbooks to frames, and creates a single image (called "flipbook") by drawing all frames to a single texture, using the "DrawMaterialToCanvas" function (with the underlying DrawTile function) ---- as opposed to this, NinjaLive does NOT use "DrawMaterialToCanvas" but "DrawMaterialToRenderTarget" (with the underlying DrawTexture function) -- which is 1:1 drawing, no tiling, no UV coordinates...
.
2. You could also test things by loading one of the original, simple ninja levels (eg Usecase 1: \Content\FluidNinjaLive\UseCases\Levels\Usecase_001_WorldSpaceWater_LIVE17) - and try to profile that one, to see the GPU processes typical to ninja. 
.
3. You could also check 3 performance test levels: \Content\FluidNinjaLive\Tutorial\LevelsSpecial\NinjaLive_Level14A_Performance_Peak_Single --- and 2 others in the same folder. These levels are made to measure ninja performance in an isolated environment.
.
CONCLUSION: a simple 256 x 256 ninja container tracing a single object consumes 0.043 milisec / frame on GTX 1070 (which is less than the 0.5% of the total 16.6 frame budget with a 60 FPS target framerate) --- of course, a 2K container, tracking dozens of objects and driving a komplex, single layer water based material, particles and volumetrics in the same time (see Usecase 14B) eats a lot more --- but, it is up to the users to decide which features are important, when the time comes to optimize.
.
