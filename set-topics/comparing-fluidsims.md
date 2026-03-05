---
doc_type: "SET_TOPIC"
title: "COMPARING FLUIDSIMS"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1031990662633115668"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2022-10-18"
---

thanks for reaching out! --- I am doing a quick comparison for you!
1. **Niagara Fluids**: just perfect, generic solution, supports 2D and 3D fluids -- but it is more like a framework / not an "instant tool" -- say, you'd like to make you character interact with the fluid: you need to build your own fluid-simulation-emitters, and your own managing system that handles interactions. So, niagara is providing you with very good basic blocks - to build your own systems
2. **FluidFlux**: perfect if you are a looking for rivers and smaller water bodies --- and it is "out-of-the-box" --- and based on a 2D, 2.5D core technology - so very fast
3. **Zibra Liquids**: released for UE recently: it is a very performant, particle based 3D fluidsim, the visuals (yet) are a bit rough / you need to set 3D grid resolution to medium/lower values to have game-ready performance
4. **FluidNinja**: generic fluidsim (fire, smoke, clouds, rivers, lakes, particles, wind-for-foliage...etc), it is not only a framework, but a tool (has built in managers, presets) - so you don't have to build systems from scratch - also fast (being 2D, 2.5D) -- but NOT out of the box / takes weeks to learn
