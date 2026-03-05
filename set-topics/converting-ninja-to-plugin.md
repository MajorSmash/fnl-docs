---
doc_type: "SET_TOPIC"
title: "CONVERTING NINJA TO PLUGIN"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/875463777561247764"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2021-08-12"
---

Yes. I use the method in the PDF referenced in the main help document with a few small differences. The main one being `MatchSubstring=true` instead of false. I've been meaning to write down the exact steps in a document/post and/or figure out a way to automate the process. Right now I just have a quick note that reminded me of what to do, and I do it manually when I want to update the plugin in my general UE5 project.

Here's the general procedure I followed last night. Hopefully this helps you get it figured out.

1) New FluidNinjaLIVE project in UE4, enable the water plugin and add in UseCase003 (before converting the project to a plugin).
2) Follow PDF method with MatchSubstring=true. The part about opening each level isn't needed. I named mine FluidNinjaLiveVFX like it did.

```
[CoreRedirects]
#+PackageRedirects=(OldName="/Game/FluidNinjaLive/", NewName="/FluidNinjaLiveVFX/", MatchSubstring=false)
+PackageRedirects=(OldName="/Game/FluidNinjaLive/", NewName="/FluidNinjaLiveVFX/", MatchSubstring=true)
```
3) In the NinjaLiveComponent, change the default "preset search path" variable to /FluidNinjaLiveVFX. That doesn't get updated automatically by the package redirect portion.
4) Copy the Plugins/NinjaLiveVFX directory into the UE4/UE5 project directory. (It seemed to work by just dropping in the plugin created in UE4 into my UE5 project.)

There are a few optional extras I've been doing. I probably need to read through the known issues/tips again since this is just what I came up with on my own a little while ago.
||5) I've got a child BP of the NinjaLiveComponent in my project which didn't work with everything at first. In NinjaLiveComponent>CheckComponentOwner, I bypass the class check branch and feed the cast success/failed into the output node. (I can't remember if I tried testing it when the cast fails.)
6) I need to revisit the actual content/settings in my project, but my MetaHuman+ALS character causes the logs to go nuts with the nested skeletal meshes. So I add a DoesSocketExist check in "Calc Pos 5" of the NinjaLiveComponent and bypass the rest of the function if it doesn't. (Not saying that's an ideal method, rather a quick fix when I notice my logs are going crazy.)
7) In my project, I've got a custom trace channel already, so I need to update the Ninja default trace channel to be the FluidTrace. I also update the collision presets and defaults as needed for the trace component and interaction/activation volumes.
8) My project also has slightly different names for the input axes. So either update the third person character to use mine, or add in the inputs from the Ninja project's defaultinput.ini into my project's ini file.
9) My character doesn't work with the Ninja Utilities trying to possess the nearest pawn. So if I'm using my character in a tutorial level, I change the level to my game mode and disable possess nearest pawn in the utilities actor.||
