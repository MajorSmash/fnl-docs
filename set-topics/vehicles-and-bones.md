---
doc_type: "SET_TOPIC"
title: "VEHICLES and BONES"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/997841037353558117"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2022-07-16"
---

This is like the first time the PhysX/Chaos car has been the goal, not the unrelated problem. 🤣 I'm glad someone's actually tried the Chaos car.

You're on the right track. Historically, Ninja has only wanted to track bones for pawn collision types. I haven't yet reviewed the implications of vehicle collision types in 1.7 or tried using tags with vehicles, but it's certainly possible to use the vehicle collision type with a few BP tweaks. Otherwise, pawn is the way to go for now.

Since you have already tried pawn, I would think the issue is with the bone names. Check this section in the attached pic.

For flickering, the cause is usually two different systems writing to the same render target. Another copy/paste type of issue could be in-level object references like the light source provider. I haven't specifically checked if Andras updated UC5 to use the new systems. I do know I only updated the PhysX->Chaos parts for the car in UE5.
