---
title: "Bridging Operating Systems: Utilizing WSL for Running Ubuntu Apps on Windows 11"
date: 2024-09-01T01:20:06.450Z
updated: 2024-09-02T01:20:06.450Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://thmb.techidaily.com/ddfdfc8e69381106d1b66c2809b663a8f7e41d96d0a4215acf2250fc3083c5a7.jpg
---

## Bridging Operating Systems: Utilizing WSL for Running Ubuntu Apps on Windows 11

### Key Takeaways

* Install WSL2 Kernel, activate Virtual Machine Platform, and make sure you have Admin rights before getting Ubuntu on Windows 11.
* Enable Windows Subsystem for Linux, then download and install Ubuntu for WSL via Microsoft Store to run Linux apps on Windows 11.

 Did you know using Ubuntu-exclusive apps doesn't require overwriting your operating system? Unlock the true potential of your Windows desktop by using Ubuntu apps on Windows 11, enhancing your PC experience by blending the power of Linux and Windows.

##  Why Use Ubuntu Apps on Windows 11?

 Adding Ubuntu to Windows 11 enables access to a wide variety of free applications unavailable on Windows alone. These aren't just ordinary programs either; they can accomplish nearly any task on your computer, from enhancing your file management to creative projects. For example, if you're looking for a great photo management tool not found on Windows 11, you might try [Shotwell](https://shotwell-project.org/doc/html/) with WSL. Or, if you're not a fan of the email apps available on Windows, you can install the Ubuntu-native [Geary](https://wiki.gnome.org/Apps/Geary) email client. There are many great exclusive applications for Ubuntu that can level up your Windows PC.

 Furthermore, if you enjoy crafting and coding, the combination of Windows and Ubuntu significantly benefits you. It simplifies the process of working on Linux-oriented projects without the need to leave the Windows environment. This integration reduces complications and amplifies productivity, whether your pursuits involve coding for enjoyment or constructing significant projects.

 Imagine you're a developer working on a cross-platform project. Using Ubuntu apps on Windows means you can quickly and effectively test your new project on Linux and Windows with ease. Take it from me: I write programs in the Go programming language, and being able to test out my code and run it on both Ubuntu and Windows 11 seamlessly is very powerful.

##  Requirements Before You Begin

 Before you can start using Ubuntu on your Windows 11 system, a few requirements must be met to ensure a smooth process. During my testing, WSL wouldn't work until I installed the latest WSL2 Kernel package installed on Windows 11\. If you're having issues with WSL running on Windows 11 like I did, install this kernel package. It will ensure that WSL v2 operating systems run correctly. You can download and install the EXE file [directly from Microsoft](https://learn.microsoft.com/en-us/windows/wsl/install-manual#step-4---download-the-linux-kernel-update-package).

 In addition to the WSL2 Kernel EXE package, you'll need to enable the "Virtual Machine Platform" feature in the "Windows Features" area of Windows 11\. WSL runs with the help of virtualization, and this feature is a requirement to get the most out of Ubuntu in Windows 11.

 Lastly, ensure you have Administrator rights on your Windows 11 system. Using WSL requires modifying Windows features, and it won't work if you don't have Administrator privileges.

<!-- affiliate ads begin -->
<a href="https://printrendy.pxf.io/c/5597632/1453721/17020" target="_top" id="1453721"><img src="//a.impactradius-go.com/display-ad/17020-1453721" border="0" alt="" width="300" height="250"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1453721/17020" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
##  Enabling Windows Subsystem for Linux (WSL)

 Windows Subsystem for Linux is not enabled by default on Windows 11\. You'll need to activate this feature on Windows before you can use it to run Ubuntu apps on your Windows PC.

 To start, open the Windows Start Menu on the desktop. Once it is open, type "Turn Windows Features on or off" into the search box. Launch the icon labeled "Control Panel" beneath it to access the "Add/Remove Features" area of Windows 11.

 Inside the "Windows Features" window, scroll down and locate "Windows Subsystem for Linux." After finding it, click on the empty box next to it to activate this feature. Select "OK" after making your selection.

![WSL feature being turned on in Windows 11.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/03/flameshot-wsl-check-box.png) 

 Now that the "OK" button has been selected, Windows 11 will begin setting up WSL on your system. This setup process should take a few minutes to complete. When the setup is complete, you must reboot your Windows PC. Select the "Restart now" button to reboot.

 Upon rebooting, log back into your Windows 11 desktop. Once you've logged back in, the Windows Subsystem for Linux will be enabled on Windows 11.

<!-- affiliate ads begin -->
<a href="https://25home.pxf.io/c/5597632/2090698/16836" target="_top" id="2090698"><img src="//a.impactradius-go.com/display-ad/16836-2090698" border="0" alt="" width="720" height="300"/></a>
<!-- affiliate ads end -->
##  Installing Ubuntu

 Ubuntu for WSL is available for Windows 11 via the Microsoft Store, enabling the installation of Ubuntu on your system to run Linux apps within Windows 11.

 To initiate the installation of Ubuntu for WSL, open the Microsoft Store from the Windows 11 desktop. Once open, locate the "Search apps, games, movies, and more" box and click on it.

 In the search box, type "Ubuntu." Upon entering "Ubuntu," the Microsoft Store will display various versions of the Ubuntu app. Select "Ubuntu 22.04.3 LTS" using the mouse.

![The user is searching for Ubuntu WSL 22.04.3 LTS in the Microsoft Store.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/03/wsl-ubuntu-22.png) 

<!-- affiliate ads begin -->
<a href="https://ephamedtechinc.pxf.io/c/5597632/2097466/26400?prodsku=B700" target="_top" id="2097466"><img src="//a.impactradius-go.com/display-ad/26400-2097466" border="0" alt="" width="2048" height="1024"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2097466/26400" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 After selecting "Ubuntu 22.04.3 LTS," you will be directed to its feature page in the Microsoft Store. Locate the "Get" button and click on it. Selecting the "Get" button will initiate the Ubuntu download for Windows 11.

 Downloading Ubuntu 22.04.3 LTS on Windows 11 should be swift, given the program's size is only about 560 MB. Once the download is complete, Ubuntu will be accessible in the Windows Start Menu.

 After Ubuntu 22.04.3 LTS has finished installing on Windows 11, access the Windows Start Menu, search for "Ubuntu 22.04.3 LTS," and launch it. Upon its first launch, Ubuntu will automatically configure itself and prepare for use.

![Ubuntu WSL is installing itself to Windows 11.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/03/wsl-ubuntu-is-installing.png) 

 Once Ubuntu has finished its setup on Windows 11, you will see an empty terminal window, ready for you to interact with Ubuntu on your Windows 11 system.

##  Basic Configuration Tips

 Here are some basic configuration tips to improve the WSL experience on Windows 11.

###  Windows and Linux File System Integration

 Windows and Linux File System Integration simplifies moving files between your Ubuntu WSL setup and your Windows 11 desktop. Here's how to utilize this feature.

 To access your Ubuntu files from Windows 11, begin by opening Windows Explorer. Once opened, locate the "Linux" penguin icon in the sidebar and select it.

 Upon selecting "Linux," a folder named "Ubuntu-22.04" will appear. Right-click this folder and choose "Pin to Quick access." This action allows you to effortlessly access your Ubuntu files from Windows.

![Ubuntu WSL's file access in the Windows 11 Explorer app.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/03/wsl-selecting-ub.png) 

 To access Windows files from Ubuntu, navigate to the **/mnt/c** folder using the cd command. This method provides interaction with the Windows 11 **C:/** drive.

cd /mnt/c

<!-- affiliate ads begin -->
<a href="https://boody-eco-wear.pxf.io/c/5597632/1567905/13846" target="_top" id="1567905"><img src="//a.impactradius-go.com/display-ad/13846-1567905" border="0" alt="" width="300" height="250"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1567905/13846" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
###  Update your Ubuntu WSL app

 It is good practice to update your Ubuntu WSL app from time to time, otherwise programs will stop working. Here's how to do it on Windows 11.

 First, open up the Ubuntu app from the Windows Start Menu. Once it is open, run the apt update command to check for Ubuntu software updates.

sudo apt update

 When you've finished checking for updates, you can use the apt upgrade command to install them.

sudo apt upgrade

![Ubuntu WSL is being updated.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/03/wsl-installing-kdenlive.png) 

<!-- affiliate ads begin -->
<a href="https://store.massmailsoftware.com/order/checkout.php?PRODS=2069351&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/dc87c13749315c7217cdc4ac692e704c/banera_for_partners-24_%282%29.jpg" border="0"></a>
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

<!-- affiliate ads begin -->
<a href="https://aidotcom.pxf.io/c/5597632/2086436/19576" target="_top" id="2086436"><img src="//a.impactradius-go.com/display-ad/19576-2086436" border="0" alt="" width="1500" height="400"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2086436/19576" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 Alternatively, applications can be started from the Windows 11 start menu.

##  Integration with Windows 11

 When apps are installed through WSL, they integrate into Windows 11 quite well by installing themselves into the Windows 11 Start menu. To access your installed WSL programs from Windows 11, look through your programs. Each integrated application will have a Linux icon.

 The WSL integration with Windows 11 is quite good. However, keep in mind that not every single application is going to create a desktop icon. Sometimes, you may need to launch your Ubuntu programs directly from the terminal. You typically do this by typing its package name and hitting Enter.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4599951&QTY=1&AFFILIATE=108875&CART=1"><iframe width="864" height="500" src="https://www.youtube.com/embed/jVnfr5HudQw" title="The Latest and Easiest Solution to Remove Kindle DRM on Windows (without Degrading)" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
Epubor Ultimate for Win：Helps you read books anywhere, including the best eBook Converter + eBook DRM Removal functions.</a>
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
<li><a href="https://screen-mirroring-recording.techidaily.com/updated-audio-quality-boost-for-skype-calls/"><u>[Updated] Audio Quality Boost for Skype Calls</u></a></li>
<li><a href="https://fox-direct.techidaily.com/updated-utilizing-edges-split-screen-feature-pip/"><u>[Updated] Utilizing Edge's Split Screen Feature  PIP</u></a></li>
<li><a href="https://fox-boxes.techidaily.com/2024-approved-discover-the-best-methods-to-record-audio-using-windows-11-tools/"><u>2024 Approved  Discover the Best Methods to Record Audio Using Windows 11 Tools</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/2024-approved-seamless-transformation-best-face-editors-on-iphones-and-androids/"><u>2024 Approved  Seamless Transformation  Best Face Editors on iPhones and Androids</u></a></li>
<li><a href="https://bypass-frp.techidaily.com/addrom-bypass-an-android-tool-to-unlock-frp-lock-screen-for-your-xiaomi-redmi-note-13-proplus-5g-by-drfone-android/"><u>AddROM Bypass An Android Tool to Unlock FRP Lock Screen For your Xiaomi Redmi Note 13 Pro+ 5G</u></a></li>
<li><a href="https://some-techniques.techidaily.com/athenahealth-accelerates-healthcare-efficiency-transforming-20-million-documents-weekly-through-abbyy-digital-solutions/"><u>Athenahealth Accelerates Healthcare Efficiency: Transforming 20 Million Documents Weekly Through ABBYY Digital Solutions</u></a></li>
<li><a href="https://some-techniques.techidaily.com/automated-with-cookiebot-enhance-your-sites-performance/"><u>Automated with Cookiebot: Enhance Your Site's Performance</u></a></li>
<li><a href="https://extra-information.techidaily.com/av1-triumph-surpassing-vp9-performance-for-2024/"><u>AV1 Triumph  Surpassing VP9 Performance for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/boost-metro-ags-transaction-speed-for-bulk-customers-by-90-using-abbyy-solutions/"><u>Boost Metro AG's Transaction Speed for Bulk Customers by 90%% Using ABBYY Solutions</u></a></li>
<li><a href="https://some-techniques.techidaily.com/boost-your-sites-traffic-with-the-help-of-cookiebot-the-ultimate-seo-solution/"><u>Boost Your Site's Traffic with the Help of Cookiebot: The Ultimate SEO Solution</u></a></li>
<li><a href="https://some-techniques.techidaily.com/boosting-online-engagement-with-advanced-cookiebot-marketing-tools/"><u>Boosting Online Engagement with Advanced Cookiebot Marketing Tools</u></a></li>
<li><a href="https://some-techniques.techidaily.com/convert-books-and-documents-to-editable-text-with-ios-scanner-and-ocr-app/"><u>Convert Books & Documents to Editable Text with iOS Scanner & OCR App</u></a></li>
<li><a href="https://some-techniques.techidaily.com/cookiebot-driven-analytics-enhancing-your-digital-marketing-strategy/"><u>Cookiebot-Driven Analytics: Enhancing Your Digital Marketing Strategy</u></a></li>
<li><a href="https://some-techniques.techidaily.com/cookiebot-driven-customized-user-experiences/"><u>Cookiebot-Driven Customized User Experiences</u></a></li>
<li><a href="https://some-techniques.techidaily.com/cookiebot-enabled-enhancing-your-websites-user-experience-with-advanced-tracking/"><u>Cookiebot-Enabled: Enhancing Your Website's User Experience with Advanced Tracking</u></a></li>
<li><a href="https://some-techniques.techidaily.com/cookiebot-enhanced-experience-the-ultimate-personalization-tool/"><u>Cookiebot-Enhanced Experience: The Ultimate Personalization Tool</u></a></li>
<li><a href="https://some-techniques.techidaily.com/cookiebot-enhanced-boosting-your-sites-engagement-with-cutting-edge-marketing-tech/"><u>Cookiebot-Enhanced: Boosting Your Site's Engagement with Cutting-Edge Marketing Tech</u></a></li>
<li><a href="https://some-techniques.techidaily.com/cookiebots-effective-consent-solutions-for-seamless-online-tracking-and-analytics/"><u>Cookiebot's Effective Consent Solutions for Seamless Online Tracking and Analytics</u></a></li>
<li><a href="https://facebook.techidaily.com/deciphering-social-media-insights-from-facebooks-openness-hub/"><u>Deciphering Social Media: Insights From Facebook's Openness Hub</u></a></li>
<li><a href="https://some-techniques.techidaily.com/driving-growth-through-cookiebot-integration-boost-your-sites-performance-and-seo/"><u>Driving Growth Through Cookiebot Integration - Boost Your Site's Performance and SEO</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/easy-steps-to-recover-deleted-music-from-honor-magic-6-by-fonelab-android-recover-music/"><u>Easy steps to recover deleted music from Honor Magic 6</u></a></li>
<li><a href="https://some-techniques.techidaily.com/enhance-digital-footprint-the-evolution-of-tracking-through-cookiebot/"><u>Enhance Digital Footprint: The Evolution of Tracking Through Cookiebot</u></a></li>
<li><a href="https://some-techniques.techidaily.com/enhance-hiring-processes-with-abbyy-ocr-technology-for-advanced-candidate-management-systems/"><u>Enhance Hiring Processes with ABBYY OCR Technology for Advanced Candidate Management Systems</u></a></li>
<li><a href="https://some-techniques.techidaily.com/enhance-user-experience-and-conversions-using-cookiebot-solutions/"><u>Enhance User Experience and Conversions Using Cookiebot Solutions</u></a></li>
<li><a href="https://some-techniques.techidaily.com/enhance-your-website-with-personalization-features-via-cookiebot/"><u>Enhance Your Website with Personalization Features via Cookiebot</u></a></li>
<li><a href="https://some-techniques.techidaily.com/enhance-your-website-with-smart-traffic-insights-from-cookiebot-technology/"><u>Enhance Your Website with Smart Traffic Insights From Cookiebot Technology</u></a></li>
<li><a href="https://some-techniques.techidaily.com/enhanced-functionality-via-advanced-cookiebot-solutions/"><u>Enhanced Functionality via Advanced Cookiebot Solutions</u></a></li>
<li><a href="https://some-techniques.techidaily.com/enhanced-personalization-through-the-latest-innovations-of-cookiebot-platforms/"><u>Enhanced Personalization Through the Latest Innovations of Cookiebot Platforms</u></a></li>
<li><a href="https://android-transfer.techidaily.com/in-2024-how-to-transfer-music-from-nubia-red-magic-8s-pro-to-ipod-drfone-by-drfone-transfer-from-android-transfer-from-android/"><u>In 2024, How to Transfer Music from Nubia Red Magic 8S Pro to iPod | Dr.fone</u></a></li>
<li><a href="https://pokemon-go-android.techidaily.com/in-2024-will-pokemon-go-ban-the-account-if-you-use-pgsharp-on-poco-m6-pro-4g-drfone-by-drfone-virtual-android/"><u>In 2024, Will Pokémon Go Ban the Account if You Use PGSharp On Poco M6 Pro 4G | Dr.fone</u></a></li>
</ul></div>
