---
title: Comparing Folders Across Windows 11 & 10 - A Comprehensive Guide
date: 2024-12-08T18:13:03.715Z
updated: 2024-12-09T20:09:55.232Z
tags:
  - deals
categories:
  - tech
thumbnail: https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/52846060984_17cb6c3aa6_o.jpg
---

## Comparing Folders Across Windows 11 & 10 - A Comprehensive Guide

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/T-ssCD10v2M?si=WVWGNayUiCAkMZzZ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

### Quick Links

* [Compare Folders From Properties](https://tech-recovery.techidaily.com/the-ultimate-fix-for-when-youtube-comments-wont-load/)
* [Compare Folders Using Command Prompt](https://video-capture.techidaily.com/new-in-2024-exacting-speech-recognition-via-googles-precision-tools/)
* [Compare Folders With WinMerge](https://win-howtos.techidaily.com/how-to-repair-when-your-macs-trackpad-wont-respond/)

### Key Takeaways

* One way to compare folders is to right-click your folders one at a time and choose "Properties" for each. Then compare the Properties window of each folder.
* The robocopy command is a command-line tool that can be used to view the differences between folder.
* Use WinMerge to compare the contents and details of folders if you want a graphical tool.

 Do you want to compare the number of files or folders or simply visualize the difference between two folders? If so, you have two graphical and one command line method to do that. We’ll show you how to perform the folder comparison task on your Windows 11 or Windows 10 PC.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/Iz2LYWd8EqI?si=G_3CqFRAmeVPczjj" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Compare Folders From Properties

 To compare the number of files, subfolders, the size, and the creation date of two folders, use the Properties option in Windows File Explorer. This lets you quickly glance at the main attributes of a folder.

 To start, [launch File Explorer](https://pokemon-go-android.techidaily.com/how-to-get-and-use-pokemon-go-promo-codes-on-realme-c67-4g-drfone-by-drfone-virtual-android/) using Windows+E. Find the first folder, right-click it, and select "Properties."

!['Properties' highlighted for a folder in File Explorer.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/1-folder-properties.jpg) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/FLlUft1ZxI0?si=pBd5QdHEE27qsNlN" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Keep the first folder’s "Properties" window open. Then, find the second folder, right-click it, and select "Properties."

 You now have the "Properties" window open for both your folders. Bring these windows side-by-side by [dragging them](https://extra-resources.techidaily.com/mastering-complex-video-effects-and-transitions-in-gopro-studio/), and you can see the differences in the contents of these folders. For example, you can see how many files both folders have, what size these folders are, and so on.

!['Properties' windows for two folders in File Explorer.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/2-compare-folder-properties.jpg) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/Nl0Z0eth1u4?si=0eecOBNfc--51AJO" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 That gives you a general overview of the differences between your folders.

##  Compare Folders Using Command Prompt

 If you prefer command line methods over graphical ones, use the robocopy command in Command Prompt to see the differences between the two folders. This command is actually for [copying files from one folder to another](https://twitter-videos.techidaily.com/new-in-2024-gain-twitter-gifs-for-pc-download-made-simple/), but you can make it show the differences between two specified folders and not copy any files.

 To use robocopy, first open the Start Menu, search **Command Prompt**, and launch it.

![Command Prompt highlighted in Start Menu.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/3-launch-command-prompt.jpg) 

 In Command Prompt, type the following command. Replace "Folder1" with the path to your first folder and "Folder2" with the path to your second folder. Ensure both folder paths are enclosed in double quotes.

 To copy a folder’s full path along with double quotes around the path, hold down the Shift key on your keyboard, right-click your folder, and choose "Copy as Path."

robocopy "Folder1" "Folder2" /L /NJH /NJS /NP /NS

![The 'robocopy' command typed in Command Prompt.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/4-compare-folders-command-prompt.jpg) 

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

 For the "2nd File or Folder" field, click the "Browse" button and choose the second folder to compare.

!['Browse' highlighted for the '2nd File or Folder' field in WinMerge.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/7-add-second-folder-winmerge.jpg) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/YB7Ou4-iKVM?si=7Fq8iUwI8voccMLx" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 In both fields, enable the "Read-Only" option. Click the "Folder: Filter" field and type **\*.\*** if it isn’t already there. This ensures the app compares all the files in both the specified folders. Then, at the bottom, click "Compare."

![Various comparison options highlighted in WinMerge.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/8-configure-comparison-options-winmerge.jpg) 

 On the following screen, you’ll see the comparison of the specified folders. You’ll see information like identical files in both folders, files missing from one folder, and so on.

![The comparison of two folders in WinMerge.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/9-folder-comparison-winmerge.jpg) 

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
<li><a href="https://vp-tips.techidaily.com/new-a-beginners-guide-to-use-snapseed-photo-editing-features/"><u>[New] A Beginner's Guide to Use Snapseed Photo Editing Features</u></a></li>
<li><a href="https://fox-info.techidaily.com/new-dissection-of-goofy-quest-the-videotape-perspective/"><u>[New] Dissection of 'Goofy Quest' – The Videotape Perspective</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-illuminating-the-art-of-iphone-long-exposure/"><u>[New] Illuminating the Art of iPhone Long Exposure</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-initiating-immediate-creation-of-captivating-facebook-panoramas/"><u>[New] Initiating Immediate Creation of Captivating Facebook Panoramas</u></a></li>
<li><a href="https://youtube-data.techidaily.com/ed-2024-approved-everything-you-need-to-know-about-youtube-shorts/"><u>[Updated] 2024 Approved Everything You Need to Know About YouTube Shorts</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-exploring-the-metaverses-humorous-realms-together/"><u>[Updated] Exploring the Metaverse's Humorous Realms Together</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-from-newbie-to-zoom-whiz-in-no-time/"><u>[Updated] From Newbie to Zoom Whiz in No Time</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-harmonizing-sights-with-itunes-acoustics/"><u>[Updated] Harmonizing Sights with iTunes Acoustics</u></a></li>
<li><a href="https://mondly-stories.techidaily.com/apertenca-a-cultura-portuguesa-greves-tipicas/"><u>Apertença À Cultura Portuguesa: Greves Tipicas</u></a></li>
<li><a href="https://some-techniques.techidaily.com/guide-to-mastering-windows-movie-maker-in-w11-for-beginners-for-2024/"><u>Guide to Mastering Windows Movie Maker in W11 for Beginners for 2024</u></a></li>
<li><a href="https://fix-guide.techidaily.com/how-to-flash-dead-samsung-galaxy-s23-tactical-edition-safely-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>How to Flash Dead Samsung Galaxy S23 Tactical Edition Safely | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-illumination-innovations-advanced-lighting-in-video-making/"><u>In 2024, Illumination Innovations Advanced Lighting in Video Making</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/in-2024-mastering-modern-photographys-dynamic-range-capabilities/"><u>In 2024, Mastering Modern Photography's Dynamic Range Capabilities</u></a></li>
<li><a href="https://tiktok-clips.techidaily.com/in-2024-melodies-meet-movements-creating-tiktok-videos-with-music/"><u>In 2024, Melodies Meet Movements Creating TikTok Videos with Music</u></a></li>
<li><a href="https://youtube-help.techidaily.com/in-2024-unveiling-t-series-profit-generation-methods-on-youtube/"><u>In 2024, Unveiling T-Series' Profit Generation Methods on YouTube</u></a></li>
</ul></div>

