---
layout: default
title: "Russian Blocks: graphics"
tags: gamedev programming
---

# A series on making a clone of that game with the block shapes

So, I like Tetris. Tetris is cool.  There is a ton of tetris.

![Where it all went nuts.](https://cdn.discordapp.com/attachments/605879338067558401/607608024596742145/gb_tetris_p_twe54z.png)
![Cheeky name, visual/audio feast.](https://cdn.discordapp.com/attachments/605879338067558401/607608491351212042/tetriseffect_keyart_1200x675.png)
![Technically more of a Puyo-Puyo game, but still, Tetris. Double the fun.](https://cdn.discordapp.com/attachments/605879338067558401/607608730632060938/H2x1_NSwitch_PuyoPuyoTetris_image1600w.png)


## Why don't I make my own?
*Let's get to it!*

First, i'm doing this on **C++** using [*Simple Directmedia Library 2*.](https://www.libsdl.org/index.php) (current ver as of writting is 2.0.10!) Unlike OpenGL, which has time again absolutely owned my ass, SDL2 has been simple and nice, like the edges of a bevel'ed cube.

![A small reminder Blender, and the recently released 2.8 version rules.](https://cdn.discordapp.com/attachments/605879338067558401/607609997194559516/unknown.png)

I suggest you try to get a base going. I can get most of the code for a boilerplate off my mind easily, but I still gotta remember some stuff from other projects. This is not wrong to do! I used to think using tutorials n' stuff made me lazy and bad. Screw you, Impostor Syndrome. If you feel you've not learned, try to experiment with stuff. Make it do different things. You'll understand better by practice.

![A grey window, ready for blocks.](https://cdn.discordapp.com/attachments/605879338067558401/607610856963833888/RussianBlocks_2019-08-03_13-44-34.png)

That's cool, but what if we want some blocks? Well, first we need some images of them blocks. I made a spritesheet of them.

![Another small reminder, Aseprite rocks.](https://cdn.discordapp.com/attachments/605879338067558401/607611115861442569/Aseprite_2019-08-01_19-55-43.png)

Now we need to get them on our game! How? Easy! SDL2 has tons of contributed libraries that help it do more stuff, like [audio](https://www.libsdl.org/projects/SDL_mixer/), [networking](https://www.libsdl.org/projects/SDL_net/), and [image](https://www.libsdl.org/projects/SDL_image/) stuff!

