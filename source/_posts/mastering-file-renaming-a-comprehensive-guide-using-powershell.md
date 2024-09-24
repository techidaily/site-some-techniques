---
title: "Mastering File Renaming: A Comprehensive Guide Using PowerShell"
date: 2024-09-19T21:48:44.094Z
updated: 2024-09-24T00:22:40.175Z
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
<a href="https://appsumo.8odi.net/c/5597632/2151884/7443" target="_top" id="2151884">
  <img src="//a.impactradius-go.com/display-ad/7443-2151884" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2151884/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 That action has copied your selected item’s full path to your clipboard. You can now [paste this path](https://twitter-videos.techidaily.com/new-in-2024-gain-twitter-gifs-for-pc-download-made-simple/) wherever required in the commands below.

<!-- affiliate ads begin -->
<a href="https://laganoo.pxf.io/c/5597632/1484909/16446" target="_top" id="1484909">
  <img src="//a.impactradius-go.com/display-ad/16446-1484909" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://laganoo.pxf.io/i/5597632/1484909/16446" style="position:absolute;visibility:hidden;" border="0" />
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

##  How to Rename Files in a Folder With an Increasing Number

 If you want to add an increasing number, such as 1, 2, 3, and so on, to your files in a specific folder, follow these steps.

 Launch a PowerShell window and type the following command. Replace **PATH** with the full path to your folder, and **txt** with the format of the files to rename. Then, press Enter.

Get-ChildItem PATH -Recurse -Include "*.txt" | ForEach-Object -Begin { $Counter = 1 } -Process { Rename-Item $_.FullName -NewName ("{0}_{1}" -f $Counter, $_.Name) ; $Counter++ }

![Files with an increasing number in File Explorer.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/3-add-numbers-to-file-names.jpg) 

<!-- affiliate ads begin -->
<a href="https://ephamedtechinc.pxf.io/c/5597632/2136624/26400" target="_top" id="2136624">
  <img src="//a.impactradius-go.com/display-ad/26400-2136624" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://ephamedtechinc.pxf.io/i/5597632/2136624/26400" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  How to Add a Prefix or Suffix to a File Name

 To add text before your file name (known as a prefix), launch a PowerShell window and enter the following command. Replace **PATH** with your folder's full path, and **PREFIX** with the text you want to append, then press Enter.

Get-ChildItem PATH | Rename-Item -NewName {"PREFIX" + $_.Name}

 To add text after your file’s name (called a suffix), use the following command, replacing **PATH** with the full path to your folder, and **SUFFIX** with the text to append. Then, press Enter.

Get-ChildItem PATH | Rename-Item -NewName {$_.BaseName + "SUFFIX" + $_.Extension}

<!-- affiliate ads begin -->
<a href="https://wigfever.sjv.io/c/5597632/2014857/22899" target="_top" id="2014857">
  <img src="//a.impactradius-go.com/display-ad/22899-2014857" border="0" alt="https://techidaily.com" width="320" height="90"/>
</a>
<img height="0" width="0" src="https://wigfever.sjv.io/i/5597632/2014857/22899" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://tiktok-clips.techidaily.com/new-hacking-tiktoks-video-pace-efficiently-for-2024/"><u>[New] Hacking TikTok's Video Pace Efficiently for 2024</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/updated-ignite-the-flames-strategies-for-growing-your-youtube-audience/"><u>[Updated] Ignite the Flames Strategies for Growing Your YouTube Audience</u></a></li>
<li><a href="https://fox-cloud.techidaily.com/updated-samsungs-gear-360-challenger-the-best-cameras-of-the-year/"><u>[Updated] Samsung’s Gear 360 Challenger The Best Cameras of the Year</u></a></li>
<li><a href="https://extra-lessons.techidaily.com/a-thorough-introduction-to-gdocs-speech-to-text-capabilities-for-2024/"><u>A Thorough Introduction to GDoc's Speech-to-Text Capabilities for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/conversion-gratuite-de-fichier-pcx-en-image-animee-gif-avec-movavi-tutoriel/"><u>Conversion Gratuite De Fichier PCX en Image Animée (GIF) Avec Movavi - Tutoriel</u></a></li>
<li><a href="https://some-techniques.techidaily.com/conversion-libre-de-flv-a-wav-en-ligne-comment-utiliser-movavi-pour-convertir-vos-fichiers/"><u>Conversion Libre De Flv À Wav en Ligne : Comment Utiliser Movavi Pour Convertir Vos Fichiers</u></a></li>
<li><a href="https://some-techniques.techidaily.com/conversione-fatale-alaw-in-wav-su-internet-gratuita-utilizza-movavi/"><u>Conversione Fatale Alaw in Wav Su Internet Gratuita - Utilizza Movavi</u></a></li>
<li><a href="https://some-techniques.techidaily.com/conversione-on-line-gratuita-da-aac-a-3gp-con-movavi/"><u>Conversione On-Line Gratuita Da AAC a 3GP Con Movavi</u></a></li>
<li><a href="https://some-techniques.techidaily.com/converti-file-video-3gp-in-formato-audio-libero-m4a-con-movavi/"><u>Converti File Video 3GP in Formato Audio Libero M4A Con Movavi</u></a></li>
<li><a href="https://some-techniques.techidaily.com/convertissez-vos-fichiers-mpe-en-mp3-facilement-et-sans-frais-via-le-convertisseur-en-ligne-movavi/"><u>Convertissez Vos Fichiers MPE en MP3 Facilement Et Sans Frais via Le Convertisseur en Ligne Movavi</u></a></li>
<li><a href="https://some-techniques.techidaily.com/denne-side-de-bedste-youtube-till-mp3-konverterne-indkald-movavi-for-venligst-fremmede-dybe-livsstil/"><u>Denne Side: De Bedste YouTube Till MP3 Konverterne - Indkald Movavi for Venligst Fremmede Dybe Livsstil</u></a></li>
<li><a href="https://some-techniques.techidaily.com/discover-photographic-artistry-paula-beatons-portfolio-showcased-by-movavi/"><u>Discover Photographic Artistry - Paula Beaton's Portfolio Showcased by Movavi</u></a></li>
<li><a href="https://some-techniques.techidaily.com/download-bandicam-free-on-mac-by-movavi-easy-video-capture-software/"><u>Download Bandicam Free on Mac by Movavi: Easy Video Capture Software</u></a></li>
<li><a href="https://win11-tips.techidaily.com/eternal-trash-bin-configurations-in-your-windows-1011-dock/"><u>Eternal Trash Bin Configurations in Your Windows 10/11 Dock</u></a></li>
<li><a href="https://win-howtos.techidaily.com/fixing-the-runtimebrokers-excessive-resource-consumption-problem-on-your-windows-10-pc/"><u>Fixing the RunTimeBroker's Excessive Resource Consumption Problem on Your Windows 10 PC</u></a></li>
<li><a href="https://video-capture.techidaily.com/in-2024-echo-chambers-tech-updates/"><u>In 2024, Echo Chambers Tech Updates</u></a></li>
<li><a href="https://tech-recovery.techidaily.com/step-by-step-guide-complete-factory-reset-on-your-dell-computer/"><u>Step-by-Step Guide: Complete Factory Reset on Your Dell Computer</u></a></li>
<li><a href="https://pokemon-go-android.techidaily.com/the-best-ispoofer-alternative-to-try-on-honor-x50i-drfone-by-drfone-virtual-android/"><u>The Best iSpoofer Alternative to Try On Honor X50i | Dr.fone</u></a></li>
<li><a href="https://ai-voice-clone.techidaily.com/updated-2024-approved-ai-avatars-online/"><u>Updated 2024 Approved AI Avatars | Online</u></a></li>
</ul></div>

