---
doc_type: "SET_TOPIC"
title: "MAPPING SIM ON DEFORMED SURFACES"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1047577072157081651"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2022-11-30"
---

🖐️ 
The sim could be used & mapped many ways!
1. The tracemesh is user defined: it could be any shape (as long as the UV space is single-piece / consistent / island-free )
for example: https://youtu.be/2QlJ2f0aK5E?list=PLVCUepYV6TvPYbofpEf_ghznfihM-yt-B&t=344
2. Independently from the tracemesh shape (which is usually a plane): the sim could be mapped on any surface using direct drive:
for example: https://youtu.be/UBNjhb4J8I0?list=PLVCUepYV6TvMXN8HQjLU9wKz-G_6JvJsF&t=1719
.
So, this problem of "following the terrain" is really a problem of volumetrics --- the volumes (all types!) are strictly boxes / extruded from flat-plane--- and currently, there is no technology to make them follow the terrain - except rotating them to surface normals. This method is quite limited --- but there is no other solution.
.
This is, how I am solving it --- for a Pawn-attached volume container *(notice the IMPACT NORMAL we get, on the right! - this is used to rotate the VolumeSmoke container)*
