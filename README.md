---
layout: post
title: L.A.V.A.
date: 2018-04-10
categories: projects
description: L.A.V.A Stands for LED Aduio Visualizer with Acrylic. Using an arduino, a led strip, some coding in C++, and a CNC mill, you to can have you're very own L.A.V.A!
author: Mary Gentile
author-bio: First Year Human Centered Computing Major at Rochester Institute of Technology
author-email: mng7722@rit.edu
author-social:
    github: https://github.com/black_roses9995
---

## Background
I decided to make L.A.V.A. after a bunch of different (failed) interations. I knew I wanted my major project this year to be something that worked with Arduino's and my friend showed me this really cool project that used a whole bunch of things-and I was in WAAY over my head. Before December I had never touched an Arduino before. Before Spring break, I'd never coded in C++ before (I did have some C# experience, but not entirely applicable). I'm still amazed I was able to do this-and it works! 

## L.A.V.A

L.A.V.A. or LED Audio Visualizer with Acrylic, uses an arduino uno rev3, some jumper wires, a fully addressable LED light strip, a card that detects sound input, a trimpot for brightness control, three buttons; one to change the colour pallete, one to change the visualization effect, and then one that randomizes both a colour and visulization effect, and a lot of code.

I used the NeoPixel library to make working with the LED light strand super easy, but essentially what happens, is the mic is actively listening and picking up the "beat" of the song, which determines the visulization pattern (not the colour). This "beat" is put into a loop and replays over and over until a different "beat" or "bump" is detected, creating a new repeating loop. I coded 4 visulization effects:
    1: Pulse- the basic visulation, just pulses from the center of the strand. All LEDS are all ONE colour in this one
    2: PalettePulse- the second most basic. Just allows for a "gradient" to be applied to the LED strand while pulsing to the beat of the sound.
    3: PaletteDance-the whole gradient oscillates to the beat, similar to a snake, and holy code a moley. Got confused on this one a few times
    4: Glitter-(currently not working)creates a white sparkle on the palette to match the beat...but it's broken ATM.
    
I have 6 different gradients that I made up for the project-there's nothing really specially about this part, it just returns RGBs in a pretty pattern. I choose not to make any static gradients, but it is possible if you wish to do so.

In an effort to add more functionality, I used a trimpot to be able to adjust the brightness of the lights. However, I'm not entirely sure it's working to its full potentional. But it does work!

Here's a link to the full repository for the code: https://github.com/blackroses9995/LAVA/blob/master/LAVA.ino

Next I used a CNC mill to laser engrave an image onto an Acrylic sheet (NOTE: CANNOT be polycarbonate). This was probably the easiest part of the project, since all I had to do was pick an image.

And the last part is, making the wooden frame that houses L.A.V.A. I had practically ZERO experience with woodworking before starting this project and I have a HUGE shoutout to Tyler for helping me through it and making sure I kept all 10 fingers. I used a CNC Router to add groves to some wood (so that the acrylic sheet could slide in), then a table saw to to cut the wood in half vertically (that was scary as all living daylights), and a chop saw to cut them down to size, and finally a bandsaw to cut out indents in the top and bottom pieces of the wood so it would fit together. Before I added the back to the frame, I wrapped the LED strand around the inside back portion of the frame.

TL;DR: The project is a strand of fully addressable LEDs that lgiht up to the beat of the song, wrapped around an image laser etched into an acrylic sheet framed by wood. Looks cool man, I swear.


## Future Plans

This was definitely a labour of love (and confusion), but for the future, I'd love to make more visulization effects and possibly hang a permanment one on floor somewhere for all to enjoy (perhaphs with a remote control....:thinking-face:). I tried to do something I called "splatter", which would be kind of like glitter, but instead of a white dot, it would throw colour on that portion of the gradient. You know, like a paint splatter. But it didn't work... Just like my trimpot.

## What I learned, What I'd Change, and How Long it Took Me

I learned a crapton doing this project-from the basics of Ardruinos to how to code in C++ to rudimentry woodworking skills, and useful pieces of information such as, polycarbonate catches fire in a CNC mill and to always check for useful libraries before you begin coding. I spent roughly 6 hours on the woodworking portion, about 15 on the coding, 3 doing the acrylic, and then I don't even know how much on learning how to use the arduino-but it was a lot. Overall, I'd say the project took me roughly 25-30 hours over the course of 4 months.

If I were to change certain things about this project I'd make it smaller and changed the image I used on the Acrylic sheet. While it still looks SUPER cool, there's just too much going on in the picture to be able to make out the image in some of the visulization modes. I used a 11x14 acrylic sheet, and I'd probably use a 8x11 to reduce surface area if I were to redo it. 

## Well...What Does it Look Like?

Here's a link to a google drive folder that contains some images and even a video of L.A.V.A. in action: https://drive.google.com/open?id=1MgXokijKBwy1GRcLIgPdTrvH44kfoKoW
