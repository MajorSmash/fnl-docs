---
doc_type: "SET_TOPIC"
title: "LIVE 1.7 FEATURES"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/993771037286207589"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2022-07-05"
---

SET TOPIC:** LIVE 1.7 FEATURES**
This post is a replica of the new *Manual Chapter 29*, introducing new features
*Manual*: https://discord.com/channels/850913821240983553/850925841793941565/855091427393273866
*Playable mini demo*: https://kynolin.itch.io/fluidninja-live-17-demo (150 Mbytes, precompiled, EXE)
.
Live 1.7 is a major update
Features, **BRIEFLY**:
.
(1) driving other systems directly (no intermediate assets. eg RenderTargets)
(2) improved world-space motion
(3) local solver combined with global pattern generator → large responsive fields
(4) driving multiple systems with a single fluidsim (eg. surface + volume + particles)
(5) improved simple-mode: draw trajectories without running fluidsim (eg. footsteps)
(6) modularity: add others as Component to Ninja / add Ninja as Component to others
(7) niagara 2-way data flow: drive parcles using fluidsim / drive fluidsim using parcles
(8) tag based actor tracking
.
Features **EXPLAINED**:
.
**LIVE 1.7** FEATURES, PART1 --- **DIRECT DRIVE**
Ninja could drive volumes, particles, foliage, landscape and water surfaces.
Before 1.7, we used manually created intermediate assets to push data to other
systems: RenderTargets for sim.buffers, ParamCollecons for sim.pos & scale.
In 1.7, we provide ninja with (1) a material that is going to be applied to the target
system and (2) a **tag **to find targets → At init, Ninja is creating a Dynamic Instance of the
provided material, assigning it to targets with all params and buffers directly set
To drive Niagara: we don’t even need any material to set params

*See 20.3 and 24.1 in this PDF for Niagara and Volume setups.*

Note: Materials and NiagaraSystems used in the project are all prepared to handle the
incoming ninja data. Open up *NinjaLiveComponent Blueprint /MODULE023* to see the
standard param names. Top 3: *VelocityDensityBuffer, TraceMeshPos, TraceMeshSize*

Releted post, **TAGGING**: https://discord.com/channels/850913821240983553/850913821827792940/1000359069539913738
