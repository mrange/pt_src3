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

!["Atari Hardfacts"](images/hardfacts.png)

## TCB Tracker

The Carebears, which I idolized due to The Cuddle Demos, was releasing their own tracker called TCB Tracker. Trackers were a software common on the Amiga to make cool music.

The TCB Tracker was rumoured to have an STE enhanced mode that utilized the Atari STE new digital to audio soundchip.

![TCB Tracker from internet archibe](images/tcbtracker.png)

I was however not impressed by the sound quality. The sound was more crisp in the Atari ST mode compared to the Atari STE mode.

Analyzing the player code I found out why.

On the old Atari ST when you emulated a digital to analog soundchip you ran an interrupt on 10kHz as compromise between quality and speed. Each interrupt the next 8 bit sample was read and using "magic" (as in I never understood how it worked) the sample was translated to instructions to the Atari ST square wave sound chip that emulated a digital to audio conversion. It did sound surprisingly good often.

On the new Atari STE there was however a dedicated DMA that automatically read 8 bit samples from memory into the soundchip for you.

The only difference between the Atari ST and Atari STE mode in the TCB Tracker player code was that instead of the interrupt writing to the Atari ST chip it wrote the samples to a 2 byte looped area that sent the samples to the STE soundchip at 12.5kHz. Essentially the same architecture which makes sense I suppose.

A very simple change to make the sound more crisp was to switch the frequency from 12.5kHz to 50kHz (the highest supported frequency by the Atari STE).

However, in my mind in order to fully utilize the Atari STE an entirely new architecture has to be created. I decided to write my own player.

## NoiseTracker and Dr. Doom

Most songs, also known as modules, was not created in TCB Tracker. They were created in SoundTracker, NoiseTracker or ProTracker on the Amiga.

In order to get access to maximum amount of songs I wanted my player to be a NoiseTracker player.

But I needed someway to get me started.

![Tristar cracktro from youtube](images/cracktro.png)

Games were typically protected in various way to prevent piracy. These protections were removed and the games were released on "Compacted Disks" containing several games on a single floppy. This was called cracking a game and the people doing so often put a small "cracktro" with contact info, cool graphics and music before loading the game.

One of those was made by a Dr. Doom. I can't find an image of this cracktro but what was special about it was that it had a decent STE player.

Using a home-grown memory scanner I managed to find the decompressed code in memory, save it and reverse engineered it.

The Dr. Doom player worked as I thought it should. It played NoiseTracker songs and it was architectured around the STE hardware.

I used the Dr. Doom player as basis for my own player and pt_src3.s is therefore ultimately a derivate of the Dr. Doom player.

## Amiga vs Atari STE

The Amiga had 4 independent digital to analog sound channels with pitch and volume control.

As much as we wanted the Atari STE to be an "Amiga killer" it didn't really deliver in that area as the Atari STE had 2 digital to analog sound channels with independent volume control and shared coarse pitch control. The replay frequency of the STE was 6kHz, 12.5kHZ, 25kHz and 50kHz.

50kHz replay frequency was significantly higher than the Amiga about max ~28kHz replay frequency but that was about it.

The NoiseTracker format is strongly coupled to the Amiga hardware as it has 4 independent channels and the values for pitch and volume can be copied into the Amiga hardware registers without modification (my memory is admittably a bit vague here).

In order to play Amiga Noisetracker the approach I went for was emulating the Amiga soundchip Paula thus pt_src3.s is a Paula emulator.

That meant I could use the Amiga NoiseTracker or ProTracker source code with just minor modifications to make them write to my "software" registers rather than the Amiga hardware registers.

In order to emulate the Paula soundchip on Atari STE you had to implement:
1. Fine grained pitch control per channel
2. Volume control per channel
3. Mix 2 channels into 1

Atari STE left and right channel are interleaved bytes like so:

```
------------------------------------------------
| Left  | Right | Left  | Right | Left  | Right
------------------------------------------------
```

One of my early attemps that wrote the left and right channel separately looked something like below.

```asm
; a0-a1 - points to sample                (2 channels)
; d0-d1 - fixed point offset into sample  (2 channels)
;  Top 16 bits is the fraction
;  Bottom 16 bits is the integer
; d2-d3 - fixed point pitch step
; d7    - number of samples to write
; a2-a3 - points to volume table          (2 channels)
.loop
move.b    (a0,d0.w),d4    ; Get sample for first channel
move.b    (a1,d1.w),d5    ; Get sample for second channel
move.b    (a2,d4.b),d4    ; Do volume calculation, divided by 2 implictly
add.b     (a3,d5.b),d4    ; Do volume calculation, divided by 2 implictly
                          ; adds the two samples to mix them
move.b    d4,(a4)         ; Store the sample in the output buffer
addq.l    #2,a4           ; The left & right channel are interleaved on STE
                          ; Therefore add with two
swap      d0              ; Restore the fixed point number
swap      d1              ; Restore the fixed point number
add.l     d2,d0           ; Add stepping speed for first channel
add.l     d3,d1           ; Add stepping speed for second channel
swap      d0              ; Restore the sample offset
swap      d1              ; Restore the sample offset
dbf       d7,.loop        ; Loop until frame is complete
```

This is not the very first version of the emulator as in the first version I also checked for the end of the sample at every sample but one of the very earliest optimizations I learnt about was extending the samples in the mod file with enough bytes so the end check could be done at the end of the frame rather at each byte.

It was a very significant improvement but still the code above is slow.

My 68k instructions timings is a bit rusty but I think the above code evaluates to about 124 cycles per sample written. To support 12.5kHz you need to write 25,000 bytes per second (1 byte per each channel) which is about 3,100,000 cycles which on an 8MHz Atari STE is about 39% CPU or 80% CPU for a 25 kHz.

25 kHz did sound pretty good but it took a significant amount of time.

## Impulse and the Brainless Institute Party - Going to my first demo party

![Impulse from Reine](images/impulse.jpg)

!["Young Nerds" from Reine](images/young_nerds.JPG)

I had a this time started to hang around with the guys in [Impulse](https://demozoo.org/groups/29352/). We are not talking TCB, TLB or Omega level here, not even close but we had fun and we went to our first demo party in Skövde together.

![Brainless from Reine](images/brainless_party.jpg)
> Brainless Institute party 1992

Being quite the introvert the demo party was stressful but also quite exciting to see so many nerds with similar interest. Where I lived at the time computers were rare and there was little interest in them.

I brought my NoiseTracker routine and while at the demo party I chatted with one of the organizer that later used it in a party demo which was cool. He also showed me the first trick of removing the end checks per sample. Since 25kHz was very time consuming he used the 12kHz mode.

## The 50kHz barrier

As 25kHz was lower than the Amiga's max frequency there was a case for making a 50kHZ player. I had tinkered with the code but couldn't make it fast enough. After some failed attempts I had concluded it was impossible.

I was therefore very surprised when I at the demo party saw Audio Sculpture which claimed to have a 50kHz mode.

![Audio Sculpture tracker from pouet](https://content.pouet.net/files/screenshots/00029/00029334.png)

As many hackers I had already developed a bit of an unmotivated ego and seeing someone else achieve what I thought was impossible was a blow to that ego.

But it started a very important process in the brain. It is obviously possible to do 50kHz player. With that knowledge the brain starts looking for cheats and can find one that it previously didn't see.

I have felt that multiple times since then. "This can't be improved". Then someone shows an improvement and that in term leads to a new solution that is even better and so on.

A friendly competition can be very fruitful for everyone.

## Self-generating code and cheating

I managed to get a copy of the Audio Sculpture software and was experimenting with it. It did sound a lot like 50kHz so they had done it but I noticed that the pitch seemed to be fixed in steps. That did sound great for some songs but not all.

So what I suspected they done is that they used self-generating code to generate code to avoid pitch computation per sample but for memory reasons couldn't get the full pitch range of Amiga.

Here I believe I took a step in a direction most players didn't which later enabled pt_src3.s.

My thoughts were something like this.

With the base frequency of 50kHz if I am to play a sample at 29kHz I need to "stretch" 29000 bytes over 50000 bytes per second or 580 bytes over 1000 bytes if we run the player each frame (1/50th of second).

The maximum amount of steps of the input sample is 580 bytes per frame and the lowest about 75 bytes per frame.

I don't have enough memory to generate code 505 (580 - 75) methods.

However what I can do is splitting the frame into smaller subframes of say 100 bytes. I then need to step between 7 to 58 steps or 51 different methods. I then stitch the subframes together into the final frame.

My player during initalization generated 51 different methods that "optimally" stepped between 7 and 58 steps.

If I during a frame needed to step 145 steps I switched between calling the 14 and 15 step function so I ended up at 145 steps in the full frame.

The first attempt looked something like

```asm
move.b  $X(a0), d0      ; Read sample
move.b  (a1,d0.b), d0   ; Do volume calculation, divided by 2 implictly
move.b  d0, $Y(a1)      ; Write sample
```

This isn't valid 68K code in that the X and Y is undefined but what you did was that you during the init step computed the corrected offsets and wrote assembly code to a method that would then look like this in the case we want to step 50 times over 100 bytes written.

```asm
move.b  $0(a0), d0      ; Read sample
move.b  (a1,d0.b), d0   ; Do volume calculation, divided by 2 implictly
move.b  d0, $0(a1)      ; Write sample

move.b  $0(a0), d0      ; Read sample
move.b  (a1,d0.b), d0   ; Do volume calculation, divided by 2 implictly
move.b  d0, $2(a1)      ; Write sample


move.b  $1(a0), d0      ; Read sample
move.b  (a1,d0.b), d0   ; Do volume calculation, divided by 2 implictly
move.b  d0, $3(a1)      ; Write sample

move.b  $1(a0), d0      ; Read sample
move.b  (a1,d0.b), d0   ; Do volume calculation, divided by 2 implictly
move.b  d0, $4(a1)      ; Write sample
```

This wrote the first channel, then we need a slightly different version that mixed the second channel.

```asm
move.b  $X(a0), d0      ; Read sample
move.b  (a1,d0.b), d0   ; Do volume calculation, divided by 2 implictly
add.b  d0, $Y(a1)       ; Mix sample
```

This was a significant improvement in performance in about 88 bytes per sample written meaning the 25kHz routine "just" takes 55% CPU time down from 80%.

But 55% is still too high as 50kHz would then take 110%.

However, there is unnecessary work done that can be eliminated.

```asm
move.b  $0(a0), d0      ; Read sample
move.b  (a1,d0.b), d0   ; Do volume calculation, divided by 2 implictly
move.b  d0, $0(a1)      ; Write sample

move.b  $0(a0), d0      ; Read sample
move.b  (a1,d0.b), d0   ; Do volume calculation, divided by 2 implictly
move.b  d0, $2(a1)      ; Write sample
```

We read the same byte twice and compute the volume twice. Instead what we can do is this.

```asm
move.b  $0(a0), d0      ; Read sample
move.b  (a1,d0.b), d0   ; Do volume calculation, divided by 2 implictly

move.b  d0, $0(a1)      ; Write 1st sample
move.b  d0, $2(a1)      ; Write 2nd sample
```

So with that modification the worst case of 580 sample reads per frame and 1000 writes would then mean approximately ~64 clockcycles per sample written or about 80% CPU for a 50kHz player.

Often it take less CPU if channels uses a lower pitch, which is the reason for  pt_src3.s signature fluctating CPU usage. Not necessarily a good thing unless you have some way to average it out.

With this technique I was able to implement my first 50kHz routine that had a fine-grained pitch.

I was very satisified.

## Utilizing the LCM1992

I was satisifed with the player but I continued tinkering on it as there was now several good 50kHz players out there.

The Amiga had 4 channels with independent pitch and volume control. The pitch control on Atari STE was to coarse to help but there was independent volumne control for left & right channel on STE through a chip known as the LCM1992.

The chip was finicky to use and I was confused with documentation on how should translate the Amiga volume control to the LCM1992 but after recomputing the tables in the documentation it was a fairly straight forward linear relationship.

But since I mixed two channels together in order to make use of the chip I had to select the channel with the highest volume, set the LCM1992 to the matching volume and recompute the secondary channel volume in relation to it.

This means the code for the primary channel looked something like this for 25kHz

```asm
move.b  (a0)+, d0       ; Read sample, on 50kHz player one could post increment
                        ; the register to save clock cycles
move.b  d0, $0(a1)      ; Write sample
move.b  d0, $2(a1)      ; Write sample
```

The secondary channel looked something like this
```asm
move.b  (a0)+, d0       ; Read sample, on 50kHz player one could post increment
                        ; the register to save clock cycles
move.b  (a1,d0.b), d0   ; Do volume calculation, divided by 2 implictly
add.b   d0, $0(a1)      ; Write sample
add.b   d0, $2(a1)      ; Write sample
```

With these improvements the player landed on about 63% CPU for 50kHz player.

## ProTracker and the magic E instruction

Up to this point I had written and maintained a NoiseTracker player based on Dr. Doom player which was reasonably compliant and performant.

![ProTracker for Amiga](images/protracker.png)

But ProTracker was taking of more and more on the Amiga scene and many modules didn't sound quite right with NoiseTracker.

I tried to implement the ProTracker player but I ran into serious issues with the E instruction which in NoiseTracker was quite simple but in ProTracker could do weird things.

There was especially one effect where I just couldn't understand the code.

In the end I gave up and pt_src3.s contains a slightly patched ProTracker player plus my Paula emulator.

The ProTracker code wasn't very fast but I accepted that compared to the Paula emulator the tiem it took wasn't very relevant.

## The Gurgelkvack "convent" 1992

![Gurgelkvack "convent" from Reine](images/gurgelkvack.jpg)
> We learnt later that "convent" in english didn't mean what we thought it did.

Summer 1992 Impulse arranged the first Impulse demo party. We had great ambitions but not many turned up. Still we had fun and in the end I think we all thought it was a success. The pizza guy was less pleased as he had stocked up in anticipation of several hundred hungry nerds buying pizza.



## Motorola Inside'93

![Nerds playing games](images/motorola_inside.JPG)
> Me holding my beloved calculator, Johan is playing some game.

Because Gurgelkvack'92 was fun we followed up next summer with Motorola Inside'93.

Here [Excellence in Art](https://demozoo.org/sceners/2101/) released his [TalkTalk](https://demozoo.org/productions/59421/) demo which because I thought was outstanding not only because it used a version of my player, or that it was released at our lame party although it certainly helped.

I think [TalkTalk](https://demozoo.org/productions/59421/) has a cool and for its time ground-breaking design and still enjoyable to watch. As a hacker very entrenched in writing optimized code and hardly being able to finish anything because of it this was an eye-opener for me.

Code don't matter, what matter is the impression you make and [TalkTalk](https://demozoo.org/productions/59421/) made a significant impression on me.

Another important event for me at Motorala Inside'93 was a chat with [Blade](https://demozoo.org/sceners/2500/) from [New Core](https://demozoo.org/groups/2218/) where we discussed STE players. [Blade](https://demozoo.org/sceners/2500/) later released [Octalyzer STE](https://demozoo.org/productions/73259/) so he is very knowledgeable.

The [Blade](https://demozoo.org/sceners/2500/) player was very performant and utilized an improved way to calculate volume. If I remember correctly at the time it looked a bit like this

```asm
move.b (a0)+,d0   ; Read channel #0, uses LCM1992 for volume control
move.b (a1)+,d1   ; Read channel #1
move.l d1,a5      ; Move d1 to a5 to read indirectly
add.b (a5),d0     ; Read volume corrected sample and mix with channel #0
move.b d0,(a4)+   ; Write left channel
move.b (a2)+,d0   ; Read channel #2, uses LCM1992 for volume control
move.b (a3)+,d2   ; Read channel #3
move.l d2,a5      ; Move d2 to a5 to read indirectly
add.b (a5),d0     ; Read volume corrected sample and mix with channel #2
move.b d0,(a4)+   ; Write right channel
```

The [Blade](https://demozoo.org/sceners/2500/) player of course relied on self-generating code and as a preprocess step it wrote the post-increments from a frequency table into the code so the input samples was stepped correctly.

The code about takes about 45% CPU and the preprocess step took as far as I remember around ~10% so in total 55% CPU which was faster than my currently best player.

# A sleep deprivation induced epiphany

I left [Blade](https://demozoo.org/sceners/2500/) and walked to my place.

The [Blade](https://demozoo.org/sceners/2500/) player was good, perhaps too good. I didn't like it obviously as I had a hacker ego.

I was tired due to not sleeping which is the custom at demo parties.

My player had some advantages in that it would optimize sample reads but it was slow on mixing. The [Blade](https://demozoo.org/sceners/2500/) player that mixed all channels at once could avoid reads and writes that way.

I was thinking to myself that even if I incorporated the improved volume calculation my player might be faster for certain songs but not overall.

*I needed something new.*

At that moment the entire design for pt_src3.s came to me. I knew how I would eliminate a lot of waste and the result would combine the benefit of my player with the benefit of the [Blade](https://demozoo.org/sceners/2500/) player.

The code would be much more complicated than any of my previous players and consume a lot of memory but it was doable.

I just had one big problem that was I unsure if it even had a solution.

# The creation of pt_src3.s

The key improvement of pt_src3.s over my old players is that instead of taking 1 channel at a time pt_src3.s takes 2 channel at a time.

That eliminates the need to read the sample from output buffer and mix it again.

It does complicate things though and I had split into even smaller subframes to not run out of memory.

Each subframe is now 40 bytes and for each channel the player stepped between 3 to 26 bytes so it needs 23 combinations per channel that is 23*23 = 529 methods.

Then depending on the channel pitch the player pick the correct combination and mix two channels at the same time. The player handles fractional steps by switching between different combinations per subframe.

This means the resulting code looks something like this in the case we are going to repeat each sample 3 times.

```asm
move.b  (a0)+, d0   ; Read channel #0
move.b  (a1)+, d1   ; Read channel #1
move.l  d1, a3      ; Blade's improved volume calculation
add.b   (a3), d0    ; Mix channels
move.b  d0, $0(a2)  ; Write sample
move.b  d0, $2(a2)  ; Write sample
move.b  d0, $4(a2)  ; Write sample
```

But the player also optimized reads when the channels went in difference pace.

Let's assume channel #0 repeat each sample twiche and channel #1 repeats each sample 10 times.

```asm
move.b  (a0)+, d0   ; Read channel #0
move.b  (a1)+, d1   ; Read channel #1
move.l  d1, a3      ; Blade's improved volume calculation
move.b  (a3), d1    ; Read volume corrected sample
add.b   d1, d0      ; Mix channels
move.b  d0, $0(a2)  ; Write sample
move.b  d1, $2(a2)  ; Write sample

move.b  (a0)+, d0   ; Read channel #0
                    ; d1 already contains the correct sample
add.b   d1, d0      ; Mix channels
move.b  d0, $0(a2)  ; Write sample
move.b  d1, $2(a2)  ; Write sample
```

That way the player ended up reading close to optimally.

The code got a lot more complex but the performance started to look real good.

But I still hadn't solved a big problem.

## Reading the manual out of desperation

The problem was writing the samples was slower than the Blade player. The Blade player could utilize post increment of the address register when writing the samples which gave a free increment.

I had to use indexed writes which was 4 cycles slower and took more memory.

4 cycles don't sound too bad but since the player had to write 100,000 samples each second those 4 cycles was 5% lost CPU time.

Very annoying.

So I read the 68000 manual in some vain hope there was some hidden address mode I didn't know about that could help me.

I guess I got lucky because I found a gem.

Up to this point I think my players didn't feature anything unique. They were ok and pt_src3.s would be good but thanks to combining a bunch of ideas into one complicated mess.

However, what I found I think is a trick seldomly used and I certainly hadn't seen it before.

The problem was this.

I wrote the left and right channel separately. Because the channels were interleaved I needed to write a byte and increment by 2.

If I did `move.b d0,(a0)+` a0 is only increment by 1. Not good.

If I did `move.w d0,(a0)+` a0 is incremented by two but it only works for the right channel as it overwrites the higher byte and in addition if a0 is an odd address the 68000 throws an exception.

So I did `move d0,$0(a0)` and used self-generating code to generate increments by 2 but this took 4 cycles extra and took more memory.

What I found was a peculiar property of the stack pointer. In order to protect the stack pointer from ending up pointing to an odd address which would crash if you tried to push a 16bit or 32bit word if you did `move.b d0,(sp)+` the stack pointer was actually incremented by 2!

What I didn't know was what happened if the stackpointer was an odd address already, would it increment by 1 or 2?

It turned out it incremented by 2 regardless if the stackpointer had an even or odd address which is _exactly_ what I needed.

Now the code became something like this:

```asm
move.b  (a0)+, d0   ; Read channel #0
move.b  (a1)+, d1   ; Read channel #1
move.l  d1, a3      ; Blade's improved volume calculation
add.b   (a3), d0    ; Mix channels
move.b  d0, (sp)+   ; Write sample
move.b  d0, (sp)+   ; Write sample
move.b  d0, (sp)+   ; Write sample
```

Most of the player code needs to run into the 68000 supervisor mode in order to access the sound chip hardware. Putting the supervisor stackpointer to an odd address is not the best in case there's an interrupt and the 68000 tries to write return addresses to the stack. That will crash.

That's why pt_src3.s very randomly switches to user mode in the middle of it all. The usermode stackpointer can "safely" point to an odd address. To switch back to supervisor mode the trap #0 vector is setup to point to the continuation.

## Post Scriptum: Legacy

## Post Scriptum: My Monochrome screen
## Post Scriptum: 50 kHz Octalyzer plugin
## Post Scriptum: Solving the spikeness
## Post Scriptum: Amiga Octalyzer plugin
## Post Scriptum: pt_src3.s refactored
## Post Scriptum: How do you get started today?
## Post Scriptum: Shaders
