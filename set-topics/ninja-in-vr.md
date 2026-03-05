---
doc_type: "SET_TOPIC"
title: "NINJA in VR"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/877193240539959376"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2021-08-17"
---

SET TOPIC: **NINJA in VR**
Officially, ninja does not support VR --- but, the hope is not lost 🙂
(1) ninja is a scalable 2D sim, that is fully android compatible and runs fine on a 2016 Samsung model (https://twitter.com/FluidNinjaLIVE/status/1325574530027368448) --- so in theory, it should be fine both on tethered (Oculus Rift) and on android based headgear (Oculus Quest 1,2)
(2) Results show: ninja could be ported to tetherd (desktop) VR (https://twitter.com/_JasonCooper/status/1364968363328491529)
(3) The latest volumetric update is made for next gen and cinematic usage - so, I was somewhat surpised when it turned out: it runs on a tethered headgear, looking great.(https://twitter.com/thegiffman/status/1417222608743976973)
(4) Oculus Quest2: the first successful test is done by HorizonVP (currently WIP) - one important conclusion:
the new HLSL  based pressure solver, introduced at live 1.3 kills the headgear - so devs are advised to switch back to Pressure Solver 1: see NinjaLiveComponent /LivePerformance /UsePressureSolver1 BOOL FLAG.
(5) In Live 1.7 a lot of TRANSLUCENT systems have been reconfigured to OPAQUE --- which is way more VR-device friendly
