---
doc_type: "SET_TOPIC"
title: "FIX USECASE 3 \"SINKING SHIP\" UNDER UE 4.27"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/850926358196125726/877998861187166278"
source_channel: "ninjalive-issues"
author: "andrasketzer"
date: "2021-08-19"
---

SET TOPIC: **FIX USECASE 3 "SINKING SHIP" UNDER UE 4.27**
UseCase003 "Boat Example" level is broken under UE 4.27: the boat sinks as we start gameplay.
On 21 Aug. 2021 we have updated the UseCase ZIP package - so, you could re-download it. In case you would like to FIX it yourself:
.
(1) Open "/Content/FluidNinjaLive/UseCases/003_DrivingUEwater/BP_Buoy" blueprint
(2) Select the "Buoyancy" Component
(3) At the Component Details /Activation: SET Auto Activation to TRUE
.
