---
doc_type: "SET_TOPIC"
title: "MESH DISTORTION vs PARALLAX MAPPING"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/850926358196125726/1417479370393784351"
source_channel: "ninjalive-issues"
author: "andrasketzer"
date: "2025-09-16"
---

SET TOPIC: **MESH DISTORTION vs PARALLAX MAPPING**
**MeshDistortion** does what the name says: moves the vertices of the mesh - so objects (like the camera) could still collide with the new / modified surface. **Parallax Occlusion Mapping** (POM) *imitates* depth without changing the actual mesh geometry - so we could create a situation, where thew surface *seems* high (actually low), and the camera goes under the fake surface - as it is still colliding with the real mesh hull.  Since POM is fake: its usage is limited - not ideal for low-angle shots (when the camera is close to the surface). Minor improvements could be achieved by tweaking POM params in the output material.
