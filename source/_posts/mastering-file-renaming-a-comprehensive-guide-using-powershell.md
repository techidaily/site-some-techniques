---
title: "Mastering File Renaming: A Comprehensive Guide Using PowerShell"
date: 2024-10-03T01:29:32.544Z
updated: 2024-10-05T21:00:04.438Z
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
<a href="https://appsumo.8odi.net/c/5597632/2052060/7443" target="_top" id="2052060">
  <img src="//a.impactradius-go.com/display-ad/7443-2052060" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2052060/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Before You Begin: Learn How to Find a File or Folder’s Full Path

 To rename files, you’ll have to provide PowerShell with your file or parent folder’s full path. If you know how to do this, skip to the relevant section below. If you aren’t quite sure [how to get a folder or file’s full path](https://fox-links.techidaily.com/updated-2024-approved-unparalleled-screenplay-craftsmanship-across-varied-fields/), we’ll show you.

[Open a File Explorer window](https://pokemon-go-android.techidaily.com/how-to-get-and-use-pokemon-go-promo-codes-on-realme-c67-4g-drfone-by-drfone-virtual-android/) and find your file or folder. Press and hold down the Shift key on your keyboard, right-click your file or folder, and choose "Copy as Path."

!['Copy as Path' highlighted in Windows 11's context menu.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/1-copy-file-path-windows.jpg) 

<!-- affiliate ads begin -->
<a href="https://bluettius.sjv.io/c/5597632/2139122/17108" target="_top" id="2139122">
  <img src="//a.impactradius-go.com/display-ad/17108-2139122" border="0" alt="https://techidaily.com" width="468" height="60"/>
</a>
<img height="0" width="0" src="https://bluettius.sjv.io/i/5597632/2139122/17108" style="position:absolute;visibility:hidden;" border="0" />
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

 PowerShell won’t display a message confirming your file is renamed, but know that the job is done.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2135418/19272" target="_top" id="2135418">
  <img src="//a.impactradius-go.com/display-ad/19272-2135418" border="0" alt="https://techidaily.com" width="468" height="60"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135418/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  How to Rename Files in a Folder With an Increasing Number

 If you want to add an increasing number, such as 1, 2, 3, and so on, to your files in a specific folder, follow these steps.

 Launch a PowerShell window and type the following command. Replace **PATH** with the full path to your folder, and **txt** with the format of the files to rename. Then, press Enter.

Get-ChildItem PATH -Recurse -Include "*.txt" | ForEach-Object -Begin { $Counter = 1 } -Process { Rename-Item $_.FullName -NewName ("{0}_{1}" -f $Counter, $_.Name) ; $Counter++ }

![Files with an increasing number in File Explorer.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/3-add-numbers-to-file-names.jpg) 

<!-- affiliate ads begin -->
<a href="https://bluettius.sjv.io/c/5597632/2139115/17108" target="_top" id="2139115">
  <img src="//a.impactradius-go.com/display-ad/17108-2139115" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://bluettius.sjv.io/i/5597632/2139115/17108" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://some-techniques.techidaily.com/new-friendship-enhancing-virtual-worlds-the-top-10-metaverse-games/"><u>[New] Friendship-Enhancing Virtual Worlds The Top 10 Metaverse Games</u></a></li>
<li><a href="https://twitter-videos.techidaily.com/new-streamlined-social-media-prime-twitter-unfollow-tools-overview-for-2024/"><u>[New] Streamlined Social Media Prime Twitter Unfollow Tools Overview for 2024</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/new-ultimate-gamer-writes-top-7-fps-games-list-for-2024/"><u>[New] Ultimate Gamer' Writes Top 7 FPS Games List for 2024</u></a></li>
<li><a href="https://article-tips.techidaily.com/updated-2024-approved-deconstructing-trillers-distinct-identity-in-the-realm-of-social-media/"><u>[Updated] 2024 Approved Deconstructing Triller's Distinct Identity in the Realm of Social Media</u></a></li>
<li><a href="https://eaxpv-info.techidaily.com/updated-2024-approved-how-to-integrate-youtube-playlists-into-your-site/"><u>[Updated] 2024 Approved How to Integrate YouTube Playlists Into Your Site</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-exclusive-guide-the-intricate-process-of-media-import-in-w11/"><u>[Updated] Exclusive Guide The Intricate Process of Media Import in W11</u></a></li>
<li><a href="https://tiktok-videos.techidaily.com/updated-in-2024-laugh-literature-documenting-the-funniest-trends-on-tiktok/"><u>[Updated] In 2024, Laugh Literature Documenting the Funniest Trends on TikTok</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-how-to-make-a-photo-video-with-pixiz/"><u>2024 Approved How to Make a Photo Video with Pixiz?</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-ideal-choices-apps-that-convert-photos-to-films/"><u>2024 Approved Ideal Choices Apps That Convert Photos to Films</u></a></li>
<li><a href="https://fox-friendly.techidaily.com/2024-approved-the-art-of-capturing-kinetic-energy-in-iphone-images/"><u>2024 Approved The Art of Capturing Kinetic Energy in iPhone Images</u></a></li>
<li><a href="https://some-techniques.techidaily.com/exclusive-list-top-business-vault-for-2024/"><u>Exclusive List Top Business Vault for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/fix-for-freezing-photo-booth-videos-that-disrupt-usage-for-2024/"><u>Fix for Freezing Photo Booth Videos That Disrupt Usage for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-exquisite-background-melodies-for-edits/"><u>In 2024, Exquisite Background Melodies for Edits</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-free-individualized-music-for-engaging-video-conclusions/"><u>In 2024, Free, Individualized Music for Engaging Video Conclusions</u></a></li>
<li><a href="https://some-guidance.techidaily.com/movavi-m2p-mpeg/"><u>Movavi의 인내성 강화: 웹에서 무료 M2P MPEG 교리 전환 기술</u></a></li>
<li><a href="https://blog-min.techidaily.com/quick-and-simple-guide-3-methods-to-save-your-favorite-daily-motion-video-downloads/"><u>Quick and Simple Guide: 3 Methods to Save Your Favorite Daily Motion Video Downloads</u></a></li>
<li><a href="https://driver-download.techidaily.com/smooth-gameplay-awaits-tap-into-your-xbox-wireless-potential-today/"><u>Smooth Gameplay Awaits: Tap Into Your Xbox Wireless Potential Today</u></a></li>
</ul></div>

