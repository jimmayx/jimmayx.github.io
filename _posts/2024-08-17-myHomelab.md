---
layout: post
title: My Homelab
date: '2022-11-23 11:55:59 +1300'
categories: [Technology]
tags: [tech, technology, homelab, servers, selfhost, docker, opnsense]
toc: true
---

In this post I am going to outline what my homelab is comprised of, all the different services I am running and some challenges I faced along the way. Resources I used to grow the homelab and learn how it all worked will be included at the bottom for those wanting to have a go themselves.

Here is a quick overview of my network devices and my ever-evolving homelab:



The first thing I want to go over is my router. It is made from a mini-itx PC that I was given from work. I gave it a little bit of extra RAM and installed OPNSense on it. Other than a few times I have been messing around in the config, it has stayed rock solid. The big reason I went for a custom router was the price of an off the shelf solutions are expensive and don't give the level of customisation and feature support I want. I also wanted to start breaking up the roles of certain devices on my network. Having an access point that can just focus on the job of an access point can be very beneficial to overall performance, especially when I am using relatively low-end hardware. 

The next thing I want to look at is my application server. It is running on an old thin client that I got from work (It is a bit of a joke at this point with how much "E-Waste" I come home with). First thing I did was research what is the best Linux distro for stability and a main homelab server. I had used Ubuntu server in past when playing around so I decided to 

\- JS