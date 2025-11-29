---
title: "Build a Mac OS 15 Sequoia VM?"
date: 2025-11-18T19:35:49-06:00
authors: ["ZDevilInside"]
draft: false
categories: ["Tech Tips"]
image: "vm.jpg"
tags: ["MacOS", "VMware", "Virtualization"]
description: "Step-by-step guide to building a Mac OS 15 Sequoia VM on Windows using VMware."
---

## Getting Started

**How to create a MacOS 15 Sequoia VM in VMware**

Apple has long marketed the Mac as the pinnacle of computing. While their hardware is polished, it comes at a premium price. For many Windows users, the appeal of macOS is curiosity rather than necessity. Fortunately, virtualization offers a way to explore macOS without buying Apple hardware.  

This guide walks you through building a **MacOS 15 Sequoia VM** on a Windows PC using VMware. It’s not always smooth sailing—there are quirks, patches, and patience required—but it’s a practical way to test macOS for development, compatibility, or just to satisfy curiosity.  

---

## Minimum Requirements

Before diving in, make sure your system can handle it:  

- **Processor**: Intel Core i-series or AMD Ryzen (8 cores recommended)  
- **RAM**: 8 GB minimum (16 GB recommended)  
- **Graphics**: iGPU or dedicated GPU  
- **Storage**: 2 GB for bare install, 90 GB with instruments and sounds  
- **Internet**: Recommended for activation and updates  

If your PC doesn’t meet these specs, the VM will struggle or fail to run.  

---

## Preparation Steps

1. **Download macOS Sequoia ISO** – [Internet Archive link](https://archive.org/details/install-mac-os-sequoia).  
2. **Download VMware Workstation Player** – [VMware Player](https://archive.org/download/vmware-player-full-17.5.0-22583795_202402/VMware-player-full-17.5.0-22583795.exe).  
3. **Download macOS Unlocker for VMware** – [GitHub Unlocker](https://github.com/DrDonk/unlocker/releases/).  
4. **Install VMware Player** – Accept defaults.  
5. **Run Unlocker** – Extract, run as administrator, and let it patch VMware.  

---

## Creating the Sequoia VM

1. Launch VMware Player → “Create a New Virtual Machine.”  
2. Select ISO file → choose macOS 15.  
3. Name your VM and set storage path.  
4. Allocate **100 GB disk** (single file).  
5. Customize hardware:  
   - RAM: 8–16 GB  
   - CPU: 4 cores  
   - Network: Bridged  
6. Edit `.vmx` file:  
   - Set `board-ID.reflectHost = FALSE`  
   - Change `ethernet0.virtualDev = vmxnet3`  
   - Add identifiers:  



board-id = \"Mac-AA95B1DDAB278B95\"\
hw.model.reflectHost = \"FALSE\"\
hw.model = \"iMac20,1\"\
serialNumber.reflectHost = \"FALSE\"\
serialNumber = \"C01234567890\"  

7. Save and start the VM.  

---

Installing MacOS Sequoia

If you have gotten this far, you will see a lot of Mac fanboys eating their hats and saying that it isn't proper to run a Mac OS VM! They are all hurt that their greatest thing doesn't have to be run on overpriced Apple hardware!

1.  After the bootup process completes, you should have Mac OS Setup open up.

2.  Select the language that you want the Mac OS Sequoia VM to be in. Click "next". 
   ![image 19](image19.png)
3.  Select Disk Utility and click on "Continue".
   ![image 20](image20.png)

4.  On the left side, right click on "VMware Virtual SATA Hard Drive Media" and then click "erase".
   ![image 21](image21.png)

5.  Name the MacOS drive, make sure the format is "APFS", and Scheme is "GUID Partition Map" and click "Erase".
   ![image 22](image22.png)

6.  Click "Done" and then close Disk Utility.
    ![image 23](image23.png)
   ![image 24](image24.png)

7.  Click "Install macOS Sequoia" and click "continue".
    ![image 25](image25.png)

8.  Click Continue, click Agree, click Agree once more.
   ![image 26](image26.png)![image 27](image27.png)![image 28](image28.png)
9.  Select the MacOS disk and then click on "install".

![image 29](image29.png)

a.  Wait until the end of the world...errrr...ummm...for Sequoia to install. The VM will reboot a few times, you can go for a swim across the ocean, or something else while it takes forever to do the install. ![image 30](image30.png)![image 31](image31.png)

<!-- -->

10. Once the installation finishes (or you felt like you are going to die of old age), select the country/region you want to set the VM up in. You get bonus points for talking back to "Hal" as it talks to you when this comes up.![image 32](image32.png)
11. Select your language and keyboard layouts, then click "Continue".
    ![image 33](image33.png)

12. Click "Not now", "skip" or whatever your setup requires to bypass the Accessibility screen.
   ![image 34](image34.png)

13. Do the same for the Data & Privacy screen -- well, do whatever you want to do here but I am not going to give Apple anything extra.
  ![image 35](image35.png)
14. Select "Not now", "skip" or whatever choice your scree gives you for the "Migration Assistant" bit. I am not going to tell you what to do there. That is entirely up to you but I am not going to help you with this part no matter what mess you create.
  ![image 36](image36.png)
15. Select "Set up later" and "skip" the Apple ID screen. Why would you want to do something stupid like this?
   ![image 37](image37.png)

16. Click agree, and then agree once more. Apple wants you to be agreeing to everything that they want you to do no matter what your true feelings are.
   ![image 38](image38.png)!

17. Enter a name, username, and the password you want to use. Click "continue". It could take a bit of time to create the account.[image 39](image39.png)

18. Click continue, and then if you want to use or not use "Location Services". I don't use it; I want to be hidden away as best as I can be when I do something like this.
   ![image 40](image40.png)

19. Pick the time zone you want to be using. Hey, US-based NFL fans. Did
    you know that you can set your time zone to Sydney Australia's on
    Super Bowl Sunday and learn the result of the game even before it is
    played in the US? Try it and find out!
    ![image 41](image41.png)
20. I unchecked the "Share Mac Analytics with Apple" faster than you
    could blink. I suggest you do the same.
    ![image 42](image42.png)

21. Click "set up later" on the Screen Time screen. Yeah, I will do that
    later....after this computer dies and is tossed in the trash.
   ![image 43](image43.png)

22. Pick a theme. Where is the Rocky 3 theme? How about Don't Worry, Be
    Happy? Oh, wait, this is a screen type theme. Choose the one that
    you want. ![image 44](image44.png)

23. Welcome to the lunacy of Apple! You can now run a Mac Virtual
    Machine on your Windows PC and freak the Apple Fanboys out with
    having greater hardware on your Windows computer while doing the
    exact same things as those idiots can do with their overpriced
    machines! ![image 45](image45.png)

24. Once you are on the desktop, go to the top of VMWare window, select
    "VM" from the menu, and select "Install VMware Tools". In the
    virtual machine, select "Install VMware Tools".
    ![image 46](image46.png)

Good luck! Pretty soon you will be banging your head like you are
listening to Quiet Riot once more!

A link to those that don't know the pop culture reference of above:
https://www.youtube.com/watch?v=O_1ruZWJigo
