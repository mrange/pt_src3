# pt_src3.s aka Lance player

## 1993-08-22, Göteborg

![Chalmers Univeristy, Public Domain](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d3/Chalmers_University_of_Technology.jpg/1024px-Chalmers_University_of_Technology.jpg)


In my small university dorm room I completed pt_src3.s right before I was about to start my university studies at Chalmers.

pt_src3.s was the amalgam of all the best ideas I had seen for Paula emulators for Atari STE.

At the time of the release I felt the Atari STE was definitely fading away in favour of the PC. I thought pt_src3.s was a good paula emulator across several metrics but because of the disappearance of the Atari scene it would never see. I uploaded the pt_src3.s to ftp.sunet.se and ftp.funet.fi and turned off my Atari STE.

![Atari STF, CC-BY-2.5 Bill Bertram](https://upload.wikimedia.org/wikipedia/commons/3/39/Atari_1040STf.jpg)

## Summer 2000, Göteborg

I was now working as a junior software engineer for a company doing map engine and other consultancy work. I had forgotten about my Atari STE and pt_src3.s.

I was therefore very surprised when I was contacted over email by [Leonard](https://demozoo.org/sceners/2527/) asking my about pt_src3.s and if I could do something about the excessive memory usage of it for a demo he was creating.

We exchanged a few emails back and forth but basically came to the conclusion that speed of pt_src3.s came from lots of self-generated code and that making it 25kHz would be rather difficult and not reclaim that much memory.

He had some ideas on how to address the problem and I didn't hear much more.

I was later blown away about what he used it for when I saw [STNICCC 2000 Demo](https://demozoo.org/productions/59549/)([Youtube](https://www.youtube.com/watch?v=nqVJWFNpTqA&t=20s)).

![STNICCC 2000 Demo](images/stnicc.png)

A life-time achievment unlocked for me although I consider the Paula emulator a very small part of that demo.

I read [Leonards blog](http://leonard.oxg.free.fr/) and found the story about breaking an [old sprite record](http://leonard.oxg.free.fr/record16/record16.html) fascinating and it reminded me about my efforts that lead to pt_src3.s. I thought that I perhaps should write the pt_src3.s story.

This is my 10th attempt of writing that story.

## First steps

The first time I saw a computer (Commodore 64) I was hooked. I was drawn to computers instinctively.

![Commodore 64](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e9/Commodore-64-Computer-FL.jpg/1024px-Commodore-64-Computer-FL.jpg)

I almost exclusively played games but tinkered in basic programming but I didn't understand much. I was greatly disappointed after pain stakingly typing in a bubble sort routine and there was no bubbles to be seen on screen.

My mind was blown by the peek/poke listings so common in computer magazines.

![Code type in from biosrhythm.com](images/code-type-in.jpg)
> How can anyone program this way? It makes no sense.

Eventually I inherited my father's Atari 260 (extended to 1 Meg of RAM) and the monochrome hi-res monitor, 640x400 71 hz and paper white.

![Atari 520 ST with a monochrome monitor](https://upload.wikimedia.org/wikipedia/commons/thumb/5/51/Atari_520_ST_%2B_with_monochrome_monitor_SM_124.jpg/1024px-Atari_520_ST_%2B_with_monochrome_monitor_SM_124.jpg)
> The computer on the picture is an Atari 520 ST but the Atari 260 ST looked exactly like that except different model number.

I still mostly played games while tinkering with programming but didn't see much point in programming as I thought I could just buy the games I needed.

## Becoming a programmer

A very important turning point for me was a summer trip through Sweden with my family. We had a big american car which was odd in sweden and we went on a trip in it.

Before the trip my father had given me an advanced calculator that had a BASIC interpreter.

![Casio FX730P from www.calculatormuseum.nl/calculators/casio_fx730p1.JPG](images/casio_fx730p1.jpg)

As there was no games on the calculator I was learning BASIC while sitting in the back of the car during the summer trip and programmed a slot machine game, guess the number and a very simple shoot-em-up.

What I learnt was that I enjoyed programming and when I returned home I started doing [GFA Basic](https://en.wikipedia.org/wiki/GFA_BASIC) for fun.

## The Cuddly Demos around 1990

As I was interested in games and graphics after awhile I had moved on from [GFA Basic](https://en.wikipedia.org/wiki/GFA_BASIC) to [STOS BASIC](https://en.wikipedia.org/wiki/STOS_BASIC) which was a basic version intended to write games and graphics in.

![STOS loading screen](https://upload.wikimedia.org/wikipedia/en/a/a9/STOS_BASIC_loading_screen.png)

![STOS editor from www.atarimania.com](images/stos.gif)

However when a friend showed me [The Cuddly Demos by The Carebears](https://demozoo.org/productions/76257/)([youtube](https://www.youtube.com/watch?v=5pRelt_CPVk)) my mind was blown. I thought:

![The Cuddly demos from demozoo](images/cuddly_demos.png)
> I can never make this in STOS. I need to learn assembler!

I know now that people have done amazing thing in STOS, maybe even on the level of The Cuddly Demos but this is what got me into assembler programming.

## Dev Pac, I loved you

Lot of great Atari Software came through germany and somehow I got hold of a german version of [DevPac from HiSoft Systems](https://en.wikipedia.org/wiki/HiSoft_Systems). Which assembler is the best is subjective but I loved Dev Pac and the debugger.

![DevPac from atarimania](images/High_Devpac_02.jpg)
![DevPac debugger from atarimania](images/debugger.png)

I learnt the basics of assembler programming from [Svenska Hemdatornytt](https://sv.wikipedia.org/wiki/Svenska_Hemdatornytt)(Swedish home computer news) and their series "Learn assembler programming".

![Hemdatornytt from internet archive](https://archive.org/services/img/SvenskaHemdator1990-03/full/pct:200/0/default.jpg)

I still remember the intense feeling when I got my first scroll text working.

## Atari STE around 1991

The Atari 260 ST was aging, it had a few technical problems and I read about the new Atari STE which among other things had support for digital to audio signal conversion. This was possible on the old Atari ST but had to be emulated which took precious clock cycles.

My father got me a summer job on a oil tanker which itself was pretty cool but the important outcome was that I earned a bit of money and could purchase an Atari STE.

To help me unlock the power of the STE I had the book "Atari ST/STE - Hårdfakta" that had been updated to contain information about the STE specific hardware.

!["Atari Hardfacts"](images/hardfacts)

## TCB Tracker

The Carebears, which I idolized due to The Cuddle Demos, was releasing their own tracker called TCB Tracker. Trackers were a software common on the Amiga to make cool music.

The TCB Tracker was rumoured to have an STE enhanced mode that utilized the Atari STE new digital to audio soundchip.

![TCB Tracker from pouet.net](https://content.pouet.net/files/screenshots/00022/00022538.gif)

I was however not impressed by the sound quality. The sound was more crisp in the Atari ST mode compared to the Atari STE mode.

Analyzing the player code I found out why.

On the old Atari ST when you emulated a digital to analog soundchip you ran an interrupt on 10kHz as compromise between quality and speed. Each interrupt the next 8 bit sample was read and using "magic" (as in I never understood how it worked) the sample was translated to instructions to the Atari ST square wave sound chip that emulated a digital to audio conversion. It did sound surprisingly good often.

On the new Atari STE there was however a dedicated DMA that automatically read 8 bit samples from memory into the soundchip for you.

The only difference between the Atari ST and Atari STE mode in the TCB Tracker player code was that instead of the interrupt writing to the Atari ST chip it wrote the samples to a 2 byte looped area that sent the samples to the STE soundchip at 12.5kHz. Essentially the same architecture which makes sense I suppose.

A very simple change to make the sound more crisp was to switch the frequency from 12.5kHz to 50kHz (the highest supported frequency by the Atari STE).

However, in my mind in order to fully utilize the Atari STE an entirely new architecture has to be created. I decided to write my own player.

# NoiseTracker and Dr. Doom

Most songs, also known as modules, was not created in TCB Tracker. They were created in SoundTracker, NoiseTracker or ProTracker on the Amiga.

In order to get access to maximum amount of songs I wanted my player to be a NoiseTracker player.

But I needed someway to get me started.

![Tristar cracktro from youtube](images/cracktro.png)

Games were typically protected in various way to prevent piracy. These protections were removed and the games were released on "Compacted Disks" containing several games on a single floppy. This was called cracking a game and the people doing so often put a small "cracktro" with contact info, cool graphics and music before loading the game.

One of those was made by a Dr. Doom. I can't find an image of this cracktro but was special about it was that it had a decent STE player.

Using a home-grown memory scanner I managed to find the decompressed code in memory, save it and reverse engineered it.

The Dr. Doom player worked as I thought it should. It played NoiseTracker songs and it was architectured around the STE hardware.
