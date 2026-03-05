---
doc_type: "SET_TOPIC"
title: "RAYTRACING"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/850926358196125726/899230124078141450"
source_channel: "ninjalive-issues"
author: "andrasketzer"
date: "2021-10-17"
---

SET TOPIC: RAYTRACING
Raytracing vs translucency vs refraction:
I believe this could be properly set up: in the BaseMaterial, we have two masterswitch to pick the type of REFRACTION - "the other" might work. Also, ninja basemat sets REFRACTION null point to "1" - it might be the case that we need to set this to "0" -- and you could do it in the OutputMaterial Instance.
.
Raytracing vs translucency vs volumetrics: volumetrics DOES NOT WORK with raytracing on - this is a general issue with UE (not a ninja specific issue)
.
.
