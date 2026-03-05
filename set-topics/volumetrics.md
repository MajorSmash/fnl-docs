---
doc_type: "SET_TOPIC"
title: "VOLUMETRICS"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/879327916176068609"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2021-08-23"
---

SET TOPIC: **VOLUMETRICS**
Both NinjaTools <:NinjaTools:851394765647118346> and NinjaLive <:NinjaLive:851418299853045810> contains true 3D volumetric shaders, could be lit with *point* and *directional* light and casts *self-shadows*. A crucial limitation is the SOURCE DATA that drives the volumetrics: ninja is 2D -- and this two dimensional data is SPATIALIZED as a height-map / elevation map ("extruded from the 2D plane") --- which has it's limitations, in turn, we have good performance. Transform: position, rotation, scale. Moar info - see *Manual, Chapter 24*.
https://drive.google.com/file/d/1I4dglPjeXLcNkSGxGok8sQCy59qgYcF9/edit
A few visual references:
https://youtu.be/iDir-ay8GVk
https://youtu.be/JNlGcKN-BN8
https://youtu.be/hHPma1YrczI
https://youtu.be/q-qKuU0SQfM
https://youtu.be/C7mSXCOUQ5I?list=PLVCUepYV6TvPYbofpEf_ghznfihM-yt-B&t=238
https://cdn1.epicgames.com/ue/product/Screenshot/02-1920x1080-45b755e2518694fc889606f2e3c532dc.jpg?resize=1&w=1600
https://cdn1.epicgames.com/ue/product/Screenshot/03-1920x1080-19b0ffee1f60d6eec553c9e3b33eb741.jpg?resize=1&w=1600
https://cdn1.epicgames.com/ue/product/Screenshot/009-1920x1080-5a6362250cdd39e38fb2da2aabf13d3f.jpg?resize=1&w=1600
https://cdn1.epicgames.com/ue/product/Screenshot/010-1920x1080-8575c9accc0c1caae598197b122745e2.jpg?resize=1&w=1600
https://cdn1.epicgames.com/ue/product/Screenshot/014-1920x1080-6a3378e7998166051557f8d610c93989.jpg?resize=1&w=1600
https://cdn1.epicgames.com/ue/product/Screenshot/015-1920x1080-7a7a6a0709da4cbbd1e4830f394a0b9e.jpg?resize=1&w=1600
