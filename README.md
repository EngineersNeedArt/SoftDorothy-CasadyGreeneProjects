# Soft Dorothy Software — Casady & Greene Projects
A disk image (intended for emulators) containing code and tools for building the commercial games John Calhoun wrote for **Casady & Greene, Inc.**

I wanted to capture in one place the sources to the early Macintosh games I published with Casady & Greene Inc. as well as the old build environments (THINK C, THINK Pascal, CodeWarrior, ResEdit) and put these on a disk image suitable for the current early Macintosh emulators. The disk image (zipped to save space) can be downloaded and then you should be able to mount it in <a href="https://basilisk.cebix.net">Basilisk II</a>, <a href="https://sheepshaver.cebix.net">Sheepshaver</a> or <a href="https://www.gryphel.com/c/minivmac/">MiniVMac</a>. Opening one of the game projects should then allow you to edit, compile, and run the game in the same way I did in the 1990's.

Below, in order of release, are the sources included on the disk image.

### Glider 4.0

**Glider 4.0** was the first game I had published commercially. I had seen ads in magazines for a few games published by **Casady & Greene, Inc.** (C&G) and reached out to them to see if they were interested in **Glider**. I suggested I could write a commercial version of **Glider** to support color and that the game would have a "house" (the game levels) with some forty or so rooms (the shareware game had only ten or fifteen rooms as I recall). They agreed and so advanced me enough money to buy a color Macintosh and a color display.

<p align="center">
<img width="752" src="https://github.com/EngineersNeedArt/SoftDorothy-PublishedProjects/blob/b365778f5129970dbb572805d3c252235d49d766/Images/BasiliskIIScreenshot.jpg">
</p>

I believe I more or less finished **Glider 4.0** around the beginning of the fall of 1991. That fall I was in my last year of an Education degree at the University of Kansas. I student-taught that last year and I recall telling my high school students that I had a Macintosh game being published, ha ha.

The "houses" for **Glider** are like a collection of *levels*. I determined pretty quickly that creating a "level editor" for **Glider** would make it much easier for me to create the promised house of forty or more rooms. And so the creation of both **Glider 4.0** and a **House Editor** began more or less at the same time.

I could have kept the **House Editor** as an internal tool but I thought that if users had access to the same "level editor" it would make **Glider** more fun.

I found out very quickly though that work on the **House Editor** in fact involved more work than **Glider** itself. It turned out that "idiot proofing" the editor required a lot of sanity checking and busy work. As an example, when a user adds a bouncing ball to a room, there is a "Get Info" dialog box that allows you to edit various parameters of the ball such as the **Length of travel**. When a user entered a value I had to make sure it was not negative, not too large for the room. These kinds of sanity checks are all over in the code and required a lot of busy effort.

<p align="center">
<img width="752" src="https://github.com/EngineersNeedArt/SoftDorothy-PublishedProjects/blob/265b7f87d170fb85c75443b5152532326113aea5/Images/GliderEditorScreenshot.jpg">
</p>

**Glider 4.0** 4.0 went on to win a MacWorld Game Hall of Fame award. I graduated with my Education degree but as a result of **Glider** having been published I decided to put off teaching — at least for the time being. The game-programming gig would likely be brief and teaching would still be there in any event.

Serendipitously, AOL (America On-Line) had become a thing about that time and **Glider 4.0** houses that people had created with the **House Editor** started being uploaded and downloaded. I was surprised to see the small community that built up. Even a fan newsletter appeared for a time. If creating new houses was not your thing, **Glider** could still have a longer shelf-life by downloading and playing houses that *others* had created.

### Pararena 2.0

**Pararena 2.0** was the second game I wrote that was published by C&G. It came about after the success of **Glider** when C&G asked, "What else you got?" I had my doubts about **Pararena** but the shareware version had something of a small but dedicated fanbase. I imagined that in addition to color, perhaps I could add enough additional features to make it more commercially viable. The dates on the original files suggest the game was written in July of 1992, roughly a year after **Glider 4.0** was written. 

<p align="center">
<img src="https://github.com/EngineersNeedArt/SoftDorothy-PublishedProjects/blob/fff10d77b13afe2aff30a19739a52d47cb835fb4/Images/PararenaRejectedSplashScreen.png">
  <br>
<em>Casady & Greene rejected this splash screen.</em>
</p>

**Pararena 2.0** was to be another first for me — I was intending to write it in the C language rather than in Pascal (which all my other games had been written in). Once again my shareware game, **Glypha**, became my testing ground. I rewrote **Glypha** in C and "shipped" it before beginning my first *commercial* C application. And again, **Glypha** written in C was well received and **Pararena 2.0** would later ship with no problems that resulted from my haviung learned a new programming language.

Some thing I added to hopefully give it more commercial-game gravitas was an "instant replay" that showed, TV-style, the seconds leading up to a scored goal. I also added several computer opponents that varied from novice to expert-level players. There were tournaments and awards you could try to attain within the game. And finally there was a rudimentary network option where two Macintoshes connected by a null-modem cable (and perhaps a bit of luck) could play **Pararena 2.0** head-to-head, human vs. human.

Despite all of the above though, **Pararena 2.0** never made even 10% of what **Glider 4.0** had made. It was not going to be possible to live on the royalties if game sales followed in **Pararena's** footsteps. I reminded myself though that I still had the Education degree and could always begin my teaching career.

### More Glider

**More Glider** is not a programming project like the others on the disk image but is included more for completeness. When the floppy disk for **More Glider** shipped it contained a new house I had created — one I made intentionally difficult to give the better **Glider 4.0** players a run for their money. I also had tweaked a lot of the game artwork from **Glider 4.0** and included the alternate artwork in files that you could swap for the existing artwork files.

Additionally, there were a number of "houses" (**Glider** levels) that users had created. Each of the individuals that had created the houses we shipped were asked for permission to ship them, were given a payout of some cash as I recall, and were able to include a "READ ME" where they describe their houses. Some of the creators I would contact again a year of so later when I was beginning the follow-on to **Glider 4.0**, **Glider PRO**. The "house" that shipped with **Glider PRO** would end up being a collaborative effort between myself and three other **Glider** fans.

### Glider PRO

Writing **Glider PRO** was to return to the one game that I had done that had seen some popularity. Even as I was writing it though I had a growing sense that the window for the "indie" game writer was coming to a close. LucasArts, just to pick one, were coming into the computer game market with all their art talent and resources (and franchise) behind them. The new CD-ROM games like Myst with all the art and assets were raising the bar as to what players expected from a modern computer game.

In one way, **Glider PRO** was a reaction to the **Glider** games up to that point. I started to feel a creeping kind of claustrophobia in the game — being holed up in a house as it were, looking for an open window. So **GliderPRO** would introduce (in addition to other things) the outdoors as a place to explore with your paper airplane.

> The name, **Glider PRO**, was conceived as a kind of joke at the time — a kind of jab at the word "pro" being tacked on to a number of productivity applications in the 90's.

The rooms remained 512 x 342 pixels in size but with larger, color displays having become the norm I decided to render as many as 9 rooms — "Hollywood Squares" style. I would also support 256 colors and not force users to play in 16-color mode.

With no "escape room" in **Glider PRO** (escaping the house being the goal in the original **Glider 4.0**) I had to have a new goal. That became collecting all the stars in the "house". So stars became a new game object — joined by a number of other new objects. Switches in one room could toggle the state of objects in another room allowing for puzzle-like levels where a number of switches needed to be found and toggled in order to progress ot the next star.

This time too, rather than a separate level-editor application, I integrated editing directly into **Glider PRO**.

As I mentioned earlier, in order to justify **Glider PRO** I asked a few "house authors" that had done really stellar work creating houses with **Glider 4.0** to help me on the house that ultimately shipped with **Glider PRO** (cllaed *Slumberland*). I blocked out a large amount of "level real estate" and Sean, Steve and Ward each took their slice and got busy creating rooms, puzzles, etc. I would periodically update them with a new beta of **Glider PRO**, periodically integrate their house edits into the combined "master".

When it finally started to come together, the kind folks at Casady & Greene began to also beta-test and try to navigate through "Slumberland". And true to the original concept, players would fly out of the first house, fly into a second, travel for a good deal through the sewers beneath the ground, travel across fields ...

### Changing Times

Eventually an engineer working on the graphics team at Apple Computer Inc. reached out to me and I was flown out to California for a job interview. In 1995 I began as a programmer at Apple just as the company was sliding into the darkest period of its existence. Nonetheless, there was no doubt in my mind that my stint as a solo game developer had run its course. My girlfriend would follow me to California for our next adventure. Writing games was questionable in any event since Apple stipulated that any programming that its engineers did belonged to Apple — on or off the clock.

In fact I somehow survived the layoffs — made my career at Apple. I married my girlfriend and we raised three California girls in the Bay Area.

Casady & Greene suffered the fate that I think the majority of the "mom and pop" software houses were succumbing to. Game sales were in fact going increasingly to the bigger players that had broader reach. Productivity apps were concentrated to a handful of the big players — utility software was being bundled in the OS itself. As a company C&G's last "hurrah" was their sale of Jeff Robbins' popular "SoundJam" application to Apple where it was rebranded "iTunes". I suppose it was not enough to sustain them though.

In my mind though, like some kind of postcard, Casady & Greene will still always be this image of straw-colored hills dotted with Live Oak trees and the friendly people I met that were so warm and welcoming to this complete stranger: this bewildered Kansas so out of my element.

<p align="center">
<img src="https://github.com/EngineersNeedArt/SoftDorothy-CasadyGreeneProjects/blob/9899fe07e681a52fdf591c80747f82b8ed17ed67/Images/JudyDonPiano1.jpeg">
  <br>
<em>Judy and Don of Casady & Greene seated at a hotel piano.</em>
</p>
