---
title: Easy Steps to Rename Your Files with Windows PowerShell Tools
date: 2024-10-26T16:26:35.611Z
updated: 2024-10-29T17:36:17.857Z
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
<span id="1977004">
					<video width="128" height="480" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1977004.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/22993-1977004">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1977004.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:80px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fhomestyler.sjv.io%2Fc%2F5597632%2F1977004%2F22993'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1977004/22993" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Before You Begin: Learn How to Find a File or Folder’s Full Path

 To rename files, you’ll have to provide PowerShell with your file or parent folder’s full path. If you know how to do this, skip to the relevant section below. If you aren’t quite sure [how to get a folder or file’s full path](https://fox-links.techidaily.com/updated-2024-approved-unparalleled-screenplay-craftsmanship-across-varied-fields/), we’ll show you.

[Open a File Explorer window](https://pokemon-go-android.techidaily.com/how-to-get-and-use-pokemon-go-promo-codes-on-realme-c67-4g-drfone-by-drfone-virtual-android/) and find your file or folder. Press and hold down the Shift key on your keyboard, right-click your file or folder, and choose "Copy as Path."

!['Copy as Path' highlighted in Windows 11's context menu.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/1-copy-file-path-windows.jpg) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1934183/19272" target="_top" id="1934183">
  <img src="//a.impactradius-go.com/display-ad/19272-1934183" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1934183/19272" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://aligracehair.sjv.io/c/5597632/1896555/19272" target="_top" id="1896555">
  <img src="//a.impactradius-go.com/display-ad/19272-1896555" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1896555/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 PowerShell won’t display a message confirming your file is renamed, but know that the job is done.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/1062450/7443" target="_top" id="1062450">
  <img src="//a.impactradius-go.com/display-ad/7443-1062450" border="0" alt="https://techidaily.com" width="600" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/1062450/7443" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://fox-access.techidaily.com/new-bend-the-rules-of-livestreaming-on-youtube-without-a-subscriber-hurdle/"><u>[New] Bend the Rules of Livestreaming on YouTube, Without a Subscriber Hurdle</u></a></li>
<li><a href="https://instagram-clips.techidaily.com/updated-2024-approved-masterclass-in-muting-and-dismantling-an-instagram-account/"><u>[Updated] 2024 Approved Masterclass in Muting & Dismantling an Instagram Account</u></a></li>
<li><a href="https://extra-hints.techidaily.com/updated-accessing-and-using-srt-audio-on-various-oses/"><u>[Updated] Accessing and Using SRT Audio on Various OSes</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-fusing-music-and-photos-online/"><u>[Updated] Fusing Music and Photos Online</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-innovative-metaverse-humor-generating-unique-memes/"><u>[Updated] Innovative Metaverse Humor Generating Unique Memes</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-free-voice-modification-tools-enhance-your-auditory-presentation/"><u>2024 Approved Free Voice Modification Tools – Enhance Your Auditory Presentation</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-freescape-extraction-revisited-a-look-at-the-latest-update/"><u>2024 Approved Freescape Extraction Revisited A Look at the Latest Update</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-from-meta-to-omni-a-new-age-digital-odyssey-guide/"><u>2024 Approved From Meta to Omni A New Age Digital Odyssey Guide</u></a></li>
<li><a href="https://app-tips.techidaily.com/cognitive-network-advancements-from-arista-enter-mainstream-sectors-a-deep-dive-tech-insights/"><u>Cognitive Network Advancements From Arista Enter Mainstream Sectors: A Deep Dive - Tech Insights</u></a></li>
<li><a href="https://extra-hints.techidaily.com/dive-into-memelore-the-kinemaster-method/"><u>Dive Into Memelore The KineMaster Method</u></a></li>
<li><a href="https://some-techniques.techidaily.com/from-sound-to-web-crafting-a-standout-podcast-rss-feed-for-2024/"><u>From Sound to Web Crafting a Standout Podcast RSS Feed for 2024</u></a></li>
<li><a href="https://games-able.techidaily.com/game-mastery-reimagined-top-6-innovations-with-gpt-assistance/"><u>Game Mastery Reimagined: Top 6 Innovations with GPT Assistance</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-expert-zoom-and-cut-companion/"><u>In 2024, Expert Zoom and Cut Companion</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-high-end-displays-ranked-1-to-5-ps5/"><u>In 2024, High-End Displays Ranked #1 to #5 (PS5)</u></a></li>
<li><a href="https://fox-helps.techidaily.com/inside-facetune-an-authoritative-review-for-improved-images-for-2024/"><u>Inside Facetune An Authoritative Review for Improved Images for 2024</u></a></li>
<li><a href="https://extra-hints.techidaily.com/space-saver-protocols-premium-storage-reviewed/"><u>Space Saver Protocols Premium Storage Reviewed</u></a></li>
<li><a href="https://iphone-unlock.techidaily.com/unlock-your-disabled-apple-iphone-13-pro-without-itunes-in-5-ways-drfone-by-drfone-ios/"><u>Unlock Your Disabled Apple iPhone 13 Pro Without iTunes in 5 Ways | Dr.fone</u></a></li>
</ul></div>

