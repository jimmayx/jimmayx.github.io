---
layout: post
title: My Homelab
date: '2022-09-13 11:55:59 +1300'
categories: [Technology]
tags: [tech, technology, homelab, servers, selfhost, docker, opnsense]
toc: true
---

In this post I am going to outline what my homelab is comprised of, all the different services I am running and some challenges I faced along the way. Resources I used to grow the homelab and learn how it all worked will be included at the bottom for those wanting to have a go themselves.

Here is a quick overview of my network devices and my ever-evolving homelab:

![My homelab diagram](..\assets\img\homelabNetworkDiagram.png "Network Diagram")

The first thing I want to go over is my router. It is made from a mini-itx PC that I was given from work. I gave it a little bit of extra RAM and installed OPNSense on it. Other than a few times I have been messing around in the config, it has stayed rock solid. The big reason I went for a custom router was the price of an off the shelf solutions are expensive and don't give the level of customisation and feature support I want. I also wanted to start breaking up the roles of certain devices on my network. Having an access point that can just focus on the job of an access point can be very beneficial to overall performance, especially when I am using relatively low-end hardware. 

The next thing I want to look at is my application server. It is running on an old thin client that I got from work (it is a bit of a joke at this point with how much "E-Waste" I come home with). First thing I did was research what is the best Linux distro for stability and a main homelab server. I had used Ubuntu server in past when playing around so I decided to go with a different distro in Debian 12. With that choice out of the way, some server hardening completed and a little bit of inspiration gathering, I started adding applications. Traefik took me a few goes but I finally managed to get it sorted. Initially what had caused me issues was just figuring out how it worked and understanding the configuration. Pihole was a source of issue as I used Piholes DNS to allow local DNS lookups but was struggling to figure out how to resolve pihole.<\mydomain>. I eventually sorted that out after I moved pihole to the app server off of a tired raspberry pi 3. 
The rest of the apps get added as I watch showcase videos or see social media posts about certain homelab apps that look cool. I have a shortlist of apps I am interested in setting up but as most homelabbers can relate to, I have too many ideas and not enough time currently. 

My most tempramental server is my media server. This server has seen too many revisions and upgrades to count. It started life as an old University cast-off PC I got from Facebook Marketplace for $50. It has grown, evolved, burnt to the ground, been fixed, faulted again multiple times. Currently it is in a "working for now" state. I have some plans to upgrade it with some aquired hardware (have a guess where I got that from). This started as a server I made when living with parents to encourage them to cord-cut. Eventually I got a girlfriend who loves movies and tv dramas and that set me down this path. I now have all the *arr apps to help download all the relevant tv shows and movies I have monitored in my library. This saves me with the admin work that became a job away from work. My biggest concern is that all my hard drives are second hand. In the beginning I would go to second hand shops and buy old DVR recorders that had 1TB 5400RPM drives. I got some cast-aways from work which have allowed me to increase the capacity slowly but I have already suffered two full data losses. I will need to fork out for new drives at some point but I can't make myself do it. At least I have managed to aqcuire 4 x 6TB WD Reds from an old mass storage PC (I'll give you 1 guess where it came from). 

The last and least complex server I want to highlight is my game server. I say game server but it just runs two minecraft server docker containers. Both of them use the itzg/minecraft image except for the modded one uses the ftba variant. This server is an office PC that I gave some extra RAM and installed Debian on. I run the servers on non-standard ports to allow for both to be mapped to an external DNS entry. I mapped them to modded.<\mydomain2> and vanilla.<\mydomain2>. There was a bit of movie magic to get this to work that required several forum site visits as this a rather unique deployment, apparently. 

My homelab is an outlet to learn and work out concepts to advance my knowledge. It brings my a lot of joy to tinker with it all and there is no better feeling than getting it working and having someone else appreciate it to like my girlfriend who has to live with it in our apartment. I have a large amount of ideas and plans for what I want to do and explore with the homelab. Me end goal is to own a house that has smart-home features built in to everything to assist in day-to-day tasks, all controlled by my homelab. That day is still a wee way away yet.

\- JS