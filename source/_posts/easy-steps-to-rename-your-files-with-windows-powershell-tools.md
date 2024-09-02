---
title: Easy Steps to Rename Your Files with Windows PowerShell Tools
date: 2024-09-01T01:24:07.135Z
updated: 2024-09-02T01:24:07.135Z
tags:
  - deals
categories:
  - tech
thumbnail: https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/10/52880885757_aff84061b0_o-1.jpg
---

## Easy Steps to Rename Your Files with Windows PowerShell Tools

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

##  How to Rename a Specific File

 To give a new name to a specific file on your PC, use PowerShell’s Rename-Item [cmdlet](https://extra-guidance.techidaily.com/new-prophotomaster-the-ai-enhanced-editing-edge/). This cmdlet takes your file’s full path, the new name you want to assign, and renames your file.

 To use it, launch a PowerShell window on your PC and type the following command. In the command, replace **PATH** with the full path to your file. Your path should have the file’s full name as well as the extension. Replace **MyName** with the new name you want to use, and **ext** with your file’s original extension.

Rename-Item PATH -NewName MyName.ext

 Make sure to use your file’s original extension when you rename the file. Using another extension can make your file unusable.

 As an example, to rename a file named Old-Test.txt located on your desktop to New-Test.txt, you’d use the following command:

Rename-Item "C:\Users\Username\Desktop\Old-Test.txt" -NewName “New-Test.txt”

!['Rename-Item' cmdlet in a PowerShell window.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/2-rename-file-with-powershell.jpg) 

<!-- affiliate ads begin -->
<a href="https://store.nero.com/order/checkout.php?PRODS=39694080&QTY=1&AFFILIATE=108875&CART=1"><img src="http://cdnwww.nero.com/nero-com-wAssets/img/banners/2023/nbr/fire/Screenshot_1red_gb.jpg" border="0">Nero Burning ROM:
The ultimate burning program for all your needs!</a>
<!-- affiliate ads end -->
 PowerShell won’t display a message confirming your file is renamed, but know that the job is done.

<!-- affiliate ads begin -->
<a href="https://shop.systoolsgroup.com/affiliate.php?ACCOUNT=SYSTOOBY&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.systoolsgroup.com%3FAFFILIATE%3D108875%26RESOURCE%3DSysTools%2BOST%2BRecovery"><img src="https://www.systoolsgroup.com/box/ost-recovery.png" border="0"></a>
<!-- affiliate ads end -->
##  How to Rename Files in a Folder With an Increasing Number

 If you want to add an increasing number, such as 1, 2, 3, and so on, to your files in a specific folder, follow these steps.

 Launch a PowerShell window and type the following command. Replace **PATH** with the full path to your folder, and **txt** with the format of the files to rename. Then, press Enter.

Get-ChildItem PATH -Recurse -Include "*.txt" | ForEach-Object -Begin { $Counter = 1 } -Process { Rename-Item $_.FullName -NewName ("{0}_{1}" -f $Counter, $_.Name) ; $Counter++ }

![Files with an increasing number in File Explorer.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/3-add-numbers-to-file-names.jpg) 

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4572700&QTY=1&AFFILIATE=108875&CART=1"><img src="	https://www.tubedigger.com/wp-content/uploads/2020/08/tubedigger-software-new.png" border="0">TubeDigger - online video downloader from mostly any site</a>
<!-- affiliate ads end -->
<!-- affiliate ads begin -->
<a href="https://electronicx.pxf.io/c/5597632/1872456/14483" target="_top" id="1872456"><img src="//a.impactradius-go.com/display-ad/14483-1872456" border="0" alt="" width="500" height="375"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1872456/14483" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
##  How to Add a Prefix or Suffix to a File Name

 To add text before your file name (known as a prefix), launch a PowerShell window and enter the following command. Replace **PATH** with your folder's full path, and **PREFIX** with the text you want to append, then press Enter.

Get-ChildItem PATH | Rename-Item -NewName {"PREFIX" + $_.Name}

 To add text after your file’s name (called a suffix), use the following command, replacing **PATH** with the full path to your folder, and **SUFFIX** with the text to append. Then, press Enter.

Get-ChildItem PATH | Rename-Item -NewName {$_.BaseName + "SUFFIX" + $_.Extension}

<!-- affiliate ads begin -->
<a href="https://store.nero.com/order/checkout.php?PRODS=42296985&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/9cea886b9f44a3c2df1163730ab64994/products/copy_nero_burning_rom_cart.png" border="0">
</a>
<!-- affiliate ads end -->
##  How to Add Timestamps to All Files in a Folder

 If you want to add a timestamp to all the files in a folder, open PowerShell and type the following command. Replace **PATH** with the full path to your folder, and press Enter.

Get-ChildItem PATH -Recurse -Include "*.*" | ForEach-Object { Rename-Item -Path $_.FullName -NewName "$($_.DirectoryName)\$($_.BaseName)_$(Get-Date -F yyyy-MM-dd_HH-mm)$($_.Extension)"}

![Files with timestamp in File Explorer.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/4-add-timestamp-to-file-names.jpg) 

<!-- affiliate ads begin -->
<a href="https://otszone.ots7.com/order/checkout.php?PRODS=4713321&QTY=1&AFFILIATE=108875&CART=1"><img src="https://green.ots7.com/screenshots/OtsAV/OtsAVDJ1.90-300x188.jpg" border="0">OtsAV DJ Pro</a>
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
<li><a href="https://fox-glue.techidaily.com/new-bring-laughs-home-for-free-mememakers-way-for-2024/"><u>[New] Bring Laughs Home for FREE - MemeMaker's Way for 2024</u></a></li>
<li><a href="https://facebook-video-footage.techidaily.com/new-cutting-edge-top-8-free-online-video-tools-for-2024/"><u>[New] Cutting Edge  Top 8 Free Online Video Tools for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-immediate-gif-to-video-conversion-top-5-free-websites/"><u>[New] Immediate GIF-to-Video Conversion, Top 5 Free Websites</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-implementing-stunning-visual-effects-on-zoom-calls/"><u>[New] Implementing Stunning Visual Effects on Zoom Calls</u></a></li>
<li><a href="https://youtube-docs.techidaily.com/n-2024-the-ultimate-guide-to-free-online-youtube-mp3-converters/"><u>[New] In 2024, The Ultimate Guide to Free Online YouTube-MP3 Converters</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-incorporating-excellent-srt-into-your-mp4-projects-a-2024-guide/"><u>[New] Incorporating Excellent SRT Into Your MP4 Projects – A 2024 Guide</u></a></li>
<li><a href="https://vp-tips.techidaily.com/new-record-breaking-reddit-threads-ranked-1-10-for-2024/"><u>[New] Record-Breaking Reddit Threads Ranked 1-10 for 2024</u></a></li>
<li><a href="https://instagram-video-files.techidaily.com/updated-2024-approved-what-is-igtv-and-how-to-use-it-everything-you-need-to-know/"><u>[Updated] 2024 Approved  What Is IGTV and How to Use It  Everything You Need to Know</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-exploring-the-world-of-montage-image-magic/"><u>[Updated] Exploring the World of Montage Image Magic</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-from-meta-to-omni-a-new-age-digital-odyssey-guide/"><u>[Updated] From Meta to Omni  A New Age Digital Odyssey Guide</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-harmonious-hush-for-restfulness-top-asmr-picks/"><u>[Updated] Harmonious Hush for Restfulness  Top ASMR Picks</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-immersive-zooming-experience-with-microsoft-teams/"><u>[Updated] Immersive Zooming Experience with Microsoft Teams</u></a></li>
<li><a href="https://facebook-clips.techidaily.com/updated-innovation-in-social-media-redefining-the-role-of-facebook-stories/"><u>[Updated] Innovation in Social Media  Redefining the Role of Facebook Stories</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-innovative-approaches-to-podcast-summary-creation/"><u>[Updated] Innovative Approaches to Podcast Summary Creation</u></a></li>
<li><a href="https://extra-tips.techidaily.com/2024-approved-access-a-wide-range-of-content-via-12-streaming-apps/"><u>2024 Approved  Access a Wide Range of Content via 12 Streaming Apps</u></a></li>
<li><a href="https://extra-approaches.techidaily.com/2024-approved-navigate-new-walls-insiders-guide-to-wallpapers-in-win11/"><u>2024 Approved  Navigate New Walls  Insider's Guide to Wallpapers in Win11</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/2024-approved-step-beyond-boundaries-with-innovative-wins11-titles/"><u>2024 Approved  Step Beyond Boundaries with Innovative Wins11 Titles</u></a></li>
<li><a href="https://fox-info.techidaily.com/analyzing-best-days-for-highest-audience-retention/"><u>Analyzing Best Days for Highest Audience Retention</u></a></li>
<li><a href="https://some-techniques.techidaily.com/ideal-painting-and-design-tools-on-windows-no-cost-or-charge-for-2024/"><u>Ideal Painting & Design Tools on Windows  No Cost or Charge for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-exploring-interconnected-digital-universes-meta-and-omni/"><u>In 2024, Exploring Interconnected Digital Universes  Meta & Omni</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-exploring-the-metaverse-and-omniverse-distinctions/"><u>In 2024, Exploring the Metaverse and Omniverse Distinctions</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-exploring-the-world-of-book-trailers-with-top-5-picks/"><u>In 2024, Exploring the World of Book Trailers with Top 5 Picks</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-fast-and-easy-filming-techniques-the-best-5-hacks-unveiled/"><u>In 2024, Fast & Easy Filming Techniques – The Best 5 Hacks Unveiled</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-first-steps-to-faster-film-playback-in-snapchat/"><u>In 2024, First Steps to Faster Film Playback in Snapchat</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-flawlessimage-advanced-bg-eraser-app/"><u>In 2024, FlawlessImage  Advanced BG Eraser App</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-free-lut-strategies-for-enhancing-ar-experiences/"><u>In 2024, Free LUT Strategies for Enhancing AR Experiences</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-full-rotation-video-gear-for-social-media-broadcasts/"><u>In 2024, Full Rotation Video Gear for Social Media Broadcasts</u></a></li>
<li><a href="https://screen-video-capture.techidaily.com/in-2024-game-capture-software-analysis-obs-vs-shadowplay/"><u>In 2024, Game Capture Software Analysis  OBS vs ShadowPlay</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-gigglesome-footage-downloader/"><u>In 2024, Gigglesome Footage Downloader</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/in-2024-windows-11-gamers-guide-to-immaculate-game-recording/"><u>In 2024, Windows 11 Gamers' Guide to Immaculate Game Recording</u></a></li>
<li><a href="https://some-techniques.techidaily.com/initiating-your-adventure-in-av1-for-2024/"><u>Initiating Your Adventure in AV1 for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/innovative-guide-transforming-social-media-sounds-into-mobile-alerts-for-2024/"><u>Innovative Guide  Transforming Social Media Sounds Into Mobile Alerts for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/innovative-video-designs-free-premiere-plans-for-2024/"><u>Innovative Video Designs  Free Premiere Plans for 2024</u></a></li>
<li><a href="https://some-guidance.techidaily.com/the-ultimate-guide-to-flawless-sound-engineering-in-audacity-for-2024/"><u>The Ultimate Guide to Flawless Sound Engineering in Audacity for 2024</u></a></li>
</ul></div>
