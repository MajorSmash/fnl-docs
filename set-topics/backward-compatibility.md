---
doc_type: "SET_TOPIC"
title: "backward compatibility"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/994220122610864218"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2022-07-06"
---

SET TOPIC: **backward compatibility** --- 1.6  vs  1.7
Live 1.7 is backward compatible:
.
(1) *ninja-to-other.systems communication* (particles, volumes, surfaces)
While Live 1.7 favors DIRECT DRIVE (see Chapter 29.1 ) previous "RenderTarget and ParamCollections" based INDIRECT DRIVE setups also work.
.
(2) *moving in world.space:*
In Live 1.7 WorldSpaceOffset is automatic, by default - but you could switch it back to "manual" mode in case you'd like to use you manually set values --- see:
/LiveComponent /Liveinteraction /TraceMeshIsMovingInWorldSpace
.
