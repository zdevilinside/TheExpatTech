---
title: "What is a Digital Nomad VPN?"
date: 2025-11-23T19:35:49-06:00
authors: ["ZDevilInside"]
draft: false
image: "VPN.png"
categories: ["digital-nomading"]
description: "VPNs types for the Digital Nomad"
---
**Let's start this off with a few explanations of things so you can better understand some basic concepts.**

First off, think of the Internet as a giant map.  There are addresses on there that you can get certain things from and only those addresses.  To reach them, you type in something like www.IDontWantToBeHere.com (I don't think that site actually exists though) and hit enter on your web browser.  Most people don't know how that actually works though.  Your Internet provider takes that website's URL and looks it up in a phone book until it gets a "phone number" that is used to dial that location.  When you enter that address, the phonebook shows the address 127.0.0.1 and dials that #.  It is that simple.

**Now, let's talk about a Digital Nomad VPN and how to set it up.**

First off, I want you to understand I am not telling you to do this.  I am just telling you **HOW** to do this thing called a private VPN server.  

Secondly, using a private VPN server to hide location from work can be done but there are some important things to know.  First, many places will fire you if they catch you working from somewhere that you are not allowed to work from.  I cannot be held responsible if you use the knowledge I pass on to work from somewhere you are not supposed to be and end up losing your job because it.  

Third, traveling the world while working from honme is a get feeling to have if you are willing to take the risks.


**What is it?**

Okay, the technical definition of a VPN server is a remote server that acts as an intermediary between your device and the internet, routing your traffic through an encrypted tunnel.  It masks your IP address and makes it look like your traffic is originating from the server's location and protects the data from prying eyes.  

Well, let's make it easy for you to understand.  A private VPN server allows someone to hide the location they are working from.  This setup, when done correctly, will allow you to work from a beach in Tahiti while making it look like you are in your mother's basement in whatever city you are from.  It is also good to make it look like you are in the US when you are in someplace like Mexico and are able to use it to watch US Netflix, Amazon Prime, etc.  

Yes, there are public VPN services out there that can do this but it is a "wack-a-mole" type thing.  When a service recognizes an server as an VPN provider, that service will block that server from being able to be used.  You will then have to try another server until that one gets caught, and you start all over again.  

**What does this mean to a Digital Nomad?**

Well, there are 3 ways you can have a VPN service.  Here, I will chart them for you.

# Types of VPN

## A breakdown on the VPN types and what it means

| | |
|---|---|
|**Public VPN** - a commercial VPN provider such as Nord, Proton or PIA|  This is a service were you run an application provided by the VPN provider and they have you connect to a litinany of providers all around the world.  Why is it a bad solution for a Digital Nomad?  It is because it is the least secure method.  It won't necessarily be able to hide all traffic on your system.  Further, you may not be able to install an application on your computer.  That isn't always teh case.|
|**Hybrid VPN**  - this is where you use a VPN router as your client and it connects to a commericial VPN service that provides you access to their servers.|  This is a better option the a pure public VPN and all data goes through the VPN router.  This isn't as simple to setup as the Public VPN and it relies on hardware that can fail.  Further, it uses commercial VPN service that show up as public VPN servers and your IT department is on the lookout for these.|
|**Private VPN** - this is the way to go if you can do it. | With this try of VPN, it is a privately hosted service where you have a VPN server at your home, friend's house, or a relative's house.  It uses their Internet connection and makes it so it appears you are at that location.  This is the best option to not make it immediately apparent that you are using a VPN.|

If your employer looks at your connection carefully,they can detect your usage from many different things so let's minimize that from happening.  This means you have to take precautions and set up some things first.

1.  Setup a kill switch.  This will make it so that if your VPN goes down, your system will block all non-VPN traffic.
2.  Separate devices for work and home.  Do not use the phone you use for your private life for your work - have separate devices instead.  Having this strict wall between devices is paramount to not being caught.  If your phone is roaming, it can give away your location even if it is connected to the VPN router.  It is called "leaking" and has led to people getting caught.
3.  On work devices, use ONLY Ethernet and USB.  Disable **ALL** radios on the work system.  No bluetooth, no Wifi, no nothing.  Nearby devices can show an estimated location.    
4.  Manually set the time zone on all your devices to match the time zone you are supposed to be working from.  Keep it consistent and have it set the same through all your devices and not just your work equipment.
5.  If they have your mobile phone # and call you, it can give you a different rings depending upon what region you are in.  Further, cell phone service providers often sell their geolocation databases of customers to outside parties.

The list can go on and on but it comes down to keeping things separate, don't post on social media where you are nor share your photos that might have something identifiable as a different place than where you say you are.  Minimize the amount of information available about you and you should be able to fly under the radar.

My next post will be about HOW to setup a Digital Nomad VPN server and client using GL.Inet equipment.
