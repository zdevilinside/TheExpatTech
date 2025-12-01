---
title: "Digital Nomad VPN Setup"
date: 2025-11-23
authors: ["ZDevilInside"]
categories: ["Digital Nomading", "Tech Tips"]
tags: ["Digital Nomading", "Tech Tips"]
image: "image1.jpg"
description: "Setting up your Digital Nomad VPN"
draft: false
slug: "digital-nomad-vpn-setup"
---

# 🚨 Secret - Restricted Data

## How to setup a Digital Nomad VPN system  

![Top Secret](TSRD.jpg)

###  **Unauthorized personnel beware!**  
###  This guide contains sensitive setup instructions.  
###  Proceed at your own risk — and remember, this is for educational purposes only.

***Management and Tech Investigation Teams are not authorized to continue past this point.***

---

### Prerequisites

1. Buy 2 GL.iNet routers — one full router and one travel router.  
   For recommended **GL.iNet devices**, [click here](/digital-nomading/recommended-vpn-hardware).  
2. We’ll be using **WireGuard** as the VPN technology.  
3. If you’re not using GL.iNet routers on both sides, this post isn’t for you.  
4. I’ll use a GL.iNet Beryl AX to demonstrate both the VPN server and client setup.  
5. Terminology:  
   - **Server** = “HOME” system (where you want to pretend to be).  
   - **Client** = the device you travel with (where you actually are).  
6. LAN = Local, WAN = World.  
7. Configure **port forwarding** on your ISP’s modem/router. Use UDP port 51820.  

---

# VPN Server – Where you want to pretend to be

1. Connect a CAT‑5e/Ethernet cable from your ISP modem/gateway/ONT to the router’s **WAN** port.  
   An easy way to remember which cable goes to what devices is look at the first letter of WAN/LAN.  
   WAN = World and therefore goes out the door (to your service provider), and LAN = Local and sticks inside the house.  
   This goes to your computer.  
   {{< figure src="image2.jpg" alt="WAN port" width="75%" >}}  

2. Connect another Ethernet cable from your computer to a **LAN** port on the router.  
3. Open your web browser and enter the router’s address.  
   {{< figure src="image3.jpg" alt="Router login" width="75%" >}}  

4. Set the router password, then click “Next.”  
   {{< figure src="image4.jpg" alt="Set password" width="75%" >}}  

5. On “Set Up Wi‑Fi,” leave defaults for now and click “Next.”  
   {{< figure src="image5.jpg" alt="Wi-Fi setup" width="75%" >}}  

6. After a few moments, click the blue “Exit” button.  
   {{< figure src="image6.jpg" alt="Exit setup" width="75%" >}}  

7. You should now see the main dashboard.  
   {{< figure src="image7.jpg" alt="Dashboard" width="75%" >}}  

8. Click “Cloud Services” on the left.  
   {{< figure src="image8.jpg" alt="Cloud services" width="75%" >}}  

9. Click “GoodCloud.”  
   {{< figure src="image9.jpg" alt="GoodCloud" width="75%" >}}  

10. Click “Get Started,” then “Enable.”  
    {{< figure src="image10.jpg" alt="Enable GoodCloud" width="75%" >}}  

11. Create an account and/or log in.  
    {{< figure src="image11.jpg" alt="GoodCloud login" width="75%" >}}  

12. Click outside the popup to return to the dashboard.  
    {{< figure src="image12.jpg" alt="Dashboard after login" width="75%" >}}  

13. Toggle on “Enable Remote SSH” and “Enable Remote Web Access,” then click Apply.  
    {{< figure src="image13.jpg" alt="Remote access toggles" width="75%" >}}  

14. Click “VPN” on the left, then select “WireGuard Server.”  
    {{< figure src="image14.jpg" alt="WireGuard server" width="75%" >}}  

15. Click “Generate Configuration.”  
    {{< figure src="image15.jpg" alt="Generate config" width="75%" >}}  

16. Click “Start.”  
    {{< figure src="image16.jpg" alt="Start server" width="75%" >}}  

17. Click the “Profiles” tab.  
    {{< figure src="image17.jpg" alt="Profiles tab" width="75%" >}}  

18. Click the blue “+ Add” button.  
    {{< figure src="image18.jpg" alt="Add profile" width="75%" >}}  

19. Name your client profile (e.g., “client”) and click “Apply.”  
    {{< figure src="image19.jpg" alt="Name profile" width="75%" >}}  

20. Click “Download” and save the config file somewhere safe.  
    {{< figure src="image20.jpg" alt="Download config" width="75%" >}}  

---

# VPN Client – The device you take with you

1. Click “WireGuard Client.”  
   {{< figure src="image14.jpg" alt="WireGuard client" width="75%" >}}  

2. Scroll down and click “+ Add Manually.”  
   {{< figure src="image21.jpg" alt="Add manually" width="75%" >}}  

3. Click “Select a file to upload or drag it here.”  
   {{< figure src="image22.jpg" alt="Upload config" width="75%" >}}  

4. Upload the config file you saved from the server setup.  
   {{< figure src="image23.jpg" alt="Select config file" width="75%" >}}  

5. Click “Apply.”  
   {{< figure src="image24.jpg" alt="Apply config" width="75%" >}}  

6. You should see the client profile listed.  
   {{< figure src="image25.jpg" alt="Client profile" width="75%" >}}  

7. Click the three dots (…) next to the profile, then click “Start.”  
   {{< figure src="image26.jpg" alt="Start client" width="75%" >}}  

8. A blue dot indicates the VPN is connected.  
   {{< figure src="image27.jpg" alt="Connected client" width="75%" >}}  

9. Click “VPN Dashboard” on the left.  
   {{< figure src="image28.jpg" alt="VPN dashboard" width="75%" >}}  

10. Turn on the **Kill Switch**.  
    {{< figure src="image29.jpg" alt="Kill switch toggle" width="75%" >}}  

11. Confirm Kill Switch is ON.  
    {{< figure src="image30.jpg" alt="Kill switch on" width="75%" >}}  

---

## Notes

- Leave the server plugged in and connected to your ISP while you’re away.  
- Make sure whoever hosts your server has a fast internet package—fiber preferred, cable second best.  
- Speed and latency are critical for smooth VPN use.

---

## 🌍 Reflection: Why this matters for digital nomads

A VPN setup like this isn’t just technical—it’s about freedom. A reliable VPN lets you work securely from anywhere, protect your privacy, and maintain access to the tools you need no matter where you are. Whether you’re in a café in Mexico, a coworking hub in Lisbon, or a mountain lodge in the Alps, this setup keeps your footprint safe while your lifestyle stays flexible.
