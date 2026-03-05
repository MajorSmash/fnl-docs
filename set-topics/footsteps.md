---
doc_type: "SET_TOPIC"
title: "FOOTSTEPS"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1083395771711365160"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2023-03-09"
---

🖐️ welcome --- I recall your question at the Marketplace --- and let us continue from there. 
I am including a picture (SEE BELOW), that will help us to understand this:
   1. the orange object the the leg of the character, moving up-and -down as he runs
   2. the green dot ts the BONE that we choose to track
   3. the yellow line is the TRAJECTORY of the bone
   4. the  blue box is the interaction-volume

Notice, how the bone is LEAVING the interaction volume at the top position.
When objects leave the interaction volume, they to not trigger painter and fluidsim response - hence, not leaving mark in the sand.
If a moving bone is inside the volume: it will trigger response, draw a mark on the floor.
Hope this helps! --- In case you are interested how to vertically fix the interaction volume and the sim:
https://discord.com/channels/850913821240983553/850913821827792940/1083393600580239483
