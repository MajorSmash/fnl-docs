---
doc_type: "SET_TOPIC"
title: "WATER"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/860172567658233866"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2021-07-01"
---

SET TOPIC: **WATER**
Ninja is slowly getting ready for watery things, here are the pre-requisites:
(0) Physics is already solved, via WorldSpace velocity (https://youtu.be/0O11SNavhM4?t=781)
(1) should look good from FPS view / low angle --- this is solved with 3D sim meshes, will be released in Live 1.4
https://youtu.be/YZHD-u5lClM
(2) should be able to handle reflection and refraction in the same time - think of a semi transparent water-surface that REFLECT the environment, but, you could see the REFRACTION-distorted bedrocks too --- currently, there is no good solution for this - using TRANSLUCENT domain materials, we have good refraction and see-through -- using OPAQUE mats, we have nice reflection (low roughness) - but there is no transparency. (See refractive examples: https://youtu.be/mEtGM6Zrr9I?list=PLVCUepYV6TvOrOfQVLMCxl_JoU_cIkK8P&t=188 --- https://youtu.be/0O11SNavhM4?list=PLVCUepYV6TvOrOfQVLMCxl_JoU_cIkK8P&t=1146 )

**CONCLUSION**: the combination of (0, 1, 2) would be enough for a decent local water container.

(3) Additionally, we need a sim container that follows the player, to have a non-local behaviour (pawn walks in shallow water)
https://discord.com/channels/850913821240983553/851787842182709268/852822829367164958
(4) Additionally, the waterline FX introduced by  could pimp the whole FX, in case our camera goes under-water
https://discord.com/channels/850913821240983553/850913821827792940/860147431617462303
