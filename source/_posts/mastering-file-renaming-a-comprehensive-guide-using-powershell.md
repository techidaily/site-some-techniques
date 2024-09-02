---
title: "Mastering File Renaming: A Comprehensive Guide Using PowerShell"
date: 2024-09-01T01:23:23.854Z
updated: 2024-09-02T01:23:23.854Z
tags:
  - deals
categories:
  - tech
thumbnail: https://thmb.techidaily.com/2f5a7138163b464da142425b5cd4fc9ef8759bb9361cd872c71016b4ccd5a432.jpg
---

## Mastering File Renaming: A Comprehensive Guide Using PowerShell

### Quick Links

* [Before You Begin: Learn How to Find a File or Folder’s Full Path](https://video-capture.techidaily.com/new-top-5-xbox-external-hard-drive-you-can-find/)
* [How to Rename a Specific File](https://visual-screen-recording.techidaily.com/updated-vidmas-technology-in-screen-capturing-spotlighted/)
* [How to Rename Files in a Folder With an Increasing Number](https://bypass-frp.techidaily.com/easy-guide-how-to-bypass-xiaomi-redmi-note-12-proplus-5g-frp-android-10111213-by-drfone-android/)
* [How to Add a Prefix or Suffix to a File Name](https://facebook-video-share.techidaily.com/updated-2024-approved-achieving-excellent-illumination-on-youtube-videos/)
* [How to Add Timestamps to All Files in a Folder](https://extra-guidance.techidaily.com/srt-simplified-core-concepts-made-clear-for-2024/)

 PowerShell makes renaming files from the command line super easy. You can use specific names, add increasing numbers, add prefixes and suffixes, and even append timestamps. We’ll show you how to do that all on your Windows 11 or Windows 10 computer.

##  Before You Begin: Learn How to Find a File or Folder’s Full Path

 To rename files, you’ll have to provide PowerShell with your file or parent folder’s full path. If you know how to do this, skip to the relevant section below. If you aren’t quite sure [how to get a folder or file’s full path](https://fox-links.techidaily.com/updated-2024-approved-unparalleled-screenplay-craftsmanship-across-varied-fields/), we’ll show you.

[Open a File Explorer window](https://pokemon-go-android.techidaily.com/how-to-get-and-use-pokemon-go-promo-codes-on-realme-c67-4g-drfone-by-drfone-virtual-android/) and find your file or folder. Press and hold down the Shift key on your keyboard, right-click your file or folder, and choose "Copy as Path."

!['Copy as Path' highlighted in Windows 11's context menu.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/1-copy-file-path-windows.jpg) 

 That action has copied your selected item’s full path to your clipboard. You can now [paste this path](https://twitter-videos.techidaily.com/new-in-2024-gain-twitter-gifs-for-pc-download-made-simple/) wherever required in the commands below.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=194977&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.blumentals.net/scrfactory/images/screensaver-software.png" border="0">Screensaver Factory, Create stunning professional screensavers within minutes. Create screensavers for yourself, for marketing or unlimited royalty-free commercial distribution. Make screensavers from images, video and swf flash, add background music and smooth sprite and transition effects. Screensaver Factory is very easy to use, and it enables you to make self-installing screensaver files and CDs for easy setup and distribution. Screensaver Factory is the most advanced software of its kind.</a>
<!-- affiliate ads end -->
##  How to Rename a Specific File

 To give a new name to a specific file on your PC, use PowerShell’s Rename-Item [cmdlet](https://extra-guidance.techidaily.com/new-prophotomaster-the-ai-enhanced-editing-edge/). This cmdlet takes your file’s full path, the new name you want to assign, and renames your file.

 To use it, launch a PowerShell window on your PC and type the following command. In the command, replace **PATH** with the full path to your file. Your path should have the file’s full name as well as the extension. Replace **MyName** with the new name you want to use, and **ext** with your file’s original extension.

Rename-Item PATH -NewName MyName.ext

 Make sure to use your file’s original extension when you rename the file. Using another extension can make your file unusable.

 As an example, to rename a file named Old-Test.txt located on your desktop to New-Test.txt, you’d use the following command:

Rename-Item "C:\Users\Username\Desktop\Old-Test.txt" -NewName “New-Test.txt”

!['Rename-Item' cmdlet in a PowerShell window.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/2-rename-file-with-powershell.jpg) 

 PowerShell won’t display a message confirming your file is renamed, but know that the job is done.

<!-- affiliate ads begin -->
<a href="https://united.elfm.net/c/5597632/748964/4704" target="_top" id="748964"><img src="//a.impactradius-go.com/display-ad/4704-748964" border="0" alt="" width="300" height="250"/></a><img height="0" width="0" src="https://united.elfm.net/i/5597632/748964/4704" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
##  How to Rename Files in a Folder With an Increasing Number

 If you want to add an increasing number, such as 1, 2, 3, and so on, to your files in a specific folder, follow these steps.

 Launch a PowerShell window and type the following command. Replace **PATH** with the full path to your folder, and **txt** with the format of the files to rename. Then, press Enter.

Get-ChildItem PATH -Recurse -Include "*.txt" | ForEach-Object -Begin { $Counter = 1 } -Process { Rename-Item $_.FullName -NewName ("{0}_{1}" -f $Counter, $_.Name) ; $Counter++ }

![Files with an increasing number in File Explorer.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/3-add-numbers-to-file-names.jpg) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2087394/7443" target="_top" id="2087394"><img src="//a.impactradius-go.com/display-ad/7443-2087394" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2087394/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
<!-- affiliate ads begin -->
<a href="https://ursime.pxf.io/c/5597632/2092236/16384" target="_top" id="2092236"><img src="//a.impactradius-go.com/display-ad/16384-2092236" border="0" alt="" width="1920" height="329"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2092236/16384" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
##  How to Add a Prefix or Suffix to a File Name

 To add text before your file name (known as a prefix), launch a PowerShell window and enter the following command. Replace **PATH** with your folder's full path, and **PREFIX** with the text you want to append, then press Enter.

Get-ChildItem PATH | Rename-Item -NewName {"PREFIX" + $_.Name}

 To add text after your file’s name (called a suffix), use the following command, replacing **PATH** with the full path to your folder, and **SUFFIX** with the text to append. Then, press Enter.

Get-ChildItem PATH | Rename-Item -NewName {$_.BaseName + "SUFFIX" + $_.Extension}

<!-- affiliate ads begin -->
<a href="https://turtlebeacheu.sjv.io/c/5597632/1996818/23722" target="_top" id="1996818"><img src="//a.impactradius-go.com/display-ad/23722-1996818" border="0" alt="" width="600" height="600"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1996818/23722" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
##  How to Add Timestamps to All Files in a Folder

 If you want to add a timestamp to all the files in a folder, open PowerShell and type the following command. Replace **PATH** with the full path to your folder, and press Enter.

Get-ChildItem PATH -Recurse -Include "*.*" | ForEach-Object { Rename-Item -Path $_.FullName -NewName "$($_.DirectoryName)\$($_.BaseName)_$(Get-Date -F yyyy-MM-dd_HH-mm)$($_.Extension)"}

![Files with timestamp in File Explorer.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/4-add-timestamp-to-file-names.jpg) 

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4718728&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/ce9a6fb2becc2d235e62b125e9260102/products/vMixCallScreenshot1-large.jpg" border="0"> vMix Basic HD - Software based live production. vMix Basic HD includes 4 inputs, 3 cameras, streaming, recording, playlist. 
This bundle includes Studio 200 for vMix from Virtualsetworks, HTTP Matrix 1.0 automation scheduler, and 4 introductory training videos from the Udemy vMix Basic to Amazing course. </a>
<!-- affiliate ads end -->
 The above command uses your computer’s system time. If that time is incorrect, it’s possible to [change the timezone on your Windows 11](https://instagram-videos.techidaily.com/new-2024-approved-harnessing-the-power-of-hashtags-to-amplify-your-igtv-content/) and [Windows 10](https://extra-support.techidaily.com/in-2024-leveraging-daylight-in-home-interiors/) PC.

---

 And that’s how you assign new names one file at a time or in bulk on your Windows system, without using File Explorer. It's just one of the many ways that PowerShell aids with mundane Windows tasks.

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
<li><a href="https://instagram-video-files.techidaily.com/new-8-free-online-instagram-reels-downloaders-that-will-save-your-day/"><u>[New] 8 FREE Online Instagram Reels Downloaders That Will Save Your Day</u></a></li>
<li><a href="https://video-screen-grab.techidaily.com/new-best-methods-for-documenting-live-youtube-broadcasts/"><u>[New] Best Methods for Documenting Live YouTube Broadcasts</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-exploring-lgs-ultra-clear-4k-screen-capabilities/"><u>[New] Exploring LG's Ultra-Clear 4K Screen Capabilities</u></a></li>
<li><a href="https://twitter-videos.techidaily.com/new-fixing-audio-absence-in-online-shared-videos/"><u>[New] Fixing Audio Absence in Online Shared Videos</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-full-spectrum-visual-creativity-with-vsco/"><u>[New] Full Spectrum Visual Creativity with VSCO</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-gopro-hero5-black-vs-garmin-virb-ultra-30-which-better-2022-upda/"><u>[New] GoPro Hero5 Black VS Garmin VIRB Ultra 30  Which Better? [2022 Upda]</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-high-octane-comparison-gopro-hero-4-vs-drift-ghost-s/"><u>[New] High Octane Comparison  GoPro Hero 4 Vs. Drift Ghost-S</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-how-to-obtain-high-quality-unrestricted-photography/"><u>[New] How To Obtain High-Quality, Unrestricted Photography</u></a></li>
<li><a href="https://article-posts.techidaily.com/new-in-2024-unlocking-success-with-effective-video-praise-techniques/"><u>[New] In 2024, Unlocking Success with Effective Video Praise Techniques</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-inflatable-microphones-for-diverse-scenarios/"><u>[New] Inflatable Microphones for Diverse Scenarios</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-innovate-your-visual-narrative-the-10-best-text-upgrades/"><u>[New] Innovate Your Visual Narrative - The 10 Best Text Upgrades</u></a></li>
<li><a href="https://facebook-video-footage.techidaily.com/new-youngest-entrepreneur-in-media-lands-fortune-peak/"><u>[New] Youngest Entrepreneur in Media Lands Fortune Peak</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-gopro-hero-5-black-vs-nikon-keymission-170-action-camera-which-is-better/"><u>[Updated] GoPro Hero 5 Black vs Nikon Keymission 170 Action Camera  Which Is Better?</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-harness-the-power-of-picture-in-picture-on-chrome-platforms/"><u>[Updated] Harness the Power of Picture In Picture on Chrome Platforms</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-how-to-make-the-most-out-of-spotifys-advertising-features/"><u>[Updated] How to Make the Most Out of Spotify's Advertising Features</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-ideal-timekeepers-top-10-androidios-apps-for-your-big-day/"><u>[Updated] Ideal Timekeepers  Top 10 Android/iOS Apps for Your Big Day</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-in-depth-analysis-simplified-dynamic-range-photography/"><u>[Updated] In-Depth Analysis  Simplified Dynamic Range Photography</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-innovative-methods-to-enhance-images-through-cropping/"><u>[Updated] Innovative Methods to Enhance Images Through Cropping</u></a></li>
<li><a href="https://vimeo-videos.techidaily.com/updated-techniques-for-downloading-vimeo-media-as-mp3/"><u>[Updated] Techniques for Downloading Vimeo Media as MP3</u></a></li>
<li><a href="https://screen-video-capture.techidaily.com/updated-top-picks-crafting-mc-villages-abodes/"><u>[Updated] Top Picks  Crafting MC Villages' Abodes</u></a></li>
<li><a href="https://extra-approaches.techidaily.com/2024-approved-iphones-made-simple-how-to-save-and-savor-animated-images/"><u>2024 Approved  IPhones Made Simple  How to Save and Savor Animated Images</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/3-best-tools-to-hard-reset-infinix-note-30-drfone-by-drfone-reset-android-reset-android/"><u>3 Best Tools to Hard Reset Infinix Note 30 | Dr.fone</u></a></li>
<li><a href="https://extra-information.techidaily.com/counteracting-loss-of-live-streams-on-twitch/"><u>Counteracting Loss of Live Streams on Twitch</u></a></li>
<li><a href="https://extra-hints.techidaily.com/craftsmanship-at-fingertips-discovering-apples-8-excellent-drawing-apps/"><u>Craftsmanship at Fingertips  Discovering Apple's 8 Excellent Drawing Apps</u></a></li>
<li><a href="https://tech-recovery.techidaily.com/find-out-what-we-consider-the-most-fantastic-current-ipad-bargains/"><u>Find Out What We Consider the Most Fantastic Current iPad Bargains</u></a></li>
<li><a href="https://some-techniques.techidaily.com/guffaw-generator-cyborg-comic-coders-for-2024/"><u>Guffaw Generator  Cyborg Comic Coders for 2024</u></a></li>
<li><a href="https://techidaily.com/hard-resetting-an-oppo-find-x6-device-made-easy-drfone-by-drfone-reset-android-reset-android/"><u>Hard Resetting an Oppo Find X6 Device Made Easy | Dr.fone</u></a></li>
<li><a href="https://win-blog.techidaily.com/how-i-fixed-persistent-league-of-legends-connectivity-errors/"><u>How I Fixed Persistent League of Legends Connectivity Errors</u></a></li>
<li><a href="https://some-techniques.techidaily.com/how-to-stay-grounded-in-virtual-reality-spaces-for-2024/"><u>How to Stay Grounded in Virtual Reality Spaces for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-experts-choice-7-premium-videos-on-mac/"><u>In 2024, Expert's Choice  7 Premium Videos on Mac</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-experts-choice-best-hdmi-21-display-models-evaluated/"><u>In 2024, Expert's Choice  Best HDMI 2.1 Display Models Evaluated</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-exploring-sierra-icloud-drives-a-complete-overview/"><u>In 2024, Exploring Sierra iCloud Drives – A Complete Overview</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-exploring-the-most-reliable-free-srt-translation-services/"><u>In 2024, Exploring the Most Reliable Free SRT Translation Services</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-film-lovers-ultimate-selection-of-stop-motion-works/"><u>In 2024, Film Lovers' Ultimate Selection of Stop-Motion Works</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-flippant-entry-and-exit-tips/"><u>In 2024, Flippant Entry & Exit Tips</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-how-to-manipulate-iphone-pics-flip-tilt-and-more/"><u>In 2024, How to Manipulate iPhone Pics  Flip, Tilt & More</u></a></li>
<li><a href="https://change-location.techidaily.com/in-2024-pokemon-go-cooldown-chart-on-vivo-y78t-drfone-by-drfone-virtual-android/"><u>In 2024, Pokémon Go Cooldown Chart On Vivo Y78t | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-depth-analysis-and-methods-with-morphvox-sound-alteration-for-2024/"><u>In-Depth Analysis and Methods with MorphVOX Sound Alteration for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-depth-study-androids-lightroom-app-functionality-for-2024/"><u>In-Depth Study  Android's Lightroom App Functionality for 2024</u></a></li>
<li><a href="https://tech-hub.techidaily.com/overcoming-chatgpt-disruption-during-conversation/"><u>Overcoming ChatGPT Disruption During Conversation</u></a></li>
<li><a href="https://program-issues.techidaily.com/ultimate-guide-resolving-pubg-mobiles-lag-and-unresponsiveness-on-desktop/"><u>Ultimate Guide: Resolving PUBG Mobile's Lag and Unresponsiveness on Desktop</u></a></li>
<li><a href="https://audio-shaping.techidaily.com/updated-in-2024-cutting-edge-audio-tools-for-iphone-and-ipad-enthusiasts/"><u>Updated In 2024, Cutting-Edge Audio Tools for iPhone and iPad Enthusiasts</u></a></li>
<li><a href="https://some-approaches.techidaily.com/utilizing-b-footage-an-essential-filmmaking-skill-for-2024/"><u>Utilizing B-Footage  An Essential Filmmaking Skill for 2024</u></a></li>
</ul></div>
