---
title: "Mastering File Renaming: A Comprehensive Guide Using PowerShell"
date: 2025-02-17T18:25:41.188Z
updated: 2025-02-19T18:52:44.629Z
tags:
  - deals
categories:
  - tech
thumbnail: https://thmb.techidaily.com/2f5a7138163b464da142425b5cd4fc9ef8759bb9361cd872c71016b4ccd5a432.jpg
---

## Mastering File Renaming: A Comprehensive Guide Using PowerShell

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/zXUt81WsQpI?si=W3DKIAsa2-qbGadJ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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
<iframe width="560" height="315" src="https://www.youtube.com/embed/9Sj2QNA-JXI?si=V-_h73iE3VlE214k" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 PowerShell won’t display a message confirming your file is renamed, but know that the job is done.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/JAkb8Bv3AU4?si=2rHwnZYTzTLieKgY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  How to Rename Files in a Folder With an Increasing Number

 If you want to add an increasing number, such as 1, 2, 3, and so on, to your files in a specific folder, follow these steps.

 Launch a PowerShell window and type the following command. Replace **PATH** with the full path to your folder, and **txt** with the format of the files to rename. Then, press Enter.

Get-ChildItem PATH -Recurse -Include "*.txt" | ForEach-Object -Begin { $Counter = 1 } -Process { Rename-Item $_.FullName -NewName ("{0}_{1}" -f $Counter, $_.Name) ; $Counter++ }

![Files with an increasing number in File Explorer.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/3-add-numbers-to-file-names.jpg) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/Vca--yEhtdo?si=7ijqjyP-oi3LYze1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  How to Add a Prefix or Suffix to a File Name

 To add text before your file name (known as a prefix), launch a PowerShell window and enter the following command. Replace **PATH** with your folder's full path, and **PREFIX** with the text you want to append, then press Enter.

Get-ChildItem PATH | Rename-Item -NewName {"PREFIX" + $_.Name}

 To add text after your file’s name (called a suffix), use the following command, replacing **PATH** with the full path to your folder, and **SUFFIX** with the text to append. Then, press Enter.

Get-ChildItem PATH | Rename-Item -NewName {$_.BaseName + "SUFFIX" + $_.Extension}

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/it8VkxDUdAc?si=ef6VZWR7kW4P9ikh" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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
<li><a href="https://facebook-videos.techidaily.com/new-download-fb-links-8-free-online-tools/"><u>[New] Download FB Links 8 FREE, Online Tools</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-exclusive-review-prime-cars-surveillance-devices/"><u>[New] Exclusive Review Prime Cars Surveillance Devices</u></a></li>
<li><a href="https://fox-friendly.techidaily.com/new-in-2024-elevating-film-colors-using-luts-methods/"><u>[New] In 2024, Elevating Film Colors Using Luts Methods</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-in-depth-kinetics-evaluation-2023/"><u>[New] In-Depth Kinetics Evaluation 2023</u></a></li>
<li><a href="https://fox-helps.techidaily.com/new-leading-streaming-tools-for-online-video-games-for-2024/"><u>[New] Leading Streaming Tools for Online Video Games for 2024</u></a></li>
<li><a href="https://extra-support.techidaily.com/new-masterclass-in-timelapse-capture-via-gopro-studio/"><u>[New] Masterclass in Timelapse Capture via GoPro Studio</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-easy-guide-to-see-youtube-liked-comments/"><u>[Updated] Easy Guide to See YouTube Liked Comments</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-eye-catching-text-top-10-photo-writing-tools-for-smartphones/"><u>[Updated] Eye-Catching Text Top 10 Photo Writing Tools for Smartphones</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-film-flashes-top-snippets-for-skilled-editors/"><u>[Updated] Film Flashes Top Snippets for Skilled Editors</u></a></li>
<li><a href="https://fox-access.techidaily.com/updated-navigating-the-world-of-no-fee-visual-aids/"><u>[Updated] Navigating the World of No-Fee Visual Aids</u></a></li>
<li><a href="https://some-techniques.techidaily.com/expert-picks-for-superior-steadicams-in-aerial-cinema-for-2024/"><u>Expert Picks for Superior Steadicams in Aerial Cinema for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/from-iphone-images-jpeg-png-guided-conversion-to-pdfs-for-2024/"><u>From iPhone Images (JPEG, PNG) - Guided Conversion to PDFs for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/highlighting-heroics-at-the-x-olympics-2022-for-2024/"><u>Highlighting Heroics at the X-Olympics 2022 for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-framed-fantasies-expert-recommendations-on-software-and-sites/"><u>In 2024, Framed Fantasies Expert Recommendations on Software & Sites</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/in-2024-innovators-crafting-immersive-viewscape/"><u>In 2024, Innovators Crafting Immersive Viewscape</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/in-2024-os-bridging-virtualmix-pro/"><u>In 2024, OS-Bridging VirtualMix Pro</u></a></li>
<li><a href="https://driver-install.techidaily.com/swift-updates-to-optimize-your-gpus-nvidia-drivers/"><u>Swift Updates to Optimize Your GPU's Nvidia Drivers</u></a></li>
<li><a href="https://hardware-updates.techidaily.com/the-complete-guide-to-canon-eos-driver-updates-and-free-downloads/"><u>The Complete Guide to Canon EOS Driver Updates and Free Downloads</u></a></li>
<li><a href="https://techno-recovery.techidaily.com/what-to-do-when-you-encounter-a-missing-coredll-file/"><u>What to Do When You Encounter a Missing Core.dll File</u></a></li>
</ul></div>

