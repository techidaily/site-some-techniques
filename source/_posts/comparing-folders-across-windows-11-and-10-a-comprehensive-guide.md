---
title: Comparing Folders Across Windows 11 & 10 - A Comprehensive Guide
date: 2024-09-01T01:24:02.960Z
updated: 2024-09-02T01:24:02.960Z
tags:
  - deals
categories:
  - tech
thumbnail: https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/52846060984_17cb6c3aa6_o.jpg
---

## Comparing Folders Across Windows 11 & 10 - A Comprehensive Guide

### Quick Links

* [Compare Folders From Properties](https://tech-recovery.techidaily.com/the-ultimate-fix-for-when-youtube-comments-wont-load/)
* [Compare Folders Using Command Prompt](https://video-capture.techidaily.com/new-in-2024-exacting-speech-recognition-via-googles-precision-tools/)
* [Compare Folders With WinMerge](https://win-howtos.techidaily.com/how-to-repair-when-your-macs-trackpad-wont-respond/)

### Key Takeaways

* One way to compare folders is to right-click your folders one at a time and choose "Properties" for each. Then compare the Properties window of each folder.
* The robocopy command is a command-line tool that can be used to view the differences between folder.
* Use WinMerge to compare the contents and details of folders if you want a graphical tool.

 Do you want to compare the number of files or folders or simply visualize the difference between two folders? If so, you have two graphical and one command line method to do that. We’ll show you how to perform the folder comparison task on your Windows 11 or Windows 10 PC.

##  Compare Folders From Properties

 To compare the number of files, subfolders, the size, and the creation date of two folders, use the Properties option in Windows File Explorer. This lets you quickly glance at the main attributes of a folder.

 To start, [launch File Explorer](https://pokemon-go-android.techidaily.com/how-to-get-and-use-pokemon-go-promo-codes-on-realme-c67-4g-drfone-by-drfone-virtual-android/) using Windows+E. Find the first folder, right-click it, and select "Properties."

!['Properties' highlighted for a folder in File Explorer.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/1-folder-properties.jpg) 

<!-- affiliate ads begin -->
<a href="https://zonlipartnershipprogram.pxf.io/c/5597632/1821134/17882" target="_top" id="1821134"><img src="//a.impactradius-go.com/display-ad/17882-1821134" border="0" alt="" width="320" height="250"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1821134/17882" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 Keep the first folder’s "Properties" window open. Then, find the second folder, right-click it, and select "Properties."

 You now have the "Properties" window open for both your folders. Bring these windows side-by-side by [dragging them](https://extra-resources.techidaily.com/mastering-complex-video-effects-and-transitions-in-gopro-studio/), and you can see the differences in the contents of these folders. For example, you can see how many files both folders have, what size these folders are, and so on.

!['Properties' windows for two folders in File Explorer.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/2-compare-folder-properties.jpg) 

 That gives you a general overview of the differences between your folders.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2082538/7443" target="_top" id="2082538"><img src="//a.impactradius-go.com/display-ad/7443-2082538" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2082538/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
##  Compare Folders Using Command Prompt

 If you prefer command line methods over graphical ones, use the robocopy command in Command Prompt to see the differences between the two folders. This command is actually for [copying files from one folder to another](https://twitter-videos.techidaily.com/new-in-2024-gain-twitter-gifs-for-pc-download-made-simple/), but you can make it show the differences between two specified folders and not copy any files.

 To use robocopy, first open the Start Menu, search **Command Prompt**, and launch it.

![Command Prompt highlighted in Start Menu.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/3-launch-command-prompt.jpg) 

 In Command Prompt, type the following command. Replace "Folder1" with the path to your first folder and "Folder2" with the path to your second folder. Ensure both folder paths are enclosed in double quotes.

 To copy a folder’s full path along with double quotes around the path, hold down the Shift key on your keyboard, right-click your folder, and choose "Copy as Path."

robocopy "Folder1" "Folder2" /L /NJH /NJS /NP /NS

![The 'robocopy' command typed in Command Prompt.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/4-compare-folders-command-prompt.jpg) 

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4708689&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.epubor.com/images/uppic/audible-converter-interface.png" border="0">Epubor Audible Converter for Win： Download and convert Audible AAXC/AA/AAX to MP3 with 100% original quality preserved.</a>
<!-- affiliate ads end -->
 You’ll see the differences between your folders.

 If you’re curious as to what the robocopy command does, here’s an explanation of each flag we used with the command:

* **L**: This tells the command not to copy files but show the log of the files in the specified folder.
* **NJH**: This flag excludes junctions, hard links, and reparse points from consideration. This way, the command focuses on the regular files in the specified folders.
* **NJS**: This flag excludes symbolic links from the process.
* **NP**: This flag excludes folder timestamps.
* **NS**: This flag excludes file security information.

##  Compare Folders With WinMerge

 If you want more details about the differences in your folders, Windows doesn't have a built-in tool to help you with that. However, you can use a free third-party app called WinMerge to compare multiple folders.

 To use it, launch a web browser on your PC, head to the [WinMerge](https://winmerge.org/downloads/?lang=en) site, and download and install the app. Make sure to download the app’s executable and not the ZIP version.

 Open the WinMerge app, then select File > Open in the Menu Bar or press Ctrl+O.

![File > Open highlighted in WinMerge.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/5-open-folder-winmerge.jpg) 

 For the "1st File or Folder" field, select "Browse" and choose the first folder to compare.

!['Browse' highlighted for the '1st File or Folder' field in WinMerge.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/6-add-first-folder-winmerge.jpg) 

<!-- affiliate ads begin -->
<a href="https://shop.incomedia.eu/order/checkout.php?PRODS=39655089&QTY=1&AFFILIATE=108875&CART=1"><img src="https://incomedia.eu/files/images/affiliates/wa/01_WA_728x90.jpg" border="0"></a>
<!-- affiliate ads end -->
 For the "2nd File or Folder" field, click the "Browse" button and choose the second folder to compare.

!['Browse' highlighted for the '2nd File or Folder' field in WinMerge.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/7-add-second-folder-winmerge.jpg) 

<!-- affiliate ads begin -->
<a href="https://store.movavi.com/affiliate.php?ACCOUNT=MOVAVI&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.movavi.com%3FAFFILIATE%3D108875%26RESOURCE%3DMovavi%2BVideo%2BEditor%2Bbox"><img src="https://mcusercontent.com/0885a03ded3d480dca9287f12/images/6d3207fd-9f15-4c21-f0ad-59c68e6a7e2a.png" border="0"></a>
<!-- affiliate ads end -->
 In both fields, enable the "Read-Only" option. Click the "Folder: Filter" field and type **\*.\*** if it isn’t already there. This ensures the app compares all the files in both the specified folders. Then, at the bottom, click "Compare."

![Various comparison options highlighted in WinMerge.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/8-configure-comparison-options-winmerge.jpg) 

 On the following screen, you’ll see the comparison of the specified folders. You’ll see information like identical files in both folders, files missing from one folder, and so on.

![The comparison of two folders in WinMerge.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/9-folder-comparison-winmerge.jpg) 

<!-- affiliate ads begin -->
<a href="https://shop.mondly.com/affiliate.php?ACCOUNT=ATISTUDI&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.mondly.com%3FAFFILIATE%3D108875%26RESOURCE%3D%2BGeneral%2B970x90%2B"><img src="https://secure.avangate.com/images/merchant/69c418c33ec2e1a4267fa9bb77fa1428/general-970x90.gif" border="0"></a>
<!-- affiliate ads end -->
 And that's how you know what one folder has that another doesn't. This can be really useful if you're trying to quickly compare different versions of the same folder, like you'd have when you[create a backup](https://activate-lock.techidaily.com/in-2024-how-to-bypass-icloud-by-checkra1n-even-on-iphone-14-pro-max-if-youve-tried-everything-by-drfone-ios/).

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
<li><a href="https://some-techniques.techidaily.com/new-filmeditingsuite-assessment-detailed-insights/"><u>[New] FilmEditingSuite Assessment – Detailed Insights</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-from-camera-clicks-to-youtube-clips-an-experts-step-by-step-visual-instruction-manual/"><u>[New] From Camera Clicks to YouTube Clips  An Expert's Step-by-Step Visual Instruction Manual</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-from-fuzzy-frames-to-sharpness-the-v22-journey/"><u>[New] From Fuzzy Frames to Sharpness - The V2.2 Journey</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-game-masters-unleashed-an-in-depth-look-at-kinemaster-on-android/"><u>[New] Game Masters Unleashed  An In-Depth Look at KineMaster on Android</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-guide-to-top-frame-rates-in-slow-motion-video-production/"><u>[New] Guide to Top Frame Rates in Slow-Motion Video Production</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/new-how-to-maximize-ios-podcast-features/"><u>[New] How to Maximize iOS Podcast Features</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-ideal-starter-accessories-for-gopro-newbies/"><u>[New] Ideal Starter Accessories for GoPro Newbies</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-immersive-exploration-mastering-close-up-views-in-minecraft/"><u>[New] Immersive Exploration  Mastering Close-Up Views in Minecraft</u></a></li>
<li><a href="https://on-screen-recording.techidaily.com/updated-2024-approved-full-spectrum-analysis-macos-and-screenflow-v4/"><u>[Updated] 2024 Approved  Full Spectrum Analysis  MacOS and ScreenFlow V4</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-foremost-12-gps-enabled-cctv-cameras-for-motion-recording/"><u>[Updated] Foremost 12 GPS-Enabled CCTV Cameras for Motion Recording</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-guide-to-accessing-price-null-picture-content/"><u>[Updated] Guide to Accessing Price-Null Picture Content</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-humorhub-join-the-fun-filled-world/"><u>[Updated] HumorHub  Join the Fun-Filled World</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-innovate-funny-graphics-share-on-giphy-platform/"><u>[Updated] Innovate Funny Graphics, Share on Giphy Platform</u></a></li>
<li><a href="https://fox-boxes.techidaily.com/updated-the-prime-camera-choices-revealing-the-best/"><u>[Updated] The Prime Camera Choices – Revealing the Best</u></a></li>
<li><a href="https://media-tips.techidaily.com/demand-youtube-to-separate-youtube-music-from-youtube-premium-services-now/"><u>Demand YouTube To Separate YouTube Music From YouTube Premium Services Now!</u></a></li>
<li><a href="https://bypass-frp.techidaily.com/easy-guide-how-to-bypass-realme-11-proplus-frp-android-10111213-by-drfone-android/"><u>Easy Guide How To Bypass Realme 11 Pro+ FRP Android 10/11/12/13</u></a></li>
<li><a href="https://techidaily.com/full-guide-to-hard-reset-your-honor-90-lite-drfone-by-drfone-reset-android-reset-android/"><u>Full Guide to Hard Reset Your Honor 90 Lite | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/get-to-know-the-pros-of-engaging-with-asmr-for-2024/"><u>Get to Know the Pros of Engaging with ASMR for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/harnessing-lut-power-for-free-high-quality-colorization-for-2024/"><u>Harnessing LUT Power for Free, High-Quality Colorization for 2024</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/hdr-horizon-highlights-selective-online-skies-compilation-for-2024/"><u>HDR Horizon Highlights  Selective Online Skies Compilation for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/hdr-rating-does-aurora-deliver-quality-in-2024/"><u>HDR Rating  Does Aurora Deliver Quality, In 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/how-much-video-can-64gb128gb-hold-in-2024/"><u>How Much Video Can 64GB/128GB Hold, In 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/illuminating-images-in-lightroom-a-step-by-step-hdr-guide-for-2024/"><u>Illuminating Images in Lightroom  A Step-by-Step HDR Guide for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-exceptional-environments-the-best-screen-snapshots/"><u>In 2024, Exceptional Environments  The Best Screen Snapshots</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-expert-editions-selecting-high-quality-blu-ray-players-freepaid/"><u>In 2024, Expert Editions  Selecting High-Quality Blu-Ray Players (Free/Paid)</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-from-idea-to-implementation-crafting-a-powerful-documntary-narrative/"><u>In 2024, From Idea to Implementation  Crafting a Powerful Documntary Narrative</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-full-dissection-gopro-silver-hero4-model-insight/"><u>In 2024, Full Dissection  GoPro Silver Hero4 Model Insight</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-game-centric-tvs-top-picks-for-ps5xbox-series-x/"><u>In 2024, Game-Centric TVs  Top Picks for PS5/Xbox Series X</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-illuminating-images-in-lightroom-a-step-by-step-hdr-guide/"><u>In 2024, Illuminating Images in Lightroom  A Step-by-Step HDR Guide</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-image-illumination-choose-best-websites-with-photo-framing-features/"><u>In 2024, Image Illumination  Choose Best Websites with Photo Framing Features</u></a></li>
<li><a href="https://change-location.techidaily.com/in-2024-the-best-ispoofer-alternative-to-try-on-samsung-galaxy-m14-4g-drfone-by-drfone-virtual-android/"><u>In 2024, The Best iSpoofer Alternative to Try On Samsung Galaxy M14 4G | Dr.fone</u></a></li>
<li><a href="https://sound-optimizing.techidaily.com/in-2024-windows-10-sound-sensation-a-step-by-step-audio-capture-tutorial/"><u>In 2024, Windows 10 Sound Sensation A Step-by-Step Audio Capture Tutorial</u></a></li>
<li><a href="https://techidaily.com/is-your-honor-100-pro-working-too-slow-heres-how-you-can-hard-reset-it-drfone-by-drfone-reset-android-reset-android/"><u>Is your Honor 100 Pro working too slow? Heres how you can hard reset it | Dr.fone</u></a></li>
<li><a href="https://fake-location.techidaily.com/spoofing-life360-how-to-do-it-on-oppo-reno-11-5g-drfone-by-drfone-virtual-android/"><u>Spoofing Life360 How to Do it on Oppo Reno 11 5G? | Dr.fone</u></a></li>
<li><a href="https://techtrends.techidaily.com/step-by-step-walkthrough-on-utilizing-copilot-with-microsoft-teams/"><u>Step-by-Step Walkthrough on Utilizing Copilot with Microsoft Teams</u></a></li>
<li><a href="https://tech-recovery.techidaily.com/the-best-picture-messaging-software-choices/"><u>The Best Picture Messaging Software Choices</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/the-ultimate-guide-to-get-the-rare-candy-on-pokemon-go-fire-red-on-oneplus-nord-ce-3-5g-drfone-by-drfone-virtual-android/"><u>The Ultimate Guide to Get the Rare Candy on Pokemon Go Fire Red On OnePlus Nord CE 3 5G | Dr.fone</u></a></li>
</ul></div>
