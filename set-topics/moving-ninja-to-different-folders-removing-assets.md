---
doc_type: "SET_TOPIC"
title: "MOVING NINJA TO DIFFERENT FOLDERS / REMOVING ASSETS"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1052320271043932181"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2022-12-13"
---

SET TOPIC: **MOVING NINJA TO DIFFERENT FOLDERS / REMOVING ASSETS**
.
**(1)** ninja is a 2 year old project that vent from 0.9 beta to 1.8 --- though dozens of updates - and in some cases, assets are cross linked: later useceses utilze assets published by earlier usecases. For this reason...
**(2)** I adwise you to gradially remove assets (starting with levels, that are the main reference holders) in small steps by frequently using the REFERENCES graph. Contentwise, try to remove not-needed usecases first, moving towards tutorial levels (eg. you remove the LAVA usecase - none of the water useceses will complain). Probably a day's work - could shrink the current ~300 Mbytes data below 50 Mbytes (most of the data is examples and a minimal set of quixel assets like rocks, pieces of wood.... etc)
**(3)** Once done with the cleanup /data removeal ----> you could move on to changing folder form /Content/NinjaLive to somethign else: again, moving assets in small chunks, continuously FIXING REDIRECTORS. Note: NinjaLive Actor BP, NinjaLive Component BP and PReset Manager BP might contain SOFT REFS (asset names contained by STINGS): pls use the find-in-blueprints tool to look up soft-ref pathnames. One of these is prominently exposed in LiveComponent /LiveGeneric: PresetPath (default value is /Content/FluidNinjaLIVE/Presets)
