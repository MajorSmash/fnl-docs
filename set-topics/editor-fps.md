---
doc_type: "SET_TOPIC"
title: "EDITOR FPS"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/875673408476676126"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2021-08-13"
---

SET TOPIC: **EDITOR FPS**
*(copy-pasted from Manual, Chapter 11)*
.
By default, UE is set to run at 120 FPS. As a simple kind of performance measurement, legacy ninja versions (until 1.3) were UNLOCKING the UE limit, using the following console command: *t.MaxFPS 900* --- (900 FPS is an arbitrary, theoretical limit)
.
As a result, tutorial levels were running with no FPS-limit - usually around 200-400 FPS on a GTX 1070. This was a simple, good way to have instant feedback on performance bottlenecks. With the release of RTX 3000 series GeForce cards, a problem emerged: these cards were able to run test levels on 900+ FPS --- and the card got exhausted. The “Override Editor 120 FPS limit” got switched off, by default (on most levels).
.
