---
doc_type: "SET_TOPIC"
title: "BUGREPORT"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/850926358196125726/856543643090419762"
source_channel: "ninjalive-issues"
author: "andrasketzer"
date: "2021-06-21"
---

SET TOPIC: **BUGREPORT **(UE5 EA1 and EA2 velocity-related bug)

DESCRIPTION: "Get Physics Linear Velocity" and "Get Component Velocity" blueprint nodes return ZERO for non-physically moving (eg. animated or blueprint driven) objects. The above two nodes work as expected under UE 4.20-4.27: returning correct velocity values for any kind of moving objects.

BUG EFFECT ON NINJA: ninja massively utilizes obj.velocity to drive simulation. Under UE5 EA1, objects do not "drag" the fluid, they leave density marks, but no drag.
REPRO:  add a simple obj to a blueprint as a component, set position with time, and print "Get Physics Linear Velo" or "Component Velo" node output

CONCLUSION: Since (1) UE5 EA1 is a dead end, and (2) UE5 release1 will be continued from UE 4.27, and (3) the get velo feature is fine under UE 4.27... --- I will not try to fix this issue with a workaround. In theory, it will be "fixed" once they release a Ue 4.27 derived UE5

PS: of course, by storing current.pos / previous.pos we could generate velocity vectors ourselves - but this is not an option when tracking dozens of objects - I expect EPIC to fix this issue
