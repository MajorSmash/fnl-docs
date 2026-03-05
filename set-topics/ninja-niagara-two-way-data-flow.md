---
doc_type: "SET_TOPIC"
title: "NINJA-NIAGARA - TWO WAY DATA FLOW"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/933350032323788861"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2022-01-19"
---

SET TOPIC: **NINJA-NIAGARA - TWO WAY DATA FLOW**
Using ninja and niagara together could work two ways!
.
(1) using fluidsim OUTPUT -- to drive particles - see *Tutorial Level 20A,B*  and  *UseCase Level 11*
(2) using particle system OUTPUT -- to drive fluidsim - see *UseCase Levels 12 + extension*
Note: the setups needed to manage these data flows are completely different!
.
**(1)** This is how it looks like: 
https://youtu.be/mEtGM6Zrr9I?list=PLVCUepYV6TvPYbofpEf_ghznfihM-yt-B&t=90
https://youtu.be/v8d0CalL9oA?list=PLVCUepYV6TvPYbofpEf_ghznfihM-yt-B&t=939
https://youtu.be/Y_1fwEHvrrE
Related downloadable usecase package: https://discord.com/channels/850913821240983553/850913821827792938/916342949321781278
**Technically**: falls to the classic "RenderTarget pairing" protocol (make sure ninja writes the same RT that is being read by niagara, make sure that multiple ninja is NOT writing the same RT). See related posts:
https://discord.com/channels/850913821240983553/851482546100633601/881167786724966440
https://discord.com/channels/850913821240983553/851482546100633601/885512724958834708
.
**(2)** This is how it looks like: https://youtu.be/nZoZwP-jUkM +++ https://youtu.be/Pl2TeWZt8wc +++ https://youtu.be/5M-z__oSmDs
Related downloadable usecase package: https://discord.com/channels/850913821240983553/850913821827792938/923792511116378142
**Technically**: UC12 is new and experimental, While RT-pairing also applies: note that ninja is using the MATERIAL input to get niagara output --- so: niagara writes to a given rendertarget, and A MATERIAL IS SET TO READ THIS RT, and ninja is set to use this material as input for sim.
FLOW: Niagara -> RenderTarget -> Material (RT as emissive, unlit, support negative emissive if you want to overdrive) -> NinjaLiveComponent Input material (RGB).

Tutorial videos on UC 12 technology:
- https://youtu.be/yzDwi3ps7aI?t=643
- https://youtu.be/LdrkKUJYBWc
- https://youtu.be/3cBo9pHUXUA?t=1187
.
