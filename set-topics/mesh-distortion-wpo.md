---
doc_type: "SET_TOPIC"
title: "MESH DISTORTION, WPO"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/850913821827792940/852809904175579136"
source_channel: "general"
author: "andrasketzer"
date: "2021-06-11"
---

SET TOPIC = **MESH DISTORTION, WPO**
 thanks for the warning: Dan Dokipen (of WETA) and  made me aware of the following changes / UE5:
(1) shader driven tessellation: discontinued
(2) displacement: discontinued
(3) Vertex WorldPositionOffset: supported, but early access (U5 EA1) automatically switches off Nanite for WPO-ed meshes: this is going to change in the final release (nantie and WPO will be friends)
(4) I have successfully tested the following solution under UE5: added pre tessellated base-meshes to ninja (plane, sphere, cylinder...etc) in various resolutions (100x100 to 500x500 vertex) - and IN CASE we would like to distort geometry, we (A) replace 1x1 (default) TraceMesh with one of these divided geometries, and (B) enable WPO in the newly modified Output Materials (Displace Removed, WPO added - similar params, all the same, looks the same)
The test linked yesterday is already captured from UE5 (https://discord.com/channels/850913821240983553/850913821827792940/852450465894498314)
