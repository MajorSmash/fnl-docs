---
doc_type: "SET_TOPIC"
title: "NIAGARA vs NINJA - MORE ON TWO WAY DATA FLOW"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/850913821827792940/1010575647900442685"
source_channel: "general"
author: "andrasketzer"
date: "2022-08-20"
---

🖐️ - thanks for leaving a note
.
SET TOPIC: **NIAGARA vs NINJA - MORE ON TWO WAY DATA FLOW**
1. RenderTargets (RTs) are like a "generic texture storage" - and could be used many ways
2. The "Direct Drive" technology, introduced in Live 1.7 aims to skip/eliminate additional RTs, by directly feeding target systems with sim data
     https://discord.com/channels/850913821240983553/851482546100633601/993771037286207589
3. There are cases, when the target system is a particle system: in these cases, Live 1.7 directly sends data to Niagara (RTs eliminated)
    See *Tutorial Level 20-A,B*, and *Usecase Level 11*
4. *Usecase Level 12* is COMPLETELY DIFFERENT: in this case, NIAGARA is feeding Ninja - particles are used as simulation input.
    Since ninja is second in the pipeline --- and niagara can not directly feed ninja - we are using RenderTargets as temporary storage.
5. The combination of pt. 3 and pt. 4 is called: TWO WAY DATA FLOW
    A.: ninja could drive particles /  B.: particles could drive ninja --- **it is very important to distinguish the two cases!**
    https://discord.com/channels/850913821240983553/851482546100633601/993780194034855997
