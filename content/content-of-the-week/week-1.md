---
title: "Bringing in the New Year — Week 1"
date: 2026-01-05
authors: ["ZDevilInside"]
description: "A new year is upon us."
draft: false
slug: "2026-week-1"
---

This week's news and other interesting content.

The New Year has arrived, and with it comes a fresh wave of tech chaos, security headaches, and a few bright spots worth celebrating.

## 🎤 CES 2026

CES 2026 is officially underway, and the theme this year is basically: *“If it exists, someone shoved AI into it.”*  
We’re seeing everything from AI‑powered home appliances to more ambitious projects like Gmail’s new inbox AI and OpenAI’s continued push into voice‑driven interfaces. It feels like the industry is finally shifting from “AI as a gimmick” to “AI as the default,” for better or worse.

If you want to dive deeper, here are a few solid rundowns:

- [Wired — What to Expect at CES 2026](https://www.wired.com/story/ces-2026-what-to-expect/)  
- [Engadget — CES 2026 Live Updates](https://www.engadget.com/ces-2026-live-updates-from-techs-biggest-conference-in-las-vegas-153146838.html)  
- [Tom’s Guide — CES 2026 Live Coverage](https://www.tomsguide.com/news/live/ces-2026-live-latest-news)

## 🔐 Computer Security News

A new Python‑based VVS stealer malware variant is circulating, targeting Discord users and attempting to steal credentials. Same old story: someone clicks something they shouldn’t, and suddenly their login info is on a server run by people who definitely aren’t using it for anything wholesome.

On the bigger‑impact side, the CLOP ransomware group is back in the headlines. They exploited Oracle EBS and managed to hit both Korean Air and the University of Phoenix. CLOP has been unusually quiet for a while, so this is a reminder that ransomware crews don’t retire — they just wait for the next unpatched system to wander into view.

## 🧰 Tech Stories of Interest

### **6 Free Tools Every Home Lab Needs**

XDA put together a list of “must‑have” home lab tools. I’ve used most of them over the years, and while the list is mostly solid, a couple of the picks feel like they were added because they’re trendy rather than essential.

Tailscale, for example, is basically WireGuard with a nice wrapper and a few convenience features. It’s great, but calling it a *must* depends on how much you value simplicity over raw control.  
NetBox, on the other hand, absolutely earns its spot. If you’re running a home lab with more than a handful of devices, proper documentation saves you from future‑you cursing past‑you.

Link: [6 Free Tools Every Home Lab Needs](https://www.xda-developers.com/free-tools-every-home-lab-needs/)

### **USB Ports, Explained Without the Headache**

USB standards have gotten so messy that even people who work in tech mix them up. USB 3.2 Gen 1 × 2? USB4 Version 2.0? At this point, the naming committee is just trolling us.

BGR has a clean breakdown that helps cut through the nonsense:

Link: [USB Port Standards, Speeds, and Types Explained](https://www.bgr.com/2063900/usb-port-standards-speeds-types-explained/)

---

## 💾 RAID 5: Once Great, Now… Not So Much

RAID 5 used to be the go‑to choice for anyone who wanted redundancy without giving up too much storage. For years it was the “set it and forget it” option for home labs, small businesses, and even plenty of enterprise setups. But modern hard drive sizes have quietly broken the math that made RAID 5 reliable in the first place.

As HDD capacities climbed into double‑digit terabytes, rebuild times stretched from hours into days. And the bigger the drive, the higher the chance of hitting an unrecoverable read error during a rebuild. That’s the nightmare scenario: one disk fails, you replace it, and during the rebuild another disk coughs up a bad sector — suddenly your entire array is toast.

This isn’t theoretical anymore. It’s common enough that most storage folks have quietly retired RAID 5 from anything mission‑critical. RAID 6, ZFS with RAID‑Z2, or even mirrored vdevs are the safer choices now, especially if you’re running 10 TB+ drives.

Link: [RAID 5 Used to Be Great — But Modern Large HDDs Broke It](https://www.xda-developers.com/raid-5-used-to-be-great-but-modern-large-hdds-broke-it/)

### RAID Comparison (Quick Reference)

| RAID Level | Fault Tolerance | Rebuild Risk on Large Drives | Notes |
|-----------|----------------|------------------------------|-------|
| **RAID 5** | 1‑disk failure | **High** | Not recommended for 10 TB+ drives |
| **RAID 6** | 2‑disk failure | Medium | Better safety margin, slower writes |
| **RAID‑Z1** | 1‑disk failure | High | Same issues as RAID 5 |
| **RAID‑Z2** | 2‑disk failure | Low | Best balance for large HDDs |
| **Mirrors** | Depends on layout | Low | Fast rebuilds, great for mixed workloads |

### What I Recommend for Home Labs in 2026

- **RAID‑Z2** if you’re using large spinning disks  
- **Mirrored vdevs** if you want performance and fast rebuilds  
- **Avoid RAID 5 entirely** unless you’re using small drives or you enjoy gambling  
- **Always** keep cold backups — redundancy is not backup

---

## 🏈 Sports

### **Denver Broncos Are the AFC’s #1 Playoff Seed!**

The Broncos wrapped up the season at 14–3 and locked down the #1 seed in the AFC. Not bad for a team still dragging around the last remnants of the Russell Wilson contract. The defense carried the load this year, and they did it convincingly enough that Defensive Coordinator Vance Joseph is already drawing interest — the Tennessee Titans have officially requested to interview him for their head coaching job.

Denver gets a week off, home‑field advantage, and a chance to make a real run. After the last few years, that alone feels like a small miracle.
