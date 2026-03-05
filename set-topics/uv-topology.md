---
doc_type: "SET_TOPIC"
title: "UV TOPOLOGY"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1022785306447069185"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2022-09-23"
---

SET TOPIC: **UV TOPOLOGY**
Ninja is a 2D sim - while it could be applied on non-planer objects - eg. a sphere or a torus - IT IS NECESSARY for the object (the TraceMesh) to have single, consistent, orthogonal UV space, with NO UV ISLANDS: with other words: you can not apply it to objects with random topology and UV islands (like a character, with separated limbs, and whatnot).
.
DESIRED UV TOPOLOGY:
