---
layout: default
title: "Hemisphere Station: video"
tags: gamedev programming hemisphere
---

# A document about video decoding in general

Oh right, I'm making a game in C++ called ***Hemisphere Station***. Its' development will be available in this website through logs like this. Here's the *Brazilian Portuguese* title art.

![Br. Portuguese Title](https://cdn.discordapp.com/attachments/605879338067558401/617844428807340053/titleart.png)

So, what do you store your video on? The most known format for such a thing is *MPEG-4*, which is used everywhere by you and your family. However, in games, formats come in all shapes and forms, especially in the *90's*, where we just could not decide upon something. Sometimes it was just straight up some special format the company made for games.

Today, cutscenes and the likes use things like **RAD Game Tools' Bink**, which makes it easy to get in videos into games. However, you need a license for that. Do you think me, a 15 year old dummy making computer games on his afternoons, studying on the Bahian Federal Institute, can ever afford such a thing?! No! I'm very cheap, and this is my first *"for reals"* game. So I am scrambling for any open source thing to use.

![Cool name tho](https://cdn.discordapp.com/attachments/605879338067558401/617848779055562758/unknown.png)

Thankfully, **MPEG-1** has no patents! (So does **MP3** as of 2017, the more you know.) It is not the *best* format, and sort of not the *best open source video format* either (Ogg Theora decoders suck, no noticable VP9 decoder too) but it'll do the job for the moment.

Using the *just recently* released [pl_mpeg single file decoder](https://github.com/phoboslab/pl_mpeg) by **PhobosLab**, I managed to get an animated render I made of my character *Jim* and my best friend's one right on the game! Such a sight to behold.

![Beholding sights](https://cdn.discordapp.com/attachments/605879338067558401/617848301659750629/unknown.png)

I must personally thank the creator for including an OpenGL example, as it helped tons! The example had the 4x4 conversion matrix from *YCbCr* to *RGB* in the fragment shader itself, but since it is constant, I just put it in the implementation file for the video system to further cut down things on conversion (which is not cheap on the CPU!).

I also have already audio in with *OpenAL - Soft*, an open source implementation of *OpenAL*. Yep! OpenAL has some burocracy over it, and we all know how boring burocracy is. It was pretty straightfoward regardless.

I'll soon share more on other things. Stay tuned, readers! And have a nice day. :)

