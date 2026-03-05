---
doc_type: "SET_TOPIC"
title: "FLOWMAPS"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/865940112394027078"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2021-07-17"
---

SET TOPIC: **FLOWMAPS**

Did you know, that all ninja projects have flowmap features implemented?

Shortly: add extra details to low-res sim output
With LIVE, it is spatial details. With TOOLS, not only spatial, but temporal:
a super-slowed basic sim extended with a fast-flowing detail map could result completely new qualities.

Explained: using sim velocity buffer as a flow map to advect a user defined map (typically procedural noise) - and mix the dynamically flowing details to the native simulation output

LIVE ------------------------- (feature added to ninjaLive 1.3)
References:
- Level 29 in the NinjaLive project
- Manual, Chapter 25 "Detail Maps" --- https://drive.google.com/file/d/1I4dglPjeXLcNkSGxGok8sQCy59qgYcF9
- ChangeLog, page 5 "Detail Maps" --- https://drive.google.com/file/d/17oVPVEoaW6Y6YKNISr4S0uUJY4_Yx_FM
- Tutorial video: https://youtu.be/v8d0CalL9oA?list=PLVCUepYV6TvOrOfQVLMCxl_JoU_cIkK8P&t=394
(Note: 3D volumetric noise flowing on clouds also belongs to this category, added to Live 1.2)

TOOLS ------------------------- (implemented since version 1.0)
References:
- Level "UseCases", multiple stages - eg. 8-frame pyro example
- Manual, page 6 "FlowPlay" --- https://drive.google.com/file/d/1eRQtcUtkkL6idelmbsfXCO03pbqBuwRu
- Tutorial video: "Using Flowmaps" --- https://youtu.be/5ZoVDdFQuoE
- Volumetric Fog technology plays simple flipbooks, and uses them to drive 3D VolumeFog - NO flowmap technology implemented in this case
- Volumetric Cloud technology plays flipbooks and uses them to drive 3D VolumeClouds - in this case, optionally, we could use flowmapping to advect a user defined 3D volume noise texture. You can set both the noise texture itself, and the parameters that influence noise-advection IN the VolumeCloud material instance. (Acces mate instance via the VolumeCloud Actor, placed on level  - little puff cloud icon).
