---
doc_type: "SET_TOPIC"
title: "USECASE 15B - DIRECT DRIVING - knowhow"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/998742315671756901"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2022-07-19"
---

Live 1.7 is about "direct driving" --- too bad the sand-storm demo (Usecase 15B)- as the only exception - could not fully utilize this 🤣 
Why? 
1. we need to drive the landscape AND the volumesmoke. Fine. And we have two output-material slots. Fine. But...
2. for the landscape material, we need to INVERT the sim output - and this eats the primary out.material slot. 1st out is then channelled to 2nd.out.mat, which then, applies the mat on the landscape mesh. --- and no more slots left for poor volumesmoke ---- so... we need to drive it (vsmoke) the oldskool way> writing the sim buffer to en external RenderTarget - and make the vsmoke container read that.
.
Hope this helps! 😘
