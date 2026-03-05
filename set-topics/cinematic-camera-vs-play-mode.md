---
doc_type: "SET_TOPIC"
title: "CINEMATIC CAMERA vs PLAY MODE"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1195740038198202378"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2024-01-13"
---

, I did a quick research:
1. UE "Play" session requires a "Player Class Object" - be it a camera, or pawn - and we "possess" this player during the play session
2. The default cinematic camera does not qualify as "Player" / can not be possessed --- hence, can not be used during Play.
3. This UE forums post offers a solution, by adding a CineCamera to a Pawn: https://forums.unrealengine.com/t/how-to-use-cinematic-camera-in-play-mode/745068
*(and a "pawn" is not necessarily a biped character: it could be "empty" as well)*
