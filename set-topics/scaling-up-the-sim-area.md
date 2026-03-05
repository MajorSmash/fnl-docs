---
doc_type: "SET_TOPIC"
title: "SCALING UP THE SIM AREA"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1001393959777611826"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2022-07-26"
---

🖐️ thanks for checking in, your recent youtube test looks nice: https://discord.com/channels/850913821240983553/850922331878588416/1001044865389436938
.
SET TOPIC: **SCALING UP THE SIM AREA**
1. Ninja is a 2D sim - that could also drive external 3D systems, like volumetrics
2. The sim and the externals are scaled separately
3. Sim is mapped on TraceMesh, and Tmesh is scaled under LiveActor Details Panel /LiveInteraction /TraceMeshSize
Your assumption is correct: the larger the Tmesh, the smaller the texel density - so, we need to INCREASE SIM RESOLUTION, under:
*NinjaLive Actor /NinjaLiveComponent /LivePerformance /Resolution* (see attached pic No.1)
Important: a 1024px sim behaves differently compared to a 256px --- so, you probably need to tweak sim settings (speed, drag, noises) using the PresetManager
4. Once our 2D sim is scaled up propely, behaves as expected: we could focus on externals. Since Live 1.7, ninja could automatically scale externals: check youe VolumeSmoke Actor (or Component) and make sure it is in headless mode: *"Direcly Set...*" flags are configured to TRUE at the Details Panel. (see attached pic No.2)
5. Besides Scaling up the SIM AREA, external systems could be configured to EXTEND BEYOND THE SIM AREA --- and use noises and tile-pattern-generators to fill the extended area with meaningful / good looking data.
**Usecase Level 1** is a good example of generating WAVES in the extended area: https://youtu.be/S5n5Tpd1Gko?list=PLVCUepYV6TvMXN8HQjLU9wKz-G_6JvJsF&t=280
**Tutorial Level 31A** demonstrates how to extend VolumetricSmoke: https://youtu.be/yzDwi3ps7aI?list=PLVCUepYV6TvMXN8HQjLU9wKz-G_6JvJsF&t=178
.
+ a video snippet (also described in Manual Chapter 29.3) -- explaining how we could generate LARGE areas while the Tracemesh is relatively SMALL: https://youtu.be/S5n5Tpd1Gko?list=PLVCUepYV6TvMXN8HQjLU9wKz-G_6JvJsF&t=597
