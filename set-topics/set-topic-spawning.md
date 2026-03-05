---
doc_type: "SET_TOPIC"
title: "SET TOPIC: SPAWNING"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/850913821827792940/1079727716229709945"
source_channel: "general"
author: "andrasketzer"
date: "2023-02-27"
---

🖐️ very relevant questions! - **SET TOPIC: SPAWNING**
1. in our experience, using ninja as a **CHILD.ACTOR** was not working under UE4 --- and recently, seems to be working with UE 5.11 - see:
*\Content\FluidNinjaLive\Tutorial\UE_Mannequin_UsageExamples\ThirdPersonCharacter_NinjaAsChildActorComponent.uasset*
2. you could add a ninja **COMPONENT** to your actor - so they will spawn together
This tut.vid explains: https://www.youtube.com/watch?v=OP1e27Dvrlk&list=PLVCUepYV6TvPYbofpEf_ghznfihM-yt-B&index=21
3. You could spawn a ninja **ACTOR** and attach/parent it to your actor by code. See this example asset - and the screenshot below:
*\Content\FluidNinjaLive\Tutorial\UE_Mannequin_UsageExamples\ThirdPersonCharacter_NinjaSpawnedAttached.uasset*
