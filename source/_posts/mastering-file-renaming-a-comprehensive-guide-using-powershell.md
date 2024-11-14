---
title: "Mastering File Renaming: A Comprehensive Guide Using PowerShell"
date: 2024-11-10T17:57:59.465Z
updated: 2024-11-13T16:37:10.924Z
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

<!-- affiliate ads begin -->
<span id="1977020">
					<video width="128" height="480" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1977020.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/22993-1977020">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1977020.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:80px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fhomestyler.sjv.io%2Fc%2F5597632%2F1977020%2F22993'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1977020/22993" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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
<a href="https://appsumo.8odi.net/c/5597632/2105874/7443" target="_top" id="2105874">
  <img src="//a.impactradius-go.com/display-ad/7443-2105874" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2105874/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 PowerShell won’t display a message confirming your file is renamed, but know that the job is done.

<!-- affiliate ads begin -->
<span id="1983471">
					<video width="576" height="240" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1983471.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/22993-1983471">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1983471.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:360px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fhomestyler.sjv.io%2Fc%2F5597632%2F1983471%2F22993'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1983471/22993" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  How to Rename Files in a Folder With an Increasing Number

 If you want to add an increasing number, such as 1, 2, 3, and so on, to your files in a specific folder, follow these steps.

 Launch a PowerShell window and type the following command. Replace **PATH** with the full path to your folder, and **txt** with the format of the files to rename. Then, press Enter.

Get-ChildItem PATH -Recurse -Include "*.txt" | ForEach-Object -Begin { $Counter = 1 } -Process { Rename-Item $_.FullName -NewName ("{0}_{1}" -f $Counter, $_.Name) ; $Counter++ }

![Files with an increasing number in File Explorer.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/3-add-numbers-to-file-names.jpg) 

<!-- affiliate ads begin -->
<span id="1977023">
					<video width="128" height="480" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1977023.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/22993-1977023">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1977023.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:80px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fhomestyler.sjv.io%2Fc%2F5597632%2F1977023%2F22993'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1977023/22993" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  How to Add a Prefix or Suffix to a File Name

 To add text before your file name (known as a prefix), launch a PowerShell window and enter the following command. Replace **PATH** with your folder's full path, and **PREFIX** with the text you want to append, then press Enter.

Get-ChildItem PATH | Rename-Item -NewName {"PREFIX" + $_.Name}

 To add text after your file’s name (called a suffix), use the following command, replacing **PATH** with the full path to your folder, and **SUFFIX** with the text to append. Then, press Enter.

Get-ChildItem PATH | Rename-Item -NewName {$_.BaseName + "SUFFIX" + $_.Extension}

##  How to Add Timestamps to All Files in a Folder

 If you want to add a timestamp to all the files in a folder, open PowerShell and type the following command. Replace **PATH** with the full path to your folder, and press Enter.

Get-ChildItem PATH -Recurse -Include "*.*" | ForEach-Object { Rename-Item -Path $_.FullName -NewName "$($_.DirectoryName)\$($_.BaseName)_$(Get-Date -F yyyy-MM-dd_HH-mm)$($_.Extension)"}

![Files with timestamp in File Explorer.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/4-add-timestamp-to-file-names.jpg) 

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
<li><a href="https://visual-screen-recording.techidaily.com/new-2024-approved-a-comprehensive-guide-to-laptop-screen-recording-techniques/"><u>[New] 2024 Approved A Comprehensive Guide to Laptop Screen Recording Techniques</u></a></li>
<li><a href="https://screen-capture.techidaily.com/new-advice-on-reversing-non-functional-obs-fullscreen/"><u>[New] Advice on Reversing Non-Functional OBS Fullscreen</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-excellence-in-detail-a-curated-list-of-8k-cameras/"><u>[New] Excellence in Detail A Curated List of 8K Cameras</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-experiences-with-the-syma-x8c-drone/"><u>[New] Experiences with the Syma X8C Drone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-hdr-mastery-the-complete-sdr-to-hdr-transformation/"><u>[New] HDR Mastery The Complete SDR-to-HDR Transformation</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/new-in-2024-pixelgrabber-evaluation-with-vendors-offerings/"><u>[New] In 2024, PixelGrabber Evaluation with Vendors' Offerings</u></a></li>
<li><a href="https://extra-skills.techidaily.com/2024-approved-nikon-1j5-takes-video-to-the-next-level-with-its-4k-features/"><u>2024 Approved Nikon 1J5 Takes Video to the Next Level with Its 4K Features</u></a></li>
<li><a href="https://iphone-unlock.techidaily.com/how-to-change-country-on-app-store-for-iphone-7-plus-with-7-methods-drfone-by-drfone-ios/"><u>How To Change Country on App Store for iPhone 7 Plus With 7 Methods | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/ideal-plot-crafting-platform-for-2024/"><u>Ideal Plot Crafting Platform for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/immerse-slides-with-audio-harmony-for-2024/"><u>Immerse Slides with Audio Harmony for 2024</u></a></li>
<li><a href="https://article-tips.techidaily.com/in-2024-cutting-edge-free-livestream-platforms-and-programs-reviewed-here/"><u>In 2024, Cutting-Edge Free Livestream Platforms and Programs Reviewed Here</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-explore-the-cheapest-deals-on-top-tier-gopros/"><u>In 2024, Explore the Cheapest Deals on Top-Tier GoPros</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/movaviopusflac/"><u>Movaviで簡単フリーOPUSからFLACへの変換 - 無料!</u></a></li>
<li><a href="https://review-topics.techidaily.com/possible-solutions-to-restore-deleted-photos-from-xiaomi-mix-fold-3-by-fonelab-android-recover-photos/"><u>Possible solutions to restore deleted photos from Xiaomi Mix Fold 3.</u></a></li>
<li><a href="https://sound-issues.techidaily.com/repair-techniques-for-defective-primary-audio-connector-a-comprehensive-guide/"><u>Repair Techniques for Defective Primary Audio Connector: A Comprehensive Guide</u></a></li>
</ul></div>

