---
doc_type: "SET_TOPIC"
title: "SETTING UP VOLUMEFOG"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1008725933794000936"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2022-08-15"
---

🖐️
Ninja supports 3 kind of volumetrics, you could read about these in the Manual, Chapter 24
https://discord.com/channels/850913821240983553/850925841793941565/855091427393273866
Looking at your screenshot, you are trying to set up a **VolumeFog** container.
1. There is a Viewport setting that enables / Disables Volumefog visualisation. Make sure it is on.
2. You need an Exponential Heightfog Actor on Level with VolumeFog enabled in the Actor Details
3. If point 1 and 2 are ok, we could move on to ninja volumes. Tutorial Level 23 displays volumefog setups. The first stage is a simple cylinder, with no fluidsim involved at all (made for testing, no ninia involved) --- to validate point 1, 2: do you see that cylinder, as seen on this video? -- https://youtu.be/C7mSXCOUQ5I?list=PLVCUepYV6TvPYbofpEf_ghznfihM-yt-B&t=65
4. IF YES, you could move on to manual chapter 24 to see how to set up Volumes.
+
Two related posts:
https://discord.com/channels/850913821240983553/851482546100633601/860217413761237023
https://discord.com/channels/850913821240983553/850913821827792940/887990556607782922
