---
doc_type: "SET_TOPIC"
title: "UNDERWATER"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1335898704569176125"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2025-02-03"
---

SET TOPIC: **UNDERWATER**
Underwater is solved with extreme simplicity:
1. we have a single PostProcessVolume (a box) that is placed "under water"
2. two special materials are applied to the postprocess volume
  - one material is imitating the underwater "fog" (distance visibility)
  - the other material is imitating the underwater caustics

To replicate this setup: simply copy-paste the underwater volume to your level.
(Optionally, you could tweak the materials. Learn more about caustics here: https://youtu.be/sdqVjyabVt4?si=J48oUKkPMXkzT2af)
