---
layout: post
title: RE:vision Of My Homelab
date: '2026-10-2 11:55:59 +1300'
categories: [Technology]
tags: [tech, technology, homelab, servers, selfhost, docker, opnsense, debian, linux]
toc: true
---

Hello readers,

After two years I think it is time to update my setup overview and run through how it works at a high level.

At the time of writing this post I have recently moved to a new job to help advance my IT career with more to learn and understand. This will help shape my homelab and with any luck take it to new heights though I also anticipate I may now have less time than I did previously to work on it.

Firstly, gone is the multiple servers. I consolidated most of my tech stack to one server to save on space which is quite limited in my flat. This change also led me to ditch Windows Server which had been having instability issues and was slowing down some of my progress.

I took a swing at Linux which I was comfortable with but by no means an expert. A multitude of hours was spent pouring over the very best literature and video commentary the internet could offer up, I made my choice with Debian. The reasons I had found Debian the suitable successor was it's rock solid stability even with continuous updates as well as the fact it makes up the building blocks for many other distros.

I had originally added a RAID card and had an assortment of used drives in the chassis but after wanting to switch cases to a rack mounted case that did not have a drive bay and receiving a cast off Synology NAS with accompanying new(ish) drives, I decided to break the storage out into it's own unit. There are plans to add the RAID card back and 3D print a drive cage for more storage that can be used for more general file and photo storage. 

I retained my OpnSense firewall which has stayed rock solid for me. I have enabled github backups so the configuration file gets automatically backed up to a private repo so I can import that if there was a failure or rollback using a known good file at anytime. I will upgrade the network card for it to support 10G speeds but for now I only have a 1G fibre connection so I will leave this be. I also picked up an old 16 port Ubiquiti POE switch and a U6 Pro which is helping upgrade the backbone of my network infrastructure. 

I also thought it would be a good idea to show you all the applications I currently have. I am always adding more as I find a need or problem I can solve or even sometimes because it sounds cool.

I have a lot of supporting applications for my media stack which is the primary function of my server. 

\- JS
