---
doc_type: "SET_TOPIC"
title: "SET TOPIC: LEVEL 23 SYSTEMS ARE DOWN FOLLOWING MIGRATION"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/850913821827792940/863180427865620533"
source_channel: "general"
author: "andrasketzer"
date: "2021-07-09"
---

**SET TOPIC: LEVEL 23 SYSTEMS ARE DOWN FOLLOWING MIGRATION**
A reply to this post: https://discord.com/channels/850913821240983553/850913821827792940/861957451619762176
, thanks for reaching out!
Two ways to start investigation: (1) RenderTargets and (2) Volumetrics
(1) Systems on Levels 23-28 and 30-32 are all using RenderTargets to forward sim data to volumes. Could you pls check those levels too? In case they are broken, too: it might be the case that migration broke links between ninja containers --- RenderTGs --- and Volumes.
You could check redirectors (did you change placement?) and you could simply re-bind RenderTargets on both sides (ninja sim container and volume) 
--- see **Manual, Chapter 24.4** - **Linking Volumetrics And Ninja**
(2) UE goes tricky sometimes, and switches off VolumeFog visualization on the engine level.
Two things to check:
(A) make sure that *Viewport UI /SHOW /Lighting Features /Volumetric Fog* is ON
(B) make sure that *Settings /EngineScalabilitySettings* are HIGH or EPIC
