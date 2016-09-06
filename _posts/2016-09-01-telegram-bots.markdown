---
layout: post
title: "Telegram Bots"
date: September 2016
categories: post intro 
layout: default
modal-id: 1
img: telegram.png
alt: image-alt
project-date: September 2016
description: What I do in my free time.

---

I made some bots!

So first: what is Telegram, and what are bots? Telegram is a messaging service (think Facebook's Messenger/WhatsApp, Google's Allo, etc.) It has some features that I really enjoy using, like how it handles images and files. What most attracted me to Telegram was its APIs for bots.

Bots are Telegram users that are controlled by computers rather than humans. When I message a person on Telegram, they chat back with me. When I message a bot, a computer program responds. I have written two bots so far!

The first bot, DurdenBot, is a simple bot. Starting out, I wanted to try using 2+ APIs and write a backend in node.js. However, I didn't know what I wanted the bot to do. So I asked around and got a very powerful suggestion: "Have it send me pictures of kittens."

I used Imgur's API and the Telegram Bot 2.0 API to create the bot such that on receiving the command `/kitten`, the bot pulls a pseudorandom picture of a kitten from Imgur that has the "kitten" tag. Later, I generalized the bot that given any one-word tag, it would pull an image. 

The bot was a ton of fun to make, but I wanted to make something more useful. I had been using the audio player Mopidy on my computer, which is a music playing program (think iTunes, Foobar, etc.) with a client-server architecture. Many different Mopidy clients have been written for all manners of platforms. I was inspired to make a bot for Mopidy (and it didn't hurt that Mopidy had APIs as well). 

I wrote a second bot, MopidyBot, to control an instance of Mopidy. It has simple features like play-pause, next song, and so on. But it also links with Spotify for an advanced search feature accomplished by having a simple conversation with the bot. It's great for entertaining guests as well, as the guests can tell the bot what they want to hear and queue up the songs!

I learned a lot from making these bots, mostly about my own programming skills and likes. I love using APIs and automating my life by programming. I learned so much about Javascript as a backend language and leveraging node.js to do that. I learned a lot about asynchronicity, callbacks, and what to do when you realize your old code is really bad. I've released both bots for free on [my Github](https://github.com/tylerjdurden), and I now plan to rewrite them in Python using Flask as a RESTful API.

Thanks for reading!
