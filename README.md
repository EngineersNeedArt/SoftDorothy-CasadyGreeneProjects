# Soft Dorothy Software — Early Published Projects
Disk images (intended for emulators) containing code and tools for building the commercial games John Calhoun wrote for Casady & Greene, Inc.

I wanted to capture in one place the sources to the early Macintosh games I published with Casady & Greene Inc. as well as the old build environment (THINK C, THINK Pascal, ResEdit) and create disk images suitable for the current early Macintosh emulators. The disk images here (zipped to save space) can be downloaded and you should be able to mount them in <a href="https://basilisk.cebix.net">Basilisk II</a>, <a href="https://sheepshaver.cebix.net">Sheepshaver</a> or <a href="https://www.gryphel.com/c/minivmac/">MiniVMac</a>. 

Below, in order of release, are the disk images included in this repository.

### Glider4Dev.dsk (First commercial version of Glider)

**Glider 4.0** (BNDL identifier `GLID`) was the first game I had published commercially. I had seen a few games published by Casady & Greene, Inc. (C&G) and reached out to them to see if they were interested in **Glider**. I suggested I could write a commercial **Glider** to support color and that the game would have a "house" (the game levels) with some forty or so rooms (the shareware game had only ten or fifteen rooms as I recall). They agreed and so advanced me enough cash to buy a color Macintosh and a color display.

<p align="center">
<img width="752" src="https://github.com/EngineersNeedArt/SoftDorothy-PublishedProjects/blob/b365778f5129970dbb572805d3c252235d49d766/Images/BasiliskIIScreenshot.jpg">
</p>

I believe I more or less finished **Glider 4.0** around the beginning of the fall of 1991. That fall I was in my last year of an Education degree at the University of Kansas. I student taught that last year and I recall telling my high school students that I had a game coming out, ha ha.

The "houses" for **Glider** are like a collection of *levels*. I determined pretty quickly that creating a "level editor" for **Glider** would make it much easier for me to create the promised house of forty or more rooms. And so the creation of both **Glider 4.0** and a **House Editor** began more or less at the same time.

I could have kept the **House Editor** (BNDL identifier `GLed`) as an internal tool but I realized that if users could create and share their own house creations, it would add to the appeal to **Glider**. I think i was thinking about something similar to the Pinball Construction Set game.

I found out very quickly though that work on the House Editor in fact involved more work than **Glider** itself. It turned out that "idiot proofing" the editor required a lot of sanity checking and busy work. As an example, when a user adds a bouncing ball to a room, there is a Get Info dialog that allows you to edit various parameters of the ball such as the **Length of travel**. When a user entered a value I had to make sure it was not negative, not too large for the room. These kinds of sanity checks are all over in the code and required a lot of busy effort.

<p align="center">
<img width="752" src="https://github.com/EngineersNeedArt/SoftDorothy-PublishedProjects/blob/265b7f87d170fb85c75443b5152532326113aea5/Images/GliderEditorScreenshot.jpg">
</p>

**Glider 4.0** 4.0 went on to win a MacWorld Game Hall of Fame award. I graduated with my Education degree but as a result of **Glider's** success I decided to put off teaching at least for the time being. The game programming gig would likely be brief and teaching would still be there in any event.

Additionally, AOL (America On-Line) had become a thing about that time and **Glider 4.0** houses that people had created with the house editor started being uploaded and downloaded. I was surprised to see the small community that built up. Even a fan newsletter for a time. If creating houses was not your thing, **Glider** could still get a longer shelf-life by downloading and playing houses that others had created.

### Pararena2Dev.dsk (Commercial version of Pararena)

As with the other disk images, unzip `Pararena2Dev.dsk` and mount with one of the early Macintosh emulators listed above. THINK C, and  ResEdit are included on the disk so that you have everything needed to build and run **Pararena 2.0**

**Pararena 2.0** (BNDL identifier `RenA`) was the second game I wrote that was published by Casady & Greene Inc. (C&G). It came about after the success of **Glider** when C&G asked, "What else you got?" I had my doubts about **Pararena** but the shareware version had something of a small but dedicated fanbase. I imagined that in addition to color, perhaps I could add enough additional features to make it more commercially viable. The dates on the original files suggest the game was written in July of 1992, roughly a year after **Glider 4.0** was written. 

<p align="center">
<img src="https://github.com/EngineersNeedArt/SoftDorothy-PublishedProjects/blob/fff10d77b13afe2aff30a19739a52d47cb835fb4/Images/PararenaRejectedSplashScreen.png">
  <br>
<em>Casady & Greene rejected this splash screen.</em>
</p>

**Pararena 2.0** was to be another first for me — I was intending to write it in the C language rather than in Pascal (which all my other games had been written in). Once again my shareware game, **Glypha**, became my testing ground. I rewrote **Glypha** in C and "shipped" it before beginning my first commercial C application. And again, **Glypha** written in C was well received and **Pararena 2.0** shipped with no problems due to my having learned a new programming language.

Some thing I added to hopefully give it more commercial-game gravitas was an "instant replay" that showed, TV-style, the seconds leading up to a scored goal. I also added several computer opponents that varied from novice to expert-level players. There were tournaments and awards you could try to attain within the game. And finally there was a rudimentary network option where two Macintoshes, connected by a null-modem cable (and if they were lucky) could play a game head-to-head, human vs. human.

Despite all of the above though, **Pararena 2.0** never made even 10% of what **Glider 4.0** had made. It was not going to be possible to live on the royalties if game sales followed in **Pararena's** footsteps. I reminded myself though that I still had the Education degree and could always begin my teaching career.
