---
doc_type: "SET_TOPIC"
title: "INTERACTION"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/991680364084985929"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2022-06-29"
---

SET TOPIC: **INTERACTION**, TIPS

**First, testing:**
- add your interactors to the original, not merged ninja project and check: can you make them interact?
- try to make various object types interacting with merged ninja in your own project (default sphere, pawn, physicsbody...etc)

**Key settings:**
1.  interactors should have "Generate Overlap Events" flag enabled at their collision settings --- see *Tutorial Level 21, Stage 2*
2. the collision-profile defined *class *of your object (eg. PhysicsBody) and the *OverlapFilter *defined classes in ninja should match
3. *InteracationVolume*: make sure your interactors are inside the volume (in some cases, the tracemesh is used to detect overlap!)
4 In *Live 1.7* there is a new option to add interacting objects via **TAGS **- no matter what class they belong to. See bottom two ops on the screenshot:
.
