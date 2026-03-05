---
doc_type: "SET_TOPIC"
title: "SIM ACTIVATION"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1023610937363677297"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2022-09-25"
---

SET TOPIC: **SIM ACTIVATION**
There is a dedicated option, responsible for the sleep/wake state of sim containers.
This feature is based on pawn proximity: "if a pawn is nearby, wake the sim".
Sometimes, user defined characters does not qualify as "pawn" (eg.: their class definition is not CharacterMesh) - and for this reason, does not wake the sim 🙂
.
Of course:  you could SWITCH OFF proximity based activation.
Select NinjaLive Actor -- locate LiveActivation option at ther user details panel -- set "SimActivatedByPawnProximity" to FALSE
.
