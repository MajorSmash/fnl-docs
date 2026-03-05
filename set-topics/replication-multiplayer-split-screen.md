---
doc_type: "SET_TOPIC"
title: "REPLICATION, MULTIPLAYER, SPLIT-SCREEN"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1050688301956354088"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2022-12-09"
---

SET TOPIC: **REPLICATION, MULTIPLAYER, SPLIT-SCREEN** - https://discord.com/channels/850913821240983553/850926358196125726/1185468157276737587
Ninja is not replicated, and multiplayer is officially not supported (as stated on the Project Homepage: https://ibb.co/D5d8WqD). Ninja operates as a client side VFX tool. As such, it has little need of replication in it's core systems. In case the agents (characters, objects) interacting with the simulation ARE replicated: all local sims produce the same result on the client side (see example shot below).

In general with replication and networking, you want to replicate as little as possible to save on bandwidth and increase responsiveness; recreating data onto the server/client. As such, Ninja really only requires an updated transform per interacting actor.
.
Since Ninja is created with this in mind, it operates in a **Listen Server** networked environment seamlessly compared to standalone.
For **Dedicated Servers**, it will require some modifications to prevent the VFX logic from running on the server.
.
*Additionally*: 
1. **user  explains his multiplayer setup:** https://discord.com/channels/850913821240983553/850913821827792940/1429508642029305917 
+ the finished game: https://store.steampowered.com/app/2270230/Glitch_Party/

2. user  achieved nice results with default-pawn:
https://discord.com/channels/850913821240983553/850926358196125726/1083863271687344199

*Related posts:* 
Spawning vs ninja overlap detection: https://discord.com/channels/850913821240983553/850913821827792940/1072071323070763071
Multiple agents / linetrace conflict: https://discord.com/channels/850913821240983553/850913821827792940/1124002722048376887
.
Split-screen does **not** work under UE 5.3: https://discord.com/channels/850913821240983553/850926358196125726/1215596676585095188 - **works** in 5.4: https://discord.com/channels/850913821240983553/850926358196125726/1220118391180754995
.
