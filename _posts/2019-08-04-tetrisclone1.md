---
layout: default
title: "Russian Blocks: graphics"
tags: gamedev programming
---

# A series on making a clone of that game with the block shapes

So, I like Tetris. Tetris is cool.  There is a ton of tetris.

![Where it all went nuts.](https://cdn.discordapp.com/attachments/605879338067558401/607608024596742145/gb_tetris_p_twe54z.png)
![Cheeky name, visual/audio feast.](https://cdn.discordapp.com/attachments/605879338067558401/607619176860745728/Diesel2Fproduct2Fkiwi2Fhome2F10_EGS_enhance_tetriseffect_G2_gamepage_about_image_v2-28129-840x840-e9.png)
![Technically more of a Puyo-Puyo game, but still, Tetris. Double the fun.](https://cdn.discordapp.com/attachments/605879338067558401/607619400547434507/image.png)


## Why don't I make my own?
*Let's get to it!*

First, i'm doing this on **C++** using [*Simple Directmedia Library 2*.](https://www.libsdl.org/index.php) (current ver as of writting is 2.0.10!) Unlike OpenGL, which has time again absolutely owned my ass, SDL2 has been simple and nice, like the edges of a bevel'ed cube.

![A small reminder Blender, and the recently released 2.8 version rules.](https://cdn.discordapp.com/attachments/605879338067558401/607609997194559516/unknown.png)

I suggest you try to get a base going. I can get most of the code for a boilerplate off my mind easily, but I still gotta remember some stuff from other projects. This is not wrong to do! I used to think using tutorials n' stuff made me lazy and bad. Screw you, Impostor Syndrome. If you feel you've not learned, try to experiment with stuff. Make it do different things. You'll understand better by practice.

![A grey window, ready for blocks.](https://cdn.discordapp.com/attachments/605879338067558401/607610856963833888/RussianBlocks_2019-08-03_13-44-34.png)

That's cool, but what if we want some blocks? Well, first we need some images of them blocks. I made a spritesheet of them.

![Another small reminder, Aseprite rocks.](https://cdn.discordapp.com/attachments/605879338067558401/607611115861442569/Aseprite_2019-08-01_19-55-43.png)

Now we need to get them on our game! How? Easy! SDL2 has tons of contributed libraries that help it do more stuff, like [audio](https://www.libsdl.org/projects/SDL_mixer/), [networking](https://www.libsdl.org/projects/SDL_net/), and [image](https://www.libsdl.org/projects/SDL_image/) stuff!

It's easy to add them too! Just add the include and library paths, link the .lib file, and if needed, also drop the .dll on your project.

![Don't forget 'em, or get ready for link errors!](https://cdn.discordapp.com/attachments/605879338067558401/607612281055870982/unknown.png)

So how do we get our cool blocks in after that? Well, after you made sure it initializes and quits correctly, the image library can load stuff as a *SDL_Surface*. This format can be enough for some, but SDL has some cool features if you turn it into a *SDL_Texture*, like having a very versatile function to put your stuff on the screen, *SDL_RenderCopyEx*, which has things like rotation and flipping! Now that's awesome.

![No tension about SDL_Surface safety!](https://cdn.discordapp.com/attachments/605879338067558401/607612744652292136/unknown.png)
![Remember to free stuff after usage!](https://cdn.discordapp.com/attachments/605879338067558401/607614055158382622/unknown.png)

After loading in our blocks, and correctly setting up things for use with the *SDL_Texture*, there it is!

![Crisp and blocky!](https://cdn.discordapp.com/attachments/605879338067558401/607614363792048156/RussianBlocks_2019-08-04_01-18-15.png)

Why not play around with things?

![Every color, a new tier!](https://cdn.discordapp.com/attachments/605879338067558401/607614907990671360/RussianBlocks_2019-08-04_02-03-32.png)
![A t piece.](https://cdn.discordapp.com/attachments/605879338067558401/607615098479181824/RussianBlocks_2019-08-04_02-15-40.png)

Let's also make the board!

![Checkers in your block game? It's more often than you think.](https://cdn.discordapp.com/attachments/605879338067558401/607615228028649503/RussianBlocks_2019-08-04_02-46-08.png)

Soon enough, we'll start getting game logic up and what not. It'll be pure russian block fun, I'll say that. Stay tuned!
