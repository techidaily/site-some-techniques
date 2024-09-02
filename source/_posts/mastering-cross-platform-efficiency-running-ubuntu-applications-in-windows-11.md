---
title: "Mastering Cross-Platform Efficiency: Running Ubuntu Applications in Windows 11"
date: 2024-09-01T01:23:22.490Z
updated: 2024-09-02T01:23:22.490Z
tags:
  - deals
categories:
  - tech
thumbnail: https://thmb.techidaily.com/d26b018bfd09d9f7c63fd1187a4536965f1d2b0dee90272569c4cc402ddd818e.jpg
---

## Mastering Cross-Platform Efficiency: Running Ubuntu Applications in Windows 11

### Key Takeaways

* Install WSL2 Kernel, activate Virtual Machine Platform, and make sure you have Admin rights before getting Ubuntu on Windows 11.
* Enable Windows Subsystem for Linux, then download and install Ubuntu for WSL via Microsoft Store to run Linux apps on Windows 11.

 Did you know using Ubuntu-exclusive apps doesn't require overwriting your operating system? Unlock the true potential of your Windows desktop by using Ubuntu apps on Windows 11, enhancing your PC experience by blending the power of Linux and Windows.

##  Why Use Ubuntu Apps on Windows 11?

 Adding Ubuntu to Windows 11 enables access to a wide variety of free applications unavailable on Windows alone. These aren't just ordinary programs either; they can accomplish nearly any task on your computer, from enhancing your file management to creative projects. For example, if you're looking for a great photo management tool not found on Windows 11, you might try [Shotwell](https://shotwell-project.org/doc/html/) with WSL. Or, if you're not a fan of the email apps available on Windows, you can install the Ubuntu-native [Geary](https://wiki.gnome.org/Apps/Geary) email client. There are many great exclusive applications for Ubuntu that can level up your Windows PC.

 Furthermore, if you enjoy crafting and coding, the combination of Windows and Ubuntu significantly benefits you. It simplifies the process of working on Linux-oriented projects without the need to leave the Windows environment. This integration reduces complications and amplifies productivity, whether your pursuits involve coding for enjoyment or constructing significant projects.

 Imagine you're a developer working on a cross-platform project. Using Ubuntu apps on Windows means you can quickly and effectively test your new project on Linux and Windows with ease. Take it from me: I write programs in the Go programming language, and being able to test out my code and run it on both Ubuntu and Windows 11 seamlessly is very powerful.

<!-- affiliate ads begin -->
<a href="https://united.elfm.net/c/5597632/517826/4704" target="_top" id="517826"><img src="//a.impactradius-go.com/display-ad/4704-517826" border="0" alt="" width="728" height="90"/></a><img height="0" width="0" src="https://united.elfm.net/i/5597632/517826/4704" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
##  Requirements Before You Begin

 Before you can start using Ubuntu on your Windows 11 system, a few requirements must be met to ensure a smooth process. During my testing, WSL wouldn't work until I installed the latest WSL2 Kernel package installed on Windows 11\. If you're having issues with WSL running on Windows 11 like I did, install this kernel package. It will ensure that WSL v2 operating systems run correctly. You can download and install the EXE file [directly from Microsoft](https://learn.microsoft.com/en-us/windows/wsl/install-manual#step-4---download-the-linux-kernel-update-package).

 In addition to the WSL2 Kernel EXE package, you'll need to enable the "Virtual Machine Platform" feature in the "Windows Features" area of Windows 11\. WSL runs with the help of virtualization, and this feature is a requirement to get the most out of Ubuntu in Windows 11.

 Lastly, ensure you have Administrator rights on your Windows 11 system. Using WSL requires modifying Windows features, and it won't work if you don't have Administrator privileges.

##  Enabling Windows Subsystem for Linux (WSL)

 Windows Subsystem for Linux is not enabled by default on Windows 11\. You'll need to activate this feature on Windows before you can use it to run Ubuntu apps on your Windows PC.

 To start, open the Windows Start Menu on the desktop. Once it is open, type "Turn Windows Features on or off" into the search box. Launch the icon labeled "Control Panel" beneath it to access the "Add/Remove Features" area of Windows 11.

 Inside the "Windows Features" window, scroll down and locate "Windows Subsystem for Linux." After finding it, click on the empty box next to it to activate this feature. Select "OK" after making your selection.

![WSL feature being turned on in Windows 11.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/03/flameshot-wsl-check-box.png) 

 Now that the "OK" button has been selected, Windows 11 will begin setting up WSL on your system. This setup process should take a few minutes to complete. When the setup is complete, you must reboot your Windows PC. Select the "Restart now" button to reboot.

 Upon rebooting, log back into your Windows 11 desktop. Once you've logged back in, the Windows Subsystem for Linux will be enabled on Windows 11.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2068425/7443" target="_top" id="2068425"><img src="//a.impactradius-go.com/display-ad/7443-2068425" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2068425/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
##  Installing Ubuntu

 Ubuntu for WSL is available for Windows 11 via the Microsoft Store, enabling the installation of Ubuntu on your system to run Linux apps within Windows 11.

 To initiate the installation of Ubuntu for WSL, open the Microsoft Store from the Windows 11 desktop. Once open, locate the "Search apps, games, movies, and more" box and click on it.

 In the search box, type "Ubuntu." Upon entering "Ubuntu," the Microsoft Store will display various versions of the Ubuntu app. Select "Ubuntu 22.04.3 LTS" using the mouse.

![The user is searching for Ubuntu WSL 22.04.3 LTS in the Microsoft Store.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/03/wsl-ubuntu-22.png) 

 After selecting "Ubuntu 22.04.3 LTS," you will be directed to its feature page in the Microsoft Store. Locate the "Get" button and click on it. Selecting the "Get" button will initiate the Ubuntu download for Windows 11.

 Downloading Ubuntu 22.04.3 LTS on Windows 11 should be swift, given the program's size is only about 560 MB. Once the download is complete, Ubuntu will be accessible in the Windows Start Menu.

 After Ubuntu 22.04.3 LTS has finished installing on Windows 11, access the Windows Start Menu, search for "Ubuntu 22.04.3 LTS," and launch it. Upon its first launch, Ubuntu will automatically configure itself and prepare for use.

![Ubuntu WSL is installing itself to Windows 11.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/03/wsl-ubuntu-is-installing.png) 

<!-- affiliate ads begin -->
<a href="https://cowinaudio.pxf.io/c/5597632/1116855/13794" target="_top" id="1116855"><img src="//a.impactradius-go.com/display-ad/13794-1116855" border="0" alt="" width="767" height="285"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1116855/13794" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 Once Ubuntu has finished its setup on Windows 11, you will see an empty terminal window, ready for you to interact with Ubuntu on your Windows 11 system.

##  Basic Configuration Tips

 Here are some basic configuration tips to improve the WSL experience on Windows 11.

###  Windows and Linux File System Integration

 Windows and Linux File System Integration simplifies moving files between your Ubuntu WSL setup and your Windows 11 desktop. Here's how to utilize this feature.

 To access your Ubuntu files from Windows 11, begin by opening Windows Explorer. Once opened, locate the "Linux" penguin icon in the sidebar and select it.

 Upon selecting "Linux," a folder named "Ubuntu-22.04" will appear. Right-click this folder and choose "Pin to Quick access." This action allows you to effortlessly access your Ubuntu files from Windows.

![Ubuntu WSL's file access in the Windows 11 Explorer app.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/03/wsl-selecting-ub.png) 

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=37540879&QTY=1&AFFILIATE=108875&CART=1"><img src="https://paperscan.orpalis.com/img/content/You_prefer_to_use.png" border="0">PaperScan Professional： PaperScan Scanner Software is a powerful TWAIN & WIA scanning application centered on one idea: making document acquisition an unparalleled easy task for anyone.</a>
<!-- affiliate ads end -->
 To access Windows files from Ubuntu, navigate to the **/mnt/c** folder using the cd command. This method provides interaction with the Windows 11 **C:/** drive.

cd /mnt/c

###  Update your Ubuntu WSL app

 It is good practice to update your Ubuntu WSL app from time to time, otherwise programs will stop working. Here's how to do it on Windows 11.

 First, open up the Ubuntu app from the Windows Start Menu. Once it is open, run the apt update command to check for Ubuntu software updates.

sudo apt update

 When you've finished checking for updates, you can use the apt upgrade command to install them.

sudo apt upgrade

![Ubuntu WSL is being updated.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/03/wsl-installing-kdenlive.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2082526/7443" target="_top" id="2082526"><img src="//a.impactradius-go.com/display-ad/7443-2082526" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2082526/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
<!-- affiliate ads begin -->
<a href="https://store.movavi.com/affiliate.php?ACCOUNT=MOVAVI&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.movavi.com%3FAFFILIATE%3D108875%26RESOURCE%3DMovavi%2BVideo%2BEditor%2Bbox"><img src="https://mcusercontent.com/0885a03ded3d480dca9287f12/images/6d3207fd-9f15-4c21-f0ad-59c68e6a7e2a.png" border="0"></a>
<!-- affiliate ads end -->
##  Starting and Using Ubuntu

 Ubuntu in Windows 11 has a terminal interface with WSL. WSL is a Linux system layer that is accessible directly from Windows, rather than a Linux desktop on top of the Windows Desktop.

 Using Ubuntu means installing packages to use on Windows 11\. To start Ubuntu, search for "Ubuntu 22.04.3 LTS" in the Windows Start Menu. Once it is opened, it'll be ready to use.

 From here, you can install any app you like. To install an Ubuntu app on your Windows 11 system, start by searching for the name of the app. You can search using the apt search command. For example, to find "wireshark," do:

apt search wireshark

 Look through the search results for the program you wish to install. Then, use the "apt install programname" command. To install Wireshark, for example, it's:

sudo apt install wireshark

 When your program is installed, you can launch it directly from the terminal with the following command:

nohup program_name & disown

![Linux apps Kdenlive and Wireshark are running inside of Windows 11.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/03/wsl-kdenlive-and-wireshark-open.png) 

 Alternatively, applications can be started from the Windows 11 start menu.

##  Integration with Windows 11

 When apps are installed through WSL, they integrate into Windows 11 quite well by installing themselves into the Windows 11 Start menu. To access your installed WSL programs from Windows 11, look through your programs. Each integrated application will have a Linux icon.

 The WSL integration with Windows 11 is quite good. However, keep in mind that not every single application is going to create a desktop icon. Sometimes, you may need to launch your Ubuntu programs directly from the terminal. You typically do this by typing its package name and hitting Enter.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=40203538&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/cc4b82e826b52ec41c810301548e8f48/products/audio-to-text-transcription-software.png" border="0">EaseText Audio to Text Converter for Windows (Personal Edition) - An intelligent tool to transcribe & convert audio to text freely </a>
<!-- affiliate ads end -->
##  Troubleshooting Common Setup Issues

 WSL usually installs without a hitch on Windows 11\. However, if you're having issues, there is a quick and easy fix. First, open up PowerShell in Windows 11\. Once it is open, use the update command for WSL. Updating WSL will install various patches and fixes that are sure to alleviate the issues you're experiencing.

wsl --update

 Alternatively, if updating doesn't help, consider re-installing Ubuntu WSL again by following the installation instructions in the "Setup" portion of this guide.

---

 WSL upgrades your Windows 11 experience by bringing Ubuntu apps to your desktop without the hassle of virtualization. Jump into Ubuntu and WSL to enhance the power of your Windows 11 PC and discover new possibilities in computing.

<ins class="adsbygoogle"
     style="display:block"
     data-ad-format="autorelaxed"
     data-ad-client="ca-pub-7571918770474297"
     data-ad-slot="1223367746"></ins>



<ins class="adsbygoogle"
     style="display:block"
     data-ad-client="ca-pub-7571918770474297"
     data-ad-slot="8358498916"
     data-ad-format="auto"
     data-full-width-responsive="true"></ins>

<span class="atpl-alsoreadstyle">Also read:</span>
<div><ul>
<li><a href="https://some-techniques.techidaily.com/new-expert-techniques-for-stellar-titling/"><u>[New] Expert Techniques for Stellar Titling</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-ffmpeg-audioscape-maintaining-original-audio-formats/"><u>[New] FFmpeg Audioscape  Maintaining Original Audio Formats</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-how-to-get-still-on-the-move-gopro-stability-tips/"><u>[New] How to Get Still on the Move  GoPro Stability Tips</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-how-to-revert-macos-from-latest-to-classic-el-capitan/"><u>[New] How to Revert MacOS From Latest to Classic - El Capitan</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-iconic-stop-motion-animations-15-best-ever/"><u>[New] Iconic Stop-Motion Animations - #15 Best Ever</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-expert-strategies-in-post-processing-colors/"><u>[Updated] Expert Strategies in Post-Processing Colors</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-high-quality-methodology-stitching-gopro-sequences-in-virtual-reality-films/"><u>[Updated] High-Quality Methodology  Stitching GoPro Sequences in Virtual Reality Films</u></a></li>
<li><a href="https://article-tips.techidaily.com/2024-approved-phantom-3-encounter-veil-4s-entry/"><u>2024 Approved  Phantom 3 Encounter  Veil 4'S Entry</u></a></li>
<li><a href="https://voice-adjusting.techidaily.com/2024-approved-perfecting-audio-precision-key-eq-settings-explored/"><u>2024 Approved Perfecting Audio Precision Key EQ Settings Explored</u></a></li>
<li><a href="https://some-techniques.techidaily.com/1723036597891-amazingly-durable-and-lightweight-comprehensive-guide-to-the-lg-gram-156-notebook-2018-model/"><u>Amazingly Durable and Lightweight - Comprehensive Guide to the LG Gram 15.6 Notebook (2018 Model)!</u></a></li>
<li><a href="https://tech-recovery.techidaily.com/efficient-movement-tactics-unlocking-the-power-of-teleport-in-minecraft/"><u>Efficient Movement Tactics: Unlocking the Power of Teleport in Minecraft</u></a></li>
<li><a href="https://howto.techidaily.com/google-play-services-wont-update-12-fixes-are-here-on-honor-magic-5-pro-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>Google Play Services Wont Update? 12 Fixes are Here on Honor Magic 5 Pro | Dr.fone</u></a></li>
<li><a href="https://howto.techidaily.com/google-play-services-wont-update-12-fixes-are-here-on-oneplus-ace-3-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>Google Play Services Wont Update? 12 Fixes are Here on OnePlus Ace 3 | Dr.fone</u></a></li>
<li><a href="https://blog-min.techidaily.com/how-to-restore-missing-photos-files-from-nord-3-5g-by-fonelab-android-recover-photos/"><u>How To  Restore Missing Photos Files from Nord 3 5G.</u></a></li>
<li><a href="https://tech-renaissance.techidaily.com/how-to-enable-dual-screen-setup-on-your-apple-devices/"><u>How To Enable Dual Screen Setup on Your Apple Devices</u></a></li>
<li><a href="https://blog-min.techidaily.com/how-to-recover-deleted-photos-from-android-gallery-app-on-galaxy-m34-5g-by-stellar-photo-recovery-android-mobile-photo-recover/"><u>How to Recover Deleted Photos from Android Gallery App on Galaxy M34 5G</u></a></li>
<li><a href="https://some-techniques.techidaily.com/ideal-culmination-in-virtual-ventures-for-2024/"><u>Ideal Culmination in Virtual Ventures for 2024</u></a></li>
<li><a href="https://android-transfer.techidaily.com/in-2024-android-to-apple-how-to-transfer-photos-from-samsung-galaxy-s23-ultra-to-ipad-easily-drfone-by-drfone-transfer-from-android-transfer-from-android/"><u>In 2024, Android to Apple How To Transfer Photos From Samsung Galaxy S23 Ultra to iPad Easily | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-exclusive-android-3d-video-enthusiasts-choice/"><u>In 2024, Exclusive Android 3D Video Enthusiasts' Choice</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-experience-the-next-level-of-virtual-reality-with-htcs-vive-headset/"><u>In 2024, Experience the Next Level of Virtual Reality with HTC's Vive Headset</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-flawless-tint-enhancer/"><u>In 2024, Flawless Tint Enhancer</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-full-review-capturing-every-angle-in-one-device-samsung/"><u>In 2024, Full Review  Capturing Every Angle in One Device - Samsung</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-hero-session-vs-hero-session-duel/"><u>In 2024, Hero Session Vs Hero Session Duel</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-hexed-harmonics-can-you-really-change-your-tone-discover-other-ways/"><u>In 2024, Hexed Harmonics  Can You Really Change Your Tone? Discover Other Ways</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-highlighting-the-best-ways-to-convert-youtube-to-mp4/"><u>In 2024, Highlighting the Best Ways to Convert YouTube to MP4</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-how-luts-revolutionize-color-balance-in-images/"><u>In 2024, How LUTs Revolutionize Color Balance in Images</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/in-2024-how-to-screen-share-on-apple-iphone-7-drfone-by-drfone-ios/"><u>In 2024, How to Screen Share on Apple iPhone 7? | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-hypervision-pro-all-in-one-4k-screen-desks/"><u>In 2024, HyperVision Pro  All-in-One 4K Screen Desks</u></a></li>
<li><a href="https://easy-unlock-android.techidaily.com/in-2024-mastering-android-device-manager-the-ultimate-guide-to-unlocking-your-nubia-red-magic-9-proplus-device-by-drfone-android/"><u>In 2024, Mastering Android Device Manager The Ultimate Guide to Unlocking Your Nubia Red Magic 9 Pro+ Device</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/in-2024-unlock-your-iphone-8-in-minutes-with-iccid-code-everything-you-need-to-know-by-drfone-ios/"><u>In 2024, Unlock Your iPhone 8 in Minutes with ICCID Code Everything You Need to Know</u></a></li>
<li><a href="https://some-techniques.techidaily.com/innovative-photo-display-solutions-for-2024/"><u>Innovative Photo Display Solutions for 2024</u></a></li>
<li><a href="https://program-issues.techidaily.com/overcoming-the-error-0xc0000005-glitch-in-call-of-duty-black-ops-cold-war/"><u>Overcoming the 'Error 0xC0000005' Glitch in Call of Duty: Black Ops Cold War</u></a></li>
<li><a href="https://win-howtos.techidaily.com/resolving-a-disk-read-malfunction-on-your-windows-11-pc-proven-solutions/"><u>Resolving a Disk Read Malfunction on Your Windows 11 PC - Proven Solutions</u></a></li>
<li><a href="https://fox-blue.techidaily.com/transforming-brands-with-language-mastery-techniques-for-2024/"><u>Transforming Brands with Language Mastery Techniques for 2024</u></a></li>
<li><a href="https://techidaily.com/your-complete-guide-to-reset-vivo-x-fold-2-drfone-by-drfone-reset-android-reset-android/"><u>Your Complete Guide To Reset Vivo X Fold 2 | Dr.fone</u></a></li>
</ul></div>
