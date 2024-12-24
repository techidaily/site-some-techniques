---
title: Easy Steps to Rename Your Files with Windows PowerShell Tools
date: 2024-12-21T20:40:13.115Z
updated: 2024-12-24T18:23:09.096Z
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

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/OZQJUTr44rA?si=ADA0nD1VnXjR_sH0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Before You Begin: Learn How to Find a File or Folder’s Full Path

 To rename files, you’ll have to provide PowerShell with your file or parent folder’s full path. If you know how to do this, skip to the relevant section below. If you aren’t quite sure [how to get a folder or file’s full path](https://fox-links.techidaily.com/updated-2024-approved-unparalleled-screenplay-craftsmanship-across-varied-fields/), we’ll show you.

[Open a File Explorer window](https://pokemon-go-android.techidaily.com/how-to-get-and-use-pokemon-go-promo-codes-on-realme-c67-4g-drfone-by-drfone-virtual-android/) and find your file or folder. Press and hold down the Shift key on your keyboard, right-click your file or folder, and choose "Copy as Path."

!['Copy as Path' highlighted in Windows 11's context menu.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/1-copy-file-path-windows.jpg) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/fo4lNZ84x9Q?si=WdcYPZp-9VJnZEnC" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 That action has copied your selected item’s full path to your clipboard. You can now [paste this path](https://twitter-videos.techidaily.com/new-in-2024-gain-twitter-gifs-for-pc-download-made-simple/) wherever required in the commands below.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/l4R7_qNIQvY?si=2zJOPfEcm6_3udzn" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/XS1nQCe95LU?si=A2dhdFkSAI61_nKA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/iOVkXoUxLf4?si=QfC18T2cb5OkiaXo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://some-techniques.techidaily.com/updated-foundational-methods-to-improve-color-balance/"><u>[Updated] Foundational Methods to Improve Color Balance</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-guard-your-gallery-with-gratis-cloud-and-paid-storage-tiers/"><u>[Updated] Guard Your Gallery with Gratis Cloud & Paid Storage Tiers</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/updated-in-2024-enhance-your-content-creation-with-these-top-12-cameras/"><u>[Updated] In 2024, Enhance Your Content Creation with These Top 12 Cameras</u></a></li>
<li><a href="https://screen-capture.techidaily.com/updated-in-2024-exciting-ios-applications-for-playing-psp-titles-1-5/"><u>[Updated] In 2024, Exciting iOS Applications for Playing PSP Titles #1-5</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/updated-pulse-picking-playlists-hot-tracks-for-viral-youtube-shorts/"><u>[Updated] Pulse-Picking Playlists Hot Tracks for Viral YouTube Shorts</u></a></li>
<li><a href="https://some-techniques.techidaily.com/experience-next-gen-notetaking-with-mematic-for-2024/"><u>Experience Next-Gen Notetaking with Mematic for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/getting-started-with-digital-image-detailing-for-2024/"><u>Getting Started with Digital Image Detailing for 2024</u></a></li>
<li><a href="https://fox-links.techidaily.com/halovision-highlights-critique-for-2024/"><u>HaloVision Highlights Critique for 2024</u></a></li>
<li><a href="https://ios-pokemon-go.techidaily.com/heres-everything-you-should-know-about-pokemon-stops-in-detail-on-apple-iphone-12-pro-drfone-by-drfone-virtual-ios/"><u>Heres Everything You Should Know About Pokemon Stops in Detail On Apple iPhone 12 Pro | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/high-fidelity-videos-our-selection-of-the-three-finest-phones-for-2024/"><u>High Fidelity Videos Our Selection of the Three Finest Phones for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/ignite-your-creative-journey-blending-photography-and-videos-through-pixiz-for-2024/"><u>Ignite Your Creative Journey Blending Photography & Videos Through Pixiz for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/illuminate-canon-cameras-combining-freebies-and-paid-lut-sets-for-2024/"><u>Illuminate Canon Cameras Combining Freebies and Paid LUT Sets for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-free-easy-online-downloader-for-your-pin-videos/"><u>In 2024, Free, Easy Online Downloader for Your Pin Videos</u></a></li>
<li><a href="https://android-unlock.techidaily.com/in-2024-top-apps-and-online-tools-to-track-vivo-v29-pro-phone-withwithout-imei-number-by-drfone-android/"><u>In 2024, Top Apps and Online Tools To Track Vivo V29 Pro Phone With/Without IMEI Number</u></a></li>
<li><a href="https://fox-glue.techidaily.com/innovative-browsing-strategies-with-picture-in-picture-mode/"><u>Innovative Browsing Strategies with Picture-In-Picture Mode</u></a></li>
<li><a href="https://win-amazing.techidaily.com/update-your-easycap-support-premium-driver-files-available-to-download/"><u>Update Your EasyCAP Support: Premium Driver Files Available to Download</u></a></li>
<li><a href="https://youtube-lab.techidaily.com/be-elites-creator-conclave/"><u>YouTube Elites Creator Conclave</u></a></li>
</ul></div>

