---
title: "Network Troubleshooting Scripts"
date: 2025-10-01T19:35:49-06:00
authors: ["ZDevilInside"]
draft: false
categories: ["Tech Tips"]
image: "test.jpg"
description: "Useful network troubleshooting scripts."
---

## Why I Built These Scripts

I recently ran into problems with my **Digital Nomad VPN setup**. When I asked for help on the GL.iNet Discord, the community wanted results from various diagnostic tests before they could assist. I provided the outputs, but the process felt scattered and inefficient.  

I noticed that these kinds of questions—*“Can you run a ping?”*, *“What’s your traceroute?”*, *“Do you have logs?”*—were asked constantly in the tech support channels. Yet there wasn’t a simple, unified way to gather all the relevant information in one place. That’s when I decided to create my own troubleshooting scripts.  

---

## Collaboration and Evolution

With the assistance of **“Wicked Yoda”**, I built a set of scripts that automate common diagnostic tasks and output logs in a clean, shareable format. Wicked has since taken the torch and expanded the project into a more robust toolkit.  

- 🔗 Current project: [Network-Diag-Utilities by Wicked Yoda](https://github.com/wickedyoda/Network-Diag-Utilities)  
- 📂 My original scripts: [network_testing_scripts](https://github.com/zdevilinside/network_testing_scripts/tree/main)  

These tools are designed to save time, reduce repetitive questions, and make troubleshooting VPN and network issues more straightforward.  

---

## What the Scripts Do

The scripts combine several common diagnostic commands into one workflow:  

- **Ping tests** – Verify connectivity to key endpoints.  
- **Traceroute** – Identify where packets are being delayed or dropped.  
- **DNS resolution checks** – Confirm that your DNS servers are working properly.  
- **VPN tunnel verification** – Test whether traffic is actually flowing through the VPN.  
- **Log collection** – Bundle results into a single file for easy sharing with support teams.  

Instead of running each command manually, the scripts automate the process and produce a consolidated report.  

---

## ✨ Did You Know? Troubleshooting Insights

- 🛠️ **Consistency Matters** – Running the same set of tests every time makes it easier to spot patterns.  
- 🌍 **VPN Complexity** – Problems often come from DNS leaks, misconfigured routes, or firewall rules.  
- 📑 **Logs Save Time** – Support teams can diagnose issues faster when they see complete logs upfront.  
- 🤝 **Community Driven** – Many open-source tools like this start as one person’s frustration and grow through collaboration.  

---

## Reflection

For digital nomads and remote workers, reliable networking is non‑negotiable. When VPNs fail, productivity grinds to a halt. These scripts were born out of necessity—my own frustration with scattered troubleshooting—and evolved into a community resource.  

By automating diagnostics, they reduce friction, save time, and empower users to provide clear information when asking for help. Whether you’re a seasoned IT pro or just trying to keep your VPN stable while traveling, these tools can make troubleshooting less painful and more effective.  

{{< figure src="kittentechs.jpeg" alt="image 1" >}}
