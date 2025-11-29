---
title: "How to fix an IPv6 speed issue"
date: 2025-11-11
authors: ["ZDevilInside"]
categories: ["Tech Tips"]
tags: ["Tech Tips"]
description: "The steps I had to take to fix this issue"
draft: false
image: "image1.jpg"
---

I recently had a big problem develop with my Digital Nomad VPN Internet Service at my home in Cuernavaca, Mexico. My ISP implemented their IPv6 migration and all sorts of problems developed. My SpeedTest.net and other links were all out of whack. I ran SpeedTest.net checks against their servers and with other servers in the Mexico City area. The results were quite surprising.

There is NOTHING wrong with the upload speed here! (sarcasm)  
![speedtest #1](test1.png)  

![speedtest #2](test2.png)  

I started to get suspicious it was something wrong with their server, so I tried one outside of their domain.  
![speedtest #3](test3.png)  

Hmm, speed is normal there.

I went back to Totalplay's Speedtest server and got this:  

![speedtest #4](test4.png)  

![speedtest #5](test5.png)  

I contacted Totalplay about this issue and they basically blew me off; it felt like they couldn’t care less about my issues and that as long as my upload speed was okay, they didn’t consider it a problem. I didn’t like this one bit, so I decided to take matters into my own hands. I ran another speedtest to check if my brain wasn’t working right. Nope, I was correct.  

![speedtest #6](test6.png)

There was definitely something wrong with their service, and I knew it was with their IPv6 implementation. What could I do? As I surfed the web, I found a test that allowed me to do speedtests against the same server using IPv4 and IPv6 separately but at the same time. Here were my results:  

![IPv6 test](image1.jpg)  
![IPv4 test](image2.jpg)  

Totalplay’s techs wouldn’t help me and basically said, “We are going to have someone call you back and fix this issue...” but I never received a call back. I kept doing some research and came across a Microsoft article titled *Guidance for configuring IPv6 in Windows for advanced users*. I read the article and found that you could use a registry key to configure IPv6, but more importantly, force your system to prefer IPv4 over IPv6.  

> Location: HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\Tcpip6\Parameters\  
> Name: DisabledComponents  
> Type: REG_DWORD  
> Min Value: 0x00 (default value)  
> Max Value: 0xFF (IPv6 disabled)

And it had the following about preferring IPv4 over IPv6:  
> Decimal 32  
> Hexadecimal 0x20  
> Binary xx1x xxxx  
>  
> Recommended instead of disabling IPv6.  
>  
> To confirm preference of IPv4 over IPv6, perform the following commands:  
>  
> - Open the command prompt or PowerShell.  
> - Use the `ping` command to check the preferred IP version. For example, `ping bing.com`.  
> - If IPv4 is preferred, you should see an IPv4 address being returned in the response.  
>  
> Network Connections:  
>  
> - Open the command prompt or PowerShell.  
> - Use `netsh interface ipv6 show prefixpolicies`  
> - Check if the prefix policies have been modified to prioritize IPv4.  
> - The `::ffff:0:0/96` prefix should have a higher precedence than the `::/0` prefix.  
>  
> For example, if you have two entries, one with precedence 35 and another with precedence 40, the one with precedence 40 will be preferred.  
> ![Netsh results](image3.jpg)  

**Now we are getting somewhere!**  

I went ahead and tried it, and my Speedtest results immediately improved. However, I wasn’t too happy with Totalplay and decided to switch over to Telmex because my IPTV boxes STILL had problems with the IPv6 implementation, where they were constantly disconnecting and reconnecting. Since I switched services, I haven’t had any problems. Totalplay needs to get their act together.

So, what kind of Speedtest results am I getting today?

![Telmex speed results](image4.jpg)  
I can live with that!
