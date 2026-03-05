---
doc_type: "SET_TOPIC"
title: "HQ VOLUMESMOKE FOR CINEMATICS"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/850913821827792940/873319456921747476"
source_channel: "general"
author: "andrasketzer"
date: "2021-08-06"
---

SET TOPIC: HQ VOLUMESMOKE FOR CINEMATICS
We have three components that influence quality:
(1) core sim: all related settings in NinjaLiveComponent /LivePerformance
(2) bridge RenderTarget - core writes here, Volume reads this -- quality settings defined at the "details" panel
(3) volumesmoke material instance: see lit/unlit and noise usage main switches.
Besides all these, engine level settings like antialiasing and motion blur quality also matter.
