---
layout: post
title:  "TGDL : Perspective"
date:   2019-11-26 00:14:35 -0700
categories: 
  - tgdl
tags:
  - concept
  - graphics
published: true
---

### Introduction

This is The Game Design Lexicon and welcome to our first glossary entry! Today we'll be looking at an aspect of our visual interaction with video games; Perspective. Kinda lame to start off with a straight definition, but it's where I started my research and it really fit. According to Merriam-Webster: 

* perspective: noun : 1b : a visible scene

I'm not sure I can do much better. How do you visually convey what your player needs to gather the information to play the game? A visible scene is usually the first choice.

### How it looks to you. A Flat Perspective.

In traditional card and board games this is all you have. No sound. Just visuals you can move around and arrange and use as per the rules given. It is no coincidence that early computer games mimicked board games in the perspective in which they displayed information for the player.

Graphics on your monitor are presented as a two dimensional image. They are a grid of dots or "pixels", hundreds of pixels tall and sometimes thousands wide. With the wide and varying needs we have today for displays, it's not unusual to see them of all shapes and sizes.

When I was a boy it was a staggering 176 by 184 pixels, sometimes less. Sure it wasn't the great depression, but try contemplating *any* first person shooter on that postage stamp... Except when I was experiencing it, it wasn't a postage stamp. You were looking at that on a 15 to 17 inch screen.

Today's screen runs from 1K to 2k to 4K. Numbers that represent the approximate pixel width of the screen.

Not to have a 'get off my lawn' moment, but I'm not fan of the the new resolution terminology. Before you gave the resolution. Saying 1024 by 768 was explicit while 1k, 2k, 4k only really give horizontal resolution, approximately. With no vertical resolution, you would need to know the display ratio to determine the full size. GET OFF MY LAWN!

Each pixel represents a color. The way your computer knows which colors to display in each pixel is stored in four number values. The first three numbers in order represent colors red, blue, and green, ranged from fully off, to fully on. The fourth value is an "alpha" value that represents how opaque the color is so it can be blended with colors that visually lie behind it. I mean, lie behind it virtually because it is a flat surface in reality.

* Ranges from 0 to 1, or 0 to 255

* [Additive Color](https://en.wikipedia.org/wiki/Additive_color)

I'm trying not to get too technical, so don't whip me for leaving out details, please. No matter how complex the scene you are viewing on your display, like any animation, it is displayed as a projector displays an image on a movie screen. Milliseconds after placing the last 2D image on your screen, it is switched out with a new image to reflect the changes that have been made in that time. This is true whether you're playing the Doom 3 or Flappy Bird, or editing your next presentation, or clicking play on Spotify. 

### Different Perspectives.

I'm not sure I need to dwell too long in a history lesson. There are others who have already done it much better than I could. I'm going to give out what you need to know, but remember to seek out as much as you can. The more you know, the more point of references you have to draw from.

#### Flat 2D: One of the first.

The earliest video games were visual representations of traditional board games. Tic-Tac-Toe, Checkers, and Chess. These only fit the definition of a Video Game if you define it as "a game run on a computer", as the 'video' portion was often constructed solely for displaying that particular game.

Though if I can make a quick recommendation; James Burke a BBC presenter and technology historian has a series called "The Day The World Changed." Episode 3 to be specific... "Point of View: Scientific Imagination in the Renaissance" ... If you want a good idea of the history of our awareness of perspective, this show is a wealth of easily digestible knowledge on it.

Needless to say as computers became more powerful and cheaper to make our ability to visualize things with them also grew. Eventually we had dynamic displays that people could more easily afford in cathode-ray tube televisions, which enabled us to make games that you could visit an arcade and play, and almost as quickly in the comfort of your own home. We still use a similar technology today. What displays the dots has changed and improved. But they are still rows of dots that fool your mind into thinking it has more depth than a painting on a wall.

Virtual Reality hardware has also recently come of age. We will touch on this a bit more when we discuss how 3D is displayed. We're at about the half-way mark. The rest of our episode will be about types of perspectives traditionally represented in video games.

#### Text: Read any good books lately?

Since the first 'computers' we had were glorified morris code machines, it isn't a far stretch to think that some of the first games for computers were nothing more than text describing a scene like you were reading a book. Games like Richard Garriot's 'dnd' were made to be played on the teletype. In case you're not up on the technology, it was a way to send text data over a phone line. The data would be translated by a 'smart typewriter' and transcribed to paper. It was the predecessor to the fax machine.

* [dnd](https://www.apl2bits.net/2014/06/30/garriott-basic-dnd-port/)

These types of games reached a crescendo during the 1980s with games like the Infocom library. The DNA from these games are in every game you play that values environment over game-play... and even some of those that don't.

#### 2D meets depth perception.

At about the same time, we had the basics for most types of 2D games. Again, people loved Chess, Checkers and Card and Casino games before they could play them on a computer, and all you needed was a 2D display. But even games like Electronic Art's Battle Chess pushed this to the limit by having the board displayed in a pseudo-3D view, with animated pieces that would beat the tar out of each other.

* [Battle Chess](https://abandonwaregames.net/game/battle-chess)

And by that time, it was happening more and more. Flat games were no longer acceptable. Even strategy games were starting to take on a more nuanced perspective. And they were the ones most comfortable in 2D! Techniques like 2.5D, displayed in tons of 1980's brawler games, still displayed everything as a 2D image, but added the illusion of depth by taking one of the axis of movement, the y axis typically, and turned it into a measurement of depth.

How 'high' your character was on the screen symbolized how far 'away' from you they were. Some even added the illusion of depth by making the image smaller the higher it was. I might as well admit it right now. Once they stopped putting just text on the screen it's all been smoke and mirrors. Over the years the push in technology has allowed game developers to make a more elaborate visual hoax.

#### Isometric: An aside.

Engineers that were using computers to make technical drawings came up with a popular perspective that allowed them to see drawings of their technical ideas with depth and the ability to move the items up and down and have the same illusion the brawler games had. Except this had the maths behind it. You would take the image as if you were looking at it from one of the six sides of it directly. Then you'd rotate it on its y about 45 degrees, and then rotate on its x axis about 35 degrees. We call this an Isometric Projection.

It allows us the illusion of 3D by having the ability to easily stack 'tiles' in a staggered fashion. Of course this is all done virtually. You still see it as a flat image. 

#### 3D: More than just red and blue goggles.

The idea of having a first person perspective in a computer game probably happened earlier than you'd imagine. Richard Garriot of Ultima fame was experimenting with it in his games back when most computer games looked like chess or pong. There were even arcade games that used a new technology that allowed you to quickly render a line between two points in 3D space at any angle you wanted it.

The first computational examples of this happened well before we saw them in video games. Lots of scientific and military applications. But by the 1970s, we were ready to make games that had dynamic vectors in them. At first they were just used to display flat games though. Space War, Star Castle, and Asteroids are good examples of vector graphics being used to display a game that you'd normally imagine being made of pixels.

* [Star Castle](https://en.wikipedia.org/wiki/Star_Castle)

Once our processing power caught up we started using them to make the quick calculations needed to reposition something in virtual 3D space, and figure out what needs to be drawn on the screen to be visible to the designated camera area.

What helped this along was the sudden availability of commercially affordable math co-processors. The main purpose in which was to do one thing: make calculations of decimal represented numbers. Like 3.14159 x 2.71828. It enabled us to do the trigonometry, linear algebra, and even calculus quick enough to meet the minimum animation rate to display it to our eyes.

Today, your video card is made of thousands of them. Each one doing multiple calculations every 16.66667 milliseconds to make that 60 frame per second game happen. All to keep up the illusion of making you think you're seeing a 3D scene, when it's just a chain of 2D images like any movie. The difference is when you react to this movie, it reacts to you!

To do this, the idea of the Vector had to come a long way. You went from just enough to display crawling through a dungeon as in Ultima I, to being able to render scenes in real-time that can fool you into thinking you are looking at a real place. The amount of Vectors this takes is ... well a lot. The more detailed a 3D image, the more vectors. A box with no detail takes eight points with vectors in-between each edge point. When was the last time you saw a 3D graphic as plain as a box?

Shhh Minecraft players, I know. It's a neat game but the graphics were intentionally lazy. But don't get me wrong, I love low poly. It's kinda the post-modernist, deconstructive movement in the visual medium of video games. So now we can build up these wonderful 3D dioramas on our 2D projected screen and view them. To complete the interactivity, you are given two choices of perspective.

#### 3rd Person: Walkin' after you...

Third-Person perspective is looking at the diorama via the agent of some dis-embodied camera. This is what our 2D perspective game we've talked about has evolved into. No longer is the illusion of 3D achieved by cleverly drawn pixel art. 

The computer is now given the model, the location of the model in the scene and how it's positioned, and then calculates what it would look like as a 2D image if viewed from a particular point in space. And figures out what pixels need to be drawn and at what shading to reflect that.

For often hundreds of items, all in 1/60th of a second.

If your viewing point isn't attached to an entity in the game, we call this Third-Person.

#### 1st Person: Me, me, me...

If it is, such as, if your view point is attached to the eyes of a person, then you are given what is called First-Person perspective. There really isn't a 2nd person perspective, though I'll place a link to an interesting video about that in the subtext.

* [Nick Robinson - This Is What a "Second-Person" Video Game Would Look Like](https://www.youtube.com/watch?v=mC8QoRa8y_Q)

And that brings us up to date. Sort of.

#### Virtual Reality: Wait, again?

One other visual 'perspective' worth mentioning is Virtual Reality. The term itself is a bit of a misnomer. You see, everything we've talked about up until now has been a form of virtual reality. Nearly every video game has been an attempt to simulate some scope of reality. Whether it's true reality or fantasy-based reality.

Virtual Reality in the late 2010's is what I would call the next iteration of stereoscopic perspective display. The technology is fairly old. Stereoscopic viewers were all the rage in the late 1800s. The 1960s saw it added to cinema with the advent of those goofy red and blue glasses. Stereoscopic perspective not only creates the illusion of depth through basic perspective, but in addition fools your brain into sensing the depth by providing different information to each eye that perceives it.

It's a subtle effect. But each eye on your head sees two different pictures despite staring at the same thing. Each picture is from a very slightly different location. This difference in location your brain can detect and use to sense the depth of an object.

In our first person example above, to change this into a stereoscopic scene, you'd need to add another camera about the same distance apart as someone's pupils, and make sure the viewer's eyes were isolated to the proper respective image. Tada! You've just used two flat images to simulate a 3D scene. And now unlike the 1800s, you can interact with it. Just try not to puke.

I'm going to leave Augmented Reality alone, as I feel it falls into similar categories already discussed.

And that's it. The basics and basic terminology of how your computer displays images, and the despoliation of some of computer science's magic tricks. 

### Summary

Look forward to future entries where we discuss some more of the concepts we barely breezed by in better detail like how an interactive game loop works and the pipeline involved from the simulation you run that you need to draw, to how you determine how to draw it, all the way to the image it needs to display.
