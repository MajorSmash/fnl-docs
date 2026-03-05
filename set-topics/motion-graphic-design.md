---
doc_type: "SET_TOPIC"
title: "MOTION GRAPHIC DESIGN"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/855134916170088459"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2021-06-17"
---

Welcome  🤓 
SET TOPIC = **MOTION GRAPHIC DESIGN** IN UNREAL

(1) the "Sequencer" is a classic keyframes-on-a-timeline tool that could be used to animate anything, from typo to objects to colors/materials. NinjaLive also could be controlled by sequencer - see chapter 23 in the manual (https://drive.google.com/file/d/1I4dglPjeXLcNkSGxGok8sQCy59qgYcF9) this video (https://youtu.be/dWJlKj446jQ), and Level5 Stage4 in the ninja project.

(2) UE 4.26 came with a new offline render: Movie Render Queue, that could render anything in high quality: resolution, DOF / motion blur / lighting all pumped to get "better than realtime" quality. Ninja works fine with MRQ - according to user reports, in some cases level-reload is needed to refresh some settings.

(3) Further UE topics to research: (A) virtual production (tracking a camera in realtime and adding elements / backplate to the incoming footage) --- (B) Paper2D for non-3D animation

(4) Courses: eg SchoolOfMotion - https://www.schoolofmotion.com/blog/motion-design-in-unreal-engine

(5) Workflow: I am also coming from mo-graph background (eg: https://www.youtube.com/watch?v=ZG72J2ylUGE ). - used to render passes (diffuse, Z-depth, color) in 3D programs (eg. 3dsMax) and use a Compositor (eg. After Effects) to make the whole thing work / do the post* / add typo. If I would be in this situation now, I would consider skipping the compositor entirely and do everything in UE...

(6) Postprocessing: *in UE, PostProcessMaterials and params could be animated as well like over-exposure, colour-filters and such. The postprocess properties could be spatially bind by a dedicated volume  (that could be infinite, so effects the whole scene) - or assigned to a given camera.
