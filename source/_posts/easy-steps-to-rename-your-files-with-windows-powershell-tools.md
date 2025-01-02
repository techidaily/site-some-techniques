---
title: Easy Steps to Rename Your Files with Windows PowerShell Tools
date: 2024-12-25T17:15:10.033Z
updated: 2025-01-01T16:27:26.555Z
tags:
  - deals
categories:
  - tech
thumbnail: https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/10/52880885757_aff84061b0_o-1.jpg
---

## Easy Steps to Rename Your Files with Windows PowerShell Tools

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/qbuund2HKOQ?si=NaGHqIrx8hSL7gWV" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

### Quick Links

* [Before You Begin: Learn How to Find a File or Folder’s Full Path](https://video-capture.techidaily.com/new-top-5-xbox-external-hard-drive-you-can-find/)
* [How to Rename a Specific File](https://visual-screen-recording.techidaily.com/updated-vidmas-technology-in-screen-capturing-spotlighted/)
* [How to Rename Files in a Folder With an Increasing Number](https://bypass-frp.techidaily.com/easy-guide-how-to-bypass-xiaomi-redmi-note-12-proplus-5g-frp-android-10111213-by-drfone-android/)
* [How to Add a Prefix or Suffix to a File Name](https://facebook-video-share.techidaily.com/updated-2024-approved-achieving-excellent-illumination-on-youtube-videos/)
* [How to Add Timestamps to All Files in a Folder](https://extra-guidance.techidaily.com/srt-simplified-core-concepts-made-clear-for-2024/)

 PowerShell makes renaming files from the command line super easy. You can use specific names, add increasing numbers, add prefixes and suffixes, and even append timestamps. We’ll show you how to do that all on your Windows 11 or Windows 10 computer.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/zWYVKFk3yPQ?si=Yu7xsjIYgRiq8zHk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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
<iframe width="560" height="315" src="https://www.youtube.com/embed/j5gTm5KxtQ0?si=onF1rBS2nEM5nLGg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 PowerShell won’t display a message confirming your file is renamed, but know that the job is done.

##  How to Rename Files in a Folder With an Increasing Number

 If you want to add an increasing number, such as 1, 2, 3, and so on, to your files in a specific folder, follow these steps.

 Launch a PowerShell window and type the following command. Replace **PATH** with the full path to your folder, and **txt** with the format of the files to rename. Then, press Enter.

Get-ChildItem PATH -Recurse -Include "*.txt" | ForEach-Object -Begin { $Counter = 1 } -Process { Rename-Item $_.FullName -NewName ("{0}_{1}" -f $Counter, $_.Name) ; $Counter++ }

![Files with an increasing number in File Explorer.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/3-add-numbers-to-file-names.jpg) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/HtM7d4dpN1I?si=2vN_xgVGD4eYGORu" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/SyMZxS9479s?si=0T6zZpyN2LBftFTM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://youtube-docs.techidaily.com/024-approved-turn-your-screen-time-into-money-with-these-tips/"><u>[New] 2024 Approved Turn Your Screen Time Into Money With These Tips</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-fundamentals-of-visual-communication-through-motion/"><u>[New] Fundamentals of Visual Communication Through Motion</u></a></li>
<li><a href="https://youtube-blog.techidaily.com/n-2024-unveiling-the-secrets-to-producing-popular-youtube-shorts/"><u>[New] In 2024, Unveiling the Secrets to Producing Popular YouTube Shorts</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-free-srt-conversion-uncover-top-8-online-options/"><u>[Updated] Free SRT Conversion Uncover Top 8 Online Options</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-graphic-animation-basic-knowledge-and-practices/"><u>[Updated] Graphic Animation Basic Knowledge & Practices</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-gratitude-freepaid-video-outro-template-gallery/"><u>[Updated] Gratitude Free/Paid Video Outro Template Gallery</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-foundational-approach-to-gradual-volume-adjustment/"><u>2024 Approved Foundational Approach to Gradual Volume Adjustment</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-how-to-safely-obtain-vlc-player-at-no-charge-on-macos/"><u>2024 Approved How to Safely Obtain VLC Player at No Charge on MacOS</u></a></li>
<li><a href="https://tech-recovery.techidaily.com/delving-into-meta-ai-unveiling-the-power-behind-advanced-algorithms/"><u>Delving Into Meta AI: Unveiling the Power Behind Advanced Algorithms</u></a></li>
<li><a href="https://mondly-stories.techidaily.com/embrace-language-diversity-6-advantages-of-learning-arabic-via-mondly-online/"><u>Embrace Language Diversity: 6 Advantages of Learning Arabic via Mondly Online</u></a></li>
<li><a href="https://win-workspace.techidaily.com/essential-usb-c-gadgets-for-both-macos-and-windows-compatible-with-8k-displays-recommended-by-zdnet/"><u>Essential USB-C Gadgets for Both macOS & Windows: Compatible with 8K Displays, Recommended by ZDNet</u></a></li>
<li><a href="https://some-techniques.techidaily.com/fine-tuning-the-art-of-recording-in-audacity-for-2024/"><u>Fine-Tuning the Art of Recording in Audacity for 2024</u></a></li>
<li><a href="https://win-tutorials.techidaily.com/free-download-winning-mixes-of-making-beats-count-dj-competition-compilation-available-now/"><u>Free Download: Winning Mixes of 'Making Beats Count' DJ Competition - Compilation Available Now!</u></a></li>
<li><a href="https://ai-vdieo-software.techidaily.com/new-best-ways-to-convert-mp4-videos-to-mp3-audio-files/"><u>New Best Ways to Convert MP4 Videos to MP3 Audio Files</u></a></li>
<li><a href="https://sound-issues.techidaily.com/solving-windows-11-audio-problems-a-comprehensive-fix/"><u>Solving Windows 11 Audio Problems: A Comprehensive Fix</u></a></li>
<li><a href="https://buynow-reviews.techidaily.com/top-ranking-ergonomic-vertical-keyboards/"><u>Top-Ranking Ergonomic Vertical Keyboards</u></a></li>
</ul></div>

