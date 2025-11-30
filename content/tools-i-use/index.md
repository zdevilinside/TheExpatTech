---
title: "Tech Tools I Use"
description: "My go-to hardware, software, and services"
layout: "single"
---

Here’s a running list of the tools I rely on for aviation, nomading, and tech work.  
I’ll keep adding to this page as I discover new gear and services and work through my bookmarks finding tools I have used in the past that I found amazing or useful in the past.  

<!-- Example parked link syntax for reference:
[Dell laptops](https://www.dell.com)
-->

## Software used to fix Windows-based computers listed in no particular order:  

- [Medicat](https://medicatusb.com/) — the Swiss Army knife of Windows bootable USBs.  
  I’ve used Medicat countless times when a computer was too far gone to boot normally. 

- [Rufus](https://rufus.ie/en/) — creating bootable USB drives the easy way.  
  Rufus has saved me hours when creating new Windows install USBs.   

- [Norton Bootable Recovery Tool](https://support.norton.com/sp/static/external/tools/nbrt.html) — another bootable antivirus option.  
  I use multiple different scanner tools in this area because they often miss something the other gets.

- [Microsoft Defender Offline](https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-offline) — Microsoft’s built-in offline scanner.  
  Like Norton above, I use multiple different scanner tools in this area because they often miss something the other gets.

- [SuperAntispyware](https://www2.superantispyware.com/) — malware cleanup utility.  
  Do you have stubborn malware on your computer or think you do? This is a great tool in which to try to clear these #%!#$#@$% out! Like anti-virus bootable drives, I use multiple anti-malware programs because one doesn't always catch them all.

- [Malwarebytes Anti-malware](https://www.malwarebytes.com/) — trusted anti-malware scanner.  
  This is the software I run with SuperAntispyware. In my experience, it is always good to use a second anti-Malware scanning tool after the other is run.
  
- [Hiren's Boot CD](https://www.hirensbootcd.org/download/) — lightweight bootable toolkit.  
  Hiren’s has been my fallback when Medicat feels like it is too powerful of a tool to run. I used it when Medicat’s boot time takes too long — Hiren’s toolkit lets me reset passwords and run diagnostics quickly with an easy-to-use interface.  

- [Custom written network diagnostic scripts](https://github.com/zdevilinside/network_testing_scripts) — my own troubleshooting scripts.  
  These scripts are ones I created. I use them troubleshooting VPN issues — the logs created help technicians and others see exactly what is going on. This has since been ported by WickedYoda as part of his ongoing volunteer efforts to provide tech support on the GL.iNet Discord.

- Speed Test tools I use:
  - [Cloudflare Speed Test](https://speed.cloudflare.com/) — advanced connection testing.  
    An advanced tool for checking Internet connections. It gives you a running display of how your system is doing during the test.    
  - [OOKLA Speed Test](https://www.speedtest.net/) — baseline connectivity test.  
    This is my baseline test utility to check for connectivity and obvious speed issues.  
  - [CESNET Speedtest](https://www.speedtest.net/) — IPv4/IPv6 speed testing.  
    This testing utility provides advanced speed testing including individual IPv4 and IPv6 testing. I used this to find the problem with Totalplay's roll out of IPv6 documented in my "Tech Tips" section of the site.  

## Diagnostic Tools
- [CPU-Z](https://www.cpuid.com/softwares/cpu-z.html) — hardware spec checker.  
  I used CPU-Z to troubleshoot my wife's brand-new Alienware system that kept blue screening during games. When I checked the discrete video card with CPU-Z, it reported the RAM amount as *unknown*. That detail was enough for Dell to immediately replace her system when I gave them a screenshot of information.  

- [HWMonitor](https://www.cpuid.com/softwares/hwmonitor.html) — temperature and voltage monitor.  
  HWMonitor has helped me find where problems are occurring. Temperature spikes shown can explain random shutdowns, and other problematic hardware.  

- [CrystalDiskInfo](https://crystalmark.info/en/software/crystaldiskinfo/) — drive health checker.  
  I have used this on my own systems. I have been able to check hard drives I buy and to also troubleshoot their performance issues. SMART data can be used to determine if a drive is failing and can be swapped out before it does occur.   

- [MemTest86](https://www.memtest86.com/) — RAM testing utility.  
  MemTest86 reveals bad RAM in systems. I once had a system that crashed whenever you were running memory intensive applications. I ran this overnight and the test results showed thousands of errors. I swapped out the RAM and the problem went away. Mission completed.  
  
## Utilities
- [7-Zip](https://www.7-zip.org/) — file archiver.  
  I’ve used 7‑Zip for years to "zip" and "unzip" files. 

- [Notepad++](https://notepad-plus-plus.org/) — advanced text editor.  
  I have been using Notepad++ for over 20 years. I feel it is a great replacement for Windows' included utility Notepad. It allows you to visually see the construction of code, and doesn't "flush" your unsaved work if you close the program. In fact, I am using this right now as I create this post.  

- [Everything](https://www.voidtools.com/) — file search utility.  
  Everything helps you find misplaced files. I have used it to help people find files that they saved but couldn't find.  

## Hardware
- GL.iNet routers — [GL.iNet](https://www.gl-inet.com/) is my chosen solution for Digital Nomad VPNs.  
  I’ve used this company's products for years. I use them for VPN servers and clients. They are easy to set up, use, and are very reliable. They just work. 

- Mini PCs I recommend:
  - [Beelink mini PCs](https://www.bee-link.com/) — compact desktop systems.  
    I have a few customers that do not like having something large on their desk and these systems are easily mounted to the VESA mount that many of today's monitors have. 
  - [MINISFORUM mini PCs](https://www.minisforum.com/) — another mini-PC choice.  
    Another mini-PC company I have used for customers just like the Beelink products. I switch back and forth between Beelink and these depending upon price and area of use.

## Software for building my website
- [Hugo](https://gohugo.io/) — static site generator.  
  Hugo has been my publishing engine. I once rebuilt my site structure in a single evening — something that would have taken days with a traditional CMS.  

- [LoveIt Hugo Theme](https://github.com/dillonzq/LoveIt) — theme for Hugo.  
  LoveIt gave me a clean starting point. I remember tweaking its CSS late at night to match my brand colors — the flexibility made it easy to get the look I wanted.  

## Services
- [GitHub](https://github.com/) — hosting and version control.  
  GitHub is used to host this website. It makes version control and hosting simple. You can share other content too: my self-created networking tools are shared here.  

- [Cloudflare](https://www.cloudflare.com/) — DNS and site protection.  
  Cloudflare has saved me from DNS headaches. I didn't want to stay with my original website hosting and DNS providers and Cloudflare fixed that for me quickly and easily.  
