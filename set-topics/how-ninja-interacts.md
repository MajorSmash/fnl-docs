---
doc_type: "SET_TOPIC"
title: "HOW NINJA INTERACTS"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1049606393101037578"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2022-12-06"
---

😉  I like your nick
Things "interact" the following way:
1. ninja is working in the background - detecting objects --> getting their position --> projects that to the simulation space --> running a sim ---> and then...
2. the sim output is applied to objects (eg. grass, water or landscape) - that SEEM to interact (it is really Ninja Actor that interacts, and Externals are just mapped with the sim)
3. technically, ninja applies the sim on things (grass, water) by FORWARDING THE SIM BUFFER AS A TEXTURE OBJECT PARAMETER to the materials that cover the external systems (grass material, water material.... etc)
4. The way to make objects "not-to-interact" is really simple: use materials that DO NOT CONTAIN parameters (does not contain the texture parameter object)
.
This video explains how it works: https://youtu.be/vXalfRAnXak?t=3240
