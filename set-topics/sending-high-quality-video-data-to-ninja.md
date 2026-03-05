---
doc_type: "SET_TOPIC"
title: "SENDING HIGH QUALITY VIDEO DATA TO NINJA"
version_min: null
version_max: null
source_url: "https://discord.com/channels/850913821240983553/851482546100633601/1457450396187361586"
source_channel: "tips-tricks"
author: "andrasketzer"
date: "2026-01-04"
---

Hello Everyone!
I just recently started to experiment with FluidNinja - as a university student. It inspired me to come back to Unreal after a few years and I am very excited to try out this cool tool!

Are you interested in a little thing that I changed/added to the NinjaLiveComponent? And if so, then is this the right place to share it? 
Anyhow, I just share it now. 😄 
**FluidNinjaLive_1.9.54.4**

What I was also delighted to see coming back to Unreal that: the support for NDI and similar live broadcast sources became official in UE5.7. (Look for "NDI" and "Media Framework" plugins.)
These live sources now can be directly played back as MediaSource by MediaPlayer. Earlier you had to use third-party stuff or expose NDI to a RenderTexture and use it through that in Materials and such places... Now MediaPlayer is capable to open them in place.

As MediaPlayer is already supported by FluidNinja,** I wanted to add NDI as MediaSource through the MediaPlayer. **

First, there was a bit of troubleshooting regarding how MediaPlayers work and then see error dropped by** "Alternative inputs fed to Composite Density Input" function**.
Okay, I went in there and I saw that the currently implemented method is 
(Using the InputMediaPlayer + MediaTexture + InputMediaSource variables)
- Setting target MediaPlayer to the MediaTexture.
- Getting the URL from the MediaSource.
- Opening URL with the MediaPlayer.
- Play function on MediaPlayer. (And after that loop and rewind.)

**The overbridgethis, I added the upper branch.**
There a Playlist gets checked if it is valid and then opened by the MediaPlayer and push Play.
