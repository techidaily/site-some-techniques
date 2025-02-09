---
title: Comparing Folders Across Windows 11 & 10 - A Comprehensive Guide
date: 2025-02-07T20:16:49.069Z
updated: 2025-02-09T20:06:34.987Z
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

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/793ViIxl4tI?si=DDBkjPlPX5bZ-f1Y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

### Key Takeaways

* One way to compare folders is to right-click your folders one at a time and choose "Properties" for each. Then compare the Properties window of each folder.
* The robocopy command is a command-line tool that can be used to view the differences between folder.
* Use WinMerge to compare the contents and details of folders if you want a graphical tool.

 Do you want to compare the number of files or folders or simply visualize the difference between two folders? If so, you have two graphical and one command line method to do that. We’ll show you how to perform the folder comparison task on your Windows 11 or Windows 10 PC.

##  Compare Folders From Properties

 To compare the number of files, subfolders, the size, and the creation date of two folders, use the Properties option in Windows File Explorer. This lets you quickly glance at the main attributes of a folder.

 To start, [launch File Explorer](https://pokemon-go-android.techidaily.com/how-to-get-and-use-pokemon-go-promo-codes-on-realme-c67-4g-drfone-by-drfone-virtual-android/) using Windows+E. Find the first folder, right-click it, and select "Properties."

!['Properties' highlighted for a folder in File Explorer.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/1-folder-properties.jpg) 

 Keep the first folder’s "Properties" window open. Then, find the second folder, right-click it, and select "Properties."

 You now have the "Properties" window open for both your folders. Bring these windows side-by-side by [dragging them](https://extra-resources.techidaily.com/mastering-complex-video-effects-and-transitions-in-gopro-studio/), and you can see the differences in the contents of these folders. For example, you can see how many files both folders have, what size these folders are, and so on.

!['Properties' windows for two folders in File Explorer.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/2-compare-folder-properties.jpg) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/FLO5dwmJAVs?si=1OYH8rv8aPaMsCiU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/0OxkndZbIA4?si=TWJlkTbYKsVag8-q" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 For the "2nd File or Folder" field, click the "Browse" button and choose the second folder to compare.

!['Browse' highlighted for the '2nd File or Folder' field in WinMerge.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/7-add-second-folder-winmerge.jpg) 

 In both fields, enable the "Read-Only" option. Click the "Folder: Filter" field and type **\*.\*** if it isn’t already there. This ensures the app compares all the files in both the specified folders. Then, at the bottom, click "Compare."

![Various comparison options highlighted in WinMerge.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/8-configure-comparison-options-winmerge.jpg) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/E1ax-vnGdeo?si=bgTkOhOEwDTlRQE3" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 On the following screen, you’ll see the comparison of the specified folders. You’ll see information like identical files in both folders, files missing from one folder, and so on.

![The comparison of two folders in WinMerge.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/9-folder-comparison-winmerge.jpg) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/E3yY7lZ-FKA?si=g8VEuExP8GH59B69" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://fox-hovers.techidaily.com/new-2024-approved-edit-like-a-pro-with-these-top-5-mac-videography-suites/"><u>[New] 2024 Approved Edit Like a Pro with These Top 5 Mac Videography Suites</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-ideal-platforms-creating-movies-from-photo-galleries/"><u>[New] Ideal Platforms Creating Movies From Photo Galleries</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-impart-rotational-luminosity-modification-in-photoshopping/"><u>[New] Impart Rotational Luminosity Modification in Photoshopping</u></a></li>
<li><a href="https://snapchat-videos.techidaily.com/new-in-2024-uncomplicated-multisnap-storytelling-on-snapchat/"><u>[New] In 2024, Uncomplicated Multisnap Storytelling on Snapchat</u></a></li>
<li><a href="https://some-tips.techidaily.com/new-the-evolution-of-live-streaming-with-periscope/"><u>[New] The Evolution of Live Streaming with Periscope</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-from-shadows-to-highlights-the-ultimate-lightroom-hdr-guide/"><u>[Updated] From Shadows to Highlights The Ultimate Lightroom HDR Guide</u></a></li>
<li><a href="https://extra-skills.techidaily.com/updated-premier-annual-update-best-free-livestream-software-and-apps-review/"><u>[Updated] Premier Annual Update Best Free Livestream Software & Apps Review</u></a></li>
<li><a href="https://technical-tips.techidaily.com/choosing-your-next-apple-device-a-comparison-of-the-latest-macbook-air-models-m3-vs-m2-expert-advice-from-zdnet/"><u>Choosing Your Next Apple Device: A Comparison of the Latest MacBook Air Models (M3 vs M2) - Expert Advice From ZDNet</u></a></li>
<li><a href="https://tech-revival.techidaily.com/demystifying-hugging-face-how-it-works-and-its-impact-on-tech/"><u>Demystifying Hugging Face: How It Works and Its Impact on Tech</u></a></li>
<li><a href="https://some-techniques.techidaily.com/filming-your-journey-essentials-checklist-for-2024/"><u>Filming Your Journey – Essentials Checklist for 2024</u></a></li>
<li><a href="https://technical-tips.techidaily.com/fixed-my-apple-watch-cellular-issue-learn-how-with-these-simple-steps/"><u>Fixed My Apple Watch Cellular Issue - Learn How with These Simple Steps</u></a></li>
<li><a href="https://some-techniques.techidaily.com/heroic-footage-face-off-black-vs-silver-in-the-gopro-wars-for-2024/"><u>HEROic Footage Face-Off Black vs Silver in the GoPro Wars for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/ideal-software-tools-for-embossing-photos-with-framing-for-2024/"><u>Ideal Software Tools for Embossing Photos with Framing for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-exclusive-top-5-iphone-podcast-apps-guide/"><u>In 2024, Exclusive Top 5 iPhone Podcast Apps Guide</u></a></li>
<li><a href="https://activate-lock.techidaily.com/in-2024-how-to-bypass-activation-lock-on-apple-iphone-6-plus-or-ipad-by-drfone-ios/"><u>In 2024, How to Bypass Activation Lock on Apple iPhone 6 Plus or iPad?</u></a></li>
<li><a href="https://vp-tips.techidaily.com/ultimate-guide-to-multi-camera-recording-with-manycams-professional-software-solutions/"><u>Ultimate Guide to Multi-Camera Recording with ManyCam's Professional Software Solutions</u></a></li>
</ul></div>

