---
doc_type: "SET_TOPIC"
title: "MEASURING PERFORMANCE USING PROFILER"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/998958329307078746"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2022-07-19"
---

SET TOPIC: **MEASURING PERFORMANCE USING PROFILER**
1. Start Game
2. Start console by pressing "0"
3. Type: "stat startfile". Wait a few seconds. "stat stopfile". A detailed perfomance log has been recorded
4. Quit Game
5. Go Window / DeveloperTools / SessionFrontEnd. Choose the “Profiler” tab.
6. Load the above recorded stat log file ( Saved/Profiling/UnrealStats/UEDPIE… )
7. Look at the frame / framedraw time graph. Search for peaks. Click on a peak.
8. Below the graph, in the "Thread" window, start to open a hierarchical view of the per frame tick analisis.
*/GameThread/FrameTime/WorldTickTime/TickTime/TG_PrePhysics/.../FTickFunctionTask/...*
9. The tick-load list is arranged by "heaviest first".
10. Check the top items, they influence perfomance the most
