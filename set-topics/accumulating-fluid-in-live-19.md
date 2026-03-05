---
doc_type: "SET_TOPIC"
title: "ACCUMULATING FLUID in LIVE 1.9"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1370000743389597797"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2025-05-08"
---

🖐️ thanks for the kind words!
Yes we can fill a pool: I've quickly created a demo for you, modding the Usecase-7 "Small water bodies" pool scene.
Key mods: cranked up FEEDBACK in Preset Manager *above 1* (so density never vanishes, but accumulates) --- and set material blend mode to *masked* (from opaque) + adjusted alpha (see screenshot):
