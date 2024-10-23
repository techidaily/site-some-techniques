---
title: "Mastering File Renaming: A Comprehensive Guide Using PowerShell"
date: 2024-10-19T17:31:01.037Z
updated: 2024-10-23T17:10:44.811Z
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

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2118319/7443" target="_top" id="2118319">
  <img src="//a.impactradius-go.com/display-ad/7443-2118319" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2118319/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Before You Begin: Learn How to Find a File or Folder’s Full Path

 To rename files, you’ll have to provide PowerShell with your file or parent folder’s full path. If you know how to do this, skip to the relevant section below. If you aren’t quite sure [how to get a folder or file’s full path](https://fox-links.techidaily.com/updated-2024-approved-unparalleled-screenplay-craftsmanship-across-varied-fields/), we’ll show you.

[Open a File Explorer window](https://pokemon-go-android.techidaily.com/how-to-get-and-use-pokemon-go-promo-codes-on-realme-c67-4g-drfone-by-drfone-virtual-android/) and find your file or folder. Press and hold down the Shift key on your keyboard, right-click your file or folder, and choose "Copy as Path."

!['Copy as Path' highlighted in Windows 11's context menu.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/1-copy-file-path-windows.jpg) 

 That action has copied your selected item’s full path to your clipboard. You can now [paste this path](https://twitter-videos.techidaily.com/new-in-2024-gain-twitter-gifs-for-pc-download-made-simple/) wherever required in the commands below.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2043597/7443" target="_top" id="2043597">
  <img src="//a.impactradius-go.com/display-ad/7443-2043597" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2043597/7443" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://appsumo.8odi.net/c/5597632/2137413/7443" target="_top" id="2137413">
  <img src="//a.impactradius-go.com/display-ad/7443-2137413" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2137413/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  How to Rename Files in a Folder With an Increasing Number

 If you want to add an increasing number, such as 1, 2, 3, and so on, to your files in a specific folder, follow these steps.

 Launch a PowerShell window and type the following command. Replace **PATH** with the full path to your folder, and **txt** with the format of the files to rename. Then, press Enter.

Get-ChildItem PATH -Recurse -Include "*.txt" | ForEach-Object -Begin { $Counter = 1 } -Process { Rename-Item $_.FullName -NewName ("{0}_{1}" -f $Counter, $_.Name) ; $Counter++ }

![Files with an increasing number in File Explorer.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/3-add-numbers-to-file-names.jpg) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2100538/7443" target="_top" id="2100538">
  <img src="//a.impactradius-go.com/display-ad/7443-2100538" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2100538/7443" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://some-techniques.techidaily.com/new-explore-the-potential-of-color-grading-through-luts-and-ar/"><u>[New] Explore the Potential of Color Grading Through LUTs and AR</u></a></li>
<li><a href="https://article-helps.techidaily.com/updated-2024-approved-playtime-registration-and-logout-tutorials/"><u>[Updated] 2024 Approved Playtime Registration & Logout Tutorials</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-ideal-high-res-displays-the-best-5-for-ps5/"><u>[Updated] Ideal High-Res Displays The Best 5 For PS5</u></a></li>
<li><a href="https://some-skills.techidaily.com/updated-unlock-high-res-video-leading-4k-conversion-tools/"><u>[Updated] Unlock High-Res Video Leading 4K Conversion Tools</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-ideal-online-places-to-raise-audience-numbers/"><u>2024 Approved Ideal Online Places to Raise Audience Numbers</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/1726029585915-pc/"><u>画面録画データ量の最適化:PC/スマホ向け圧縮方法</u></a></li>
<li><a href="https://some-techniques.techidaily.com/exclusive-analysis-full-potential-of-bublcams-360-degree-scope-for-2024/"><u>Exclusive Analysis Full Potential of Bublcam's 360-Degree Scope for 2024</u></a></li>
<li><a href="https://extra-resources.techidaily.com/expert-tips-for-procuring-unlocked-picture-frame-videos/"><u>Expert Tips for Procuring Unlocked Picture Frame Videos</u></a></li>
<li><a href="https://some-techniques.techidaily.com/free-online-jpggif-converters-the-best-10-list-for-2024/"><u>Free Online JPG/GIF Converters The Best 10 List for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-explore-the-best-8-web-sites-for-accessing-3d-text-psds/"><u>In 2024, Explore the Best 8 Web Sites for Accessing 3D Text PSDs</u></a></li>
<li><a href="https://extra-skills.techidaily.com/in-2024-simplified-steps-for-photo-motion-blur-in-photoshop/"><u>In 2024, Simplified Steps for Photo Motion Blur in Photoshop</u></a></li>
<li><a href="https://data-safeguard.techidaily.com/mastering-photo-recovery-with-stellars-all-in-one-tool-for-both-pc-and-mac-users/"><u>Mastering Photo Recovery with Stellar's All-in-One Tool for Both PC & Mac Users</u></a></li>
<li><a href="https://tech-revival.techidaily.com/reimagined-automation-top-non-chatgpt-solutions-for-developers/"><u>Reimagined Automation: Top Non-ChatGPT Solutions for Developers</u></a></li>
<li><a href="https://buynow-reviews.techidaily.com/review-of-the-antop-at-127-a-stylish-antenna-bringing-you-free-clear-tv-signals/"><u>Review of the Antop AT-127: A Stylish Antenna Bringing You Free, Clear TV Signals</u></a></li>
<li><a href="https://some-guidance.techidaily.com/step-by-step-guide-successfully-exiting-safe-mode-in-windows-11/"><u>Step-by-Step Guide: Successfully Exiting Safe Mode in Windows 11</u></a></li>
</ul></div>

