---
doc_type: "SET_TOPIC"
title: "SPAWNING/KILLING OBJECTS INSIDE NINJA INTERACTION VOLUME"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1262520765761458186"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2024-07-15"
---

1. ninja uses standard UE *triggerboxes* to detect objects, that overlap with the simulation.
2. UE triggerbox detects object that *enter* the box, or *leave* the box --- but: it does not detect objects that *spawn* inside the box (except at game-start) - also does not detect *destuction* ("killing") of objects. This behaviour is not ninja related: this is UE triggerbox behaviour. Problem: destroyed objects remain in the ninja "to be tracked" list.
Workaround: users need to create a mechanism that collects spawned objects, and adds them to ninja's "objects to be tracked" list:
(for destruction: a function, that *removes* killed actors from ninja's list of tracked components / SKmesh components)
