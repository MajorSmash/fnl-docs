---
doc_type: "SET_TOPIC"
title: "USING NINJALIVE FOR BAKING"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/866255962205978645"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2021-07-18"
---

SET TOPIC: **USING NINJALIVE FOR BAKING**
NinjaTools <:NinjaTools:851394765647118346>  and NinjaLive <:NinjaLive:851418299853045810>  are used in different workflows, and Live does not have built in baking support --> But, there is a back-door: a function that could write any simulation buffer (eg. density) to an EXTERNAL RenderTarget that is pre-made by the user, in the Content browser. The function is located at NinjaLiveComponent /LiveGeneric. Create a simple blueprint that (1) reads this RenderTarget every frame and (2) using one of the available blueprint nodes (eg. export RenderTarget OR convert RenderTarget) write frames to UASSETS or PNG files outside Unreal. By having a look at NinjaTools BP might give ideas how it could be done!
