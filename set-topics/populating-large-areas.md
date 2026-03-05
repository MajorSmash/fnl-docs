---
doc_type: "SET_TOPIC"
title: "POPULATING LARGE AREAS"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1064177463334273085"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2023-01-15"
---

SET TOPIC: **POPULATING LARGE AREAS** / NINJA in WORLD SPACE
1. the concept behind ninja is: have a local (limited, finite size) sim area attached to the player - and make it large enough to cover things in player-sight ---> so the player has this illusion of moving in a world-space where interaction (eg. water, or sand response) is not limited to a given area of the level.
Explained here: https://youtu.be/vXalfRAnXak?t=5249
.
2. alternatively, we could place (spawn and wake/sleep) a multitude of containers by using memory pooling  ("*recycled memory*")
See: *\Content\FluidNinjaLive\Tutorial\LevelsSpecial\NinjaLive_Level15_Performance_MemoryPooling.umap*
Demonstrated here: https://youtu.be/0O11SNavhM4?t=1535
.
3. ninja also supports an "efficent" mode (low memory, low GPU) - called "simple painter" - where no fluidsim is running, we only register overlap and draw trajctories - ideal for footsteps or wheeltracks. See: https://youtu.be/S5n5Tpd1Gko?list=PLVCUepYV6TvMXN8HQjLU9wKz-G_6JvJsF&t=889
.
So.: it is up to the users how they use this toolkit / how they populate third worlds with FX
