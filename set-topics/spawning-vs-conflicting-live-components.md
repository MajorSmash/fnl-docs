---
doc_type: "SET_TOPIC"
title: "SPAWNING vs CONFLICTING LIVE COMPONENTS"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1285318333406904360"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2024-09-16"
---

SET TOPIC: **SPAWNING vs CONFLICTING LIVE COMPONENTS**
1. when multiple ninja-sims overlap, linetracers would conflict / a tracemesh of simulation "A" blocks the linetrace rays of simulation "B".
2. to avoid conflict, NinjaLive COMPONENT collects all actors with Live Interface at EventBeginPlay (and on RePlay) -- and excludes them from its linetracer - by adding them to the "NinjaLiveTraceExclude" Array. See MODULE020 in NinjaLiveComponent Blueprint - https://discord.com/channels/850913821240983553/850913821827792940/1284102636295032874
3. problem: since "to be excluded" ninja sims are collected upon EventBeginPlay... spawned sims could conflict: https://discord.com/channels/850913821240983553/850913821827792940/1284089817327599638
4. this could be avoided, by calling an event on spawn, that adds the newly spawned sim to the exclusion list: https://discord.com/channels/850913821240983553/850913821827792940/1285269756047527988
