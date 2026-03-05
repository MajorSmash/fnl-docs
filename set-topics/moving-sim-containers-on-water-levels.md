---
doc_type: "SET_TOPIC"
title: "MOVING SIM CONTAINERS ON WATER LEVELS"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/887987379397345310"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2021-09-16"
---

SET TOPIC: **MOVING SIM CONTAINERS ON WATER LEVELS**
.
*Post part 1 --- written in the Live 1.6 era:*
Ninja containers are being moved TWO ways in UseCase 1-6:
(A) the level blueprint gets pawn POS, and applies the XY component to ninja, while keeps Z fixed.
(B) ninja is attached to pawn with ROT locked.
.
Both method has its advantage: B doesn't require additional BP help - but the container also follows Pawn on the vertical (Z) axis - so the Pawn can not "jump out / jump above" the water.
.
*Post part 2 --- written in the Live 1.7-1.8 era:*
https://discord.com/channels/850913821240983553/850926358196125726/1034904106730533014
