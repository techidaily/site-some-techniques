---
title: "Mastering File Renaming: A Comprehensive Guide Using PowerShell"
date: 2024-10-04T17:40:43.257Z
updated: 2024-10-11T16:20:29.617Z
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
<a href="https://aligracehair.sjv.io/c/5597632/1885932/19272" target="_top" id="1885932">
  <img src="//a.impactradius-go.com/display-ad/19272-1885932" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1885932/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 That action has copied your selected item’s full path to your clipboard. You can now [paste this path](https://twitter-videos.techidaily.com/new-in-2024-gain-twitter-gifs-for-pc-download-made-simple/) wherever required in the commands below.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2144272/7443" target="_top" id="2144272">
  <img src="//a.impactradius-go.com/display-ad/7443-2144272" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2144272/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  How to Rename a Specific File

 To give a new name to a specific file on your PC, use PowerShell’s Rename-Item [cmdlet](https://extra-guidance.techidaily.com/new-prophotomaster-the-ai-enhanced-editing-edge/). This cmdlet takes your file’s full path, the new name you want to assign, and renames your file.

 To use it, launch a PowerShell window on your PC and type the following command. In the command, replace **PATH** with the full path to your file. Your path should have the file’s full name as well as the extension. Replace **MyName** with the new name you want to use, and **ext** with your file’s original extension.

Rename-Item PATH -NewName MyName.ext

 Make sure to use your file’s original extension when you rename the file. Using another extension can make your file unusable.

 As an example, to rename a file named Old-Test.txt located on your desktop to New-Test.txt, you’d use the following command:

Rename-Item "C:\Users\Username\Desktop\Old-Test.txt" -NewName “New-Test.txt”

!['Rename-Item' cmdlet in a PowerShell window.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/2-rename-file-with-powershell.jpg) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2135405/19272" target="_top" id="2135405">
  <img src="//a.impactradius-go.com/display-ad/19272-2135405" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135405/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 PowerShell won’t display a message confirming your file is renamed, but know that the job is done.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2037358/7443" target="_top" id="2037358">
  <img src="//a.impactradius-go.com/display-ad/7443-2037358" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2037358/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  How to Rename Files in a Folder With an Increasing Number

 If you want to add an increasing number, such as 1, 2, 3, and so on, to your files in a specific folder, follow these steps.

 Launch a PowerShell window and type the following command. Replace **PATH** with the full path to your folder, and **txt** with the format of the files to rename. Then, press Enter.

Get-ChildItem PATH -Recurse -Include "*.txt" | ForEach-Object -Begin { $Counter = 1 } -Process { Rename-Item $_.FullName -NewName ("{0}_{1}" -f $Counter, $_.Name) ; $Counter++ }

![Files with an increasing number in File Explorer.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/3-add-numbers-to-file-names.jpg) 

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
<li><a href="https://some-techniques.techidaily.com/new-expert-guide-to-converting-xmlssattml-into-srt/"><u>[New] Expert Guide to Converting XML/SSA/TTML Into SRT</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-future-conversations-iphone-2024-recordings/"><u>[Updated] Future Conversations IPhone 2024 Recordings</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-flicker-studio-the-complete-lightroom-alternatives-guide/"><u>2024 Approved Flicker Studio The Complete Lightroom Alternatives Guide</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-from-basics-to-brilliance-fullscreen-proficiency-in-premiere/"><u>2024 Approved From Basics to Brilliance Fullscreen Proficiency in Premiere</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-ideal-tactic-fusing-gopro-footage-into-a-unified-360-video-experience/"><u>2024 Approved Ideal Tactic Fusing GoPro Footage Into a Unified 360 Video Experience</u></a></li>
<li><a href="https://article-posts.techidaily.com/cutting-edge-memes-top-ten-template-showcase/"><u>Cutting Edge Memes Top Ten Template Showcase</u></a></li>
<li><a href="https://some-techniques.techidaily.com/firefox-x-pie-mode-decoded-for-everyday-users-for-2024/"><u>Firefox X-Pie Mode Decoded for Everyday Users for 2024</u></a></li>
<li><a href="https://youtube-videos.techidaily.com/in-2024-channel-mastery-leverage-customizable-description-templates-for-more-followers/"><u>In 2024, Channel Mastery Leverage Customizable Description Templates for More Followers</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-go-beyond-boundaries-with-panasonic-hx-a1-wearable-camera/"><u>In 2024, Go Beyond Boundaries with Panasonic HX-A1 Wearable Camera</u></a></li>
<li><a href="https://apple-account.techidaily.com/in-2024-how-to-remove-apple-id-from-iphone-14-plus-without-password-by-drfone-ios/"><u>In 2024, How to Remove Apple ID from iPhone 14 Plus without Password?</u></a></li>
<li><a href="https://smart-video-creator.techidaily.com/new-compress-mpeg2-videos-with-free-virtualdub-software/"><u>New Compress MPEG2 Videos with Free VirtualDub Software</u></a></li>
<li><a href="https://techtrends.techidaily.com/pixel-buds-pro-2-update-anticipated-launch-info-pricing-and-specs-dive-into-the-latest-buzz/"><u>Pixel Buds Pro 2 Update: Anticipated Launch Info, Pricing, and Specs – Dive Into the Latest Buzz!</u></a></li>
<li><a href="https://fox-that.techidaily.com/troubleshooting-iphone-screen-time-issues-with-unanticipated-websites-listed/"><u>Troubleshooting iPhone Screen Time Issues with Unanticipated Websites Listed</u></a></li>
<li><a href="https://fox-that.techidaily.com/unlock-the-solution-to-your-iphones-imessage-continuous-disconnection-woes/"><u>Unlock the Solution to Your iPhone's iMessage Continuous Disconnection Woes</u></a></li>
<li><a href="https://facebook.techidaily.com/unraveling-facebooks-latest-community-connections/"><u>Unraveling Facebook's Latest Community Connections</u></a></li>
</ul></div>

