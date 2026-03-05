---
doc_type: "SET_TOPIC"
title: "WATER FOAM"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1181223435200892958"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2023-12-04"
---

🖐️ 
Yes: sim density is used to generate foam. Sim density comes from three sources: interacting object's brush-marks + a noise texture, added to the simulation + The output material. By removing the noise texture, and adjusting the output material, we could get rid of the "non interactive" foam. Steps:
Select ninja actor. Go to Actor Details Panel. Select ninja Component. Locate LiveGeneric Param Group. Locate "DefaultPreset" entry at the top. Double click the preset-asset. A data table pops up. Locate the "Density Template" entry. Delete the texture name (make the input field empty / the entry remains). Save the Data table. That's all.
