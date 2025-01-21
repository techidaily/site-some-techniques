---
title: "Securing Your PC: A Step-by-Step Guide to Locking Windows 11 with Command Line"
date: 2025-01-15T16:03:59.350Z
updated: 2025-01-21T21:40:45.177Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://thmb.techidaily.com/07cfabd2fe9acb782e30cca8205dc0f557a2c3371dbf02532bc0633c00063d56.jpg
---

## Securing Your PC: A Step-by-Step Guide to Locking Windows 11 with Command Line

### Quick Links

* [Lock Your Windows 10 PC Using Command Prompt](https://vp-tips.techidaily.com/new-audiovisual-adaptability-in-free-fire-for-2024/)
* [Set the Lock Screen Timeout Setting Using Command Prompt](https://eaxpv-info.techidaily.com/new-finding-a-different-way-to-naming-your-channel-with-filmora-for-2024/)

### Key Takeaways

* To lock your Windows PC using Command Prompt, run "**Rundll32.exe user32.dll,LockWorkStation"** in the Command Prompt
* To set the lock screen timeout, run "**powercfg.exe /SETACVALUEINDEX SCHEME\_CURRENT SUB\_VIDEO VIDEOCONLOCK <time>"** in Command Prompt as Admin
* Activate the lock screen timeout setting by running "**powercfg.exe /SETACTIVE SCHEME\_CURRENT"** after you set the timeout.

 One of the first rules of cyber security is to always lock your PC before stepping away. While it may not be the quickest way to lock your Windows 10 PC, you can do it using the Command Prompt.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/2Iv3DjT2Fyw?si=pR_z8ZDDVGF2MvKJ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Lock Your Windows 10 PC Using Command Prompt

 First, [open the Command Prompt](https://android-frp.techidaily.com/in-2024-step-by-step-tutorial-how-to-bypass-oppo-a78-frp-by-drfone-android/) on your PC by opening the Start menu, typing “cmd” in the Windows Search bar, and then selecting “Command Prompt” from the search results.

![Click the Start button, search for 'cmd,' then open 'Command Prompt.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/1-launch-cmd.png) 

 Command Prompt will now open. Here, run this command to lock your Windows 10 PC.

Rundll32.exe user32.dll,LockWorkStation

![Locking your PC with Command Prompt.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/2-lock-pc-command-prompt.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/LaWcXdTn5SE?si=QbxEkX-4a17J5RVs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Once executed, your PC will be locked. You'll have to sign back in with your PIN, password, or whatever sign-in method you usually use.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/jjGL9wFdlbo?si=Vb1JgZqRXNc03UGG" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Set the Lock Screen Timeout Setting Using Command Prompt

 Once you’ve locked your PC, the lock screen will generally be displayed for a certain amount of time before it time outs. You can set the amount of time that needs to pass before timing out using the Command Prompt.

 To do this, you’ll need to [open Command Prompt as an admin](https://screen-mirror.techidaily.com/how-to-screen-mirroring-xiaomi-14-ultra-drfone-by-drfone-android/). Do so by typing “cmd” in the Windows Search bar and then right-clicking “Command Prompt” from the results. Next, select “Run As Administrator” from the menu that appears.

![Launching Command Prompt as admin.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/3-launch-cmd.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/DBMTAJBx-X4?si=sje5pFJXiHzJJGbP" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 With Command Prompt open, run this command.

powercfg.exe /SETACVALUEINDEX SCHEME_CURRENT SUB_VIDEO VIDEOCONLOCK <time>

 Replace `<time>` with your desired amount of time in seconds. That means if you want to time out the lock screen after two minutes, you’d enter this command:

powercfg.exe /SETACVALUEINDEX SCHEME_CURRENT SUB_VIDEO VIDEOCONLOCK 120

![Change the timeout to 120.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/4-changing-timeout-to-120.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/aoMiYpYiFZs?si=qvYvGytDD17fvSXO" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 This command sets the lock screen timeout setting for your PC if it’s plugged in to a power source. To set the lock screen timeout setting for your PC if it’s running on battery, change`/SETACVALUEINDEX` to`/SETDCVALUEINDEX` and run the command as normal.

 Next, run this command:

powercfg.exe /SETACTIVE SCHEME_CURRENT

![Apply the setting to the currently active scheme.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/5-set-active.png) 

 Now your [lock screen](https://driver-download.techidaily.com/1722977751917-synaptics-drivers-download-and-update-for-windows-easily/) will timeout after the set amount of time. Give it a try!

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
<li><a href="https://some-techniques.techidaily.com/new-ideal-soundscapes-for-editing-films-and-vids/"><u>[New] Ideal Soundscapes for Editing Films & Vids</u></a></li>
<li><a href="https://facebook-video-content.techidaily.com/updated-2024-approved-enhancing-social-media-presence-with-professional-slideshow-making/"><u>[Updated] 2024 Approved Enhancing Social Media Presence with Professional Slideshow Making</u></a></li>
<li><a href="https://vimeo-videos.techidaily.com/updated-in-2024-step-by-step-instructions-for-extracting-mp3-from-video/"><u>[Updated] In 2024, Step-By-Step Instructions for Extracting MP3 From Video</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-excellent-20-anime-opening-anthems/"><u>2024 Approved Excellent 20 Anime Opening Anthems</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-how-to-optimize-solo-streaming-with-flawless-execution/"><u>2024 Approved How to Optimize Solo Streaming with Flawless Execution</u></a></li>
<li><a href="https://fox-links.techidaily.com/2024-approved-the-best-professional-template-pack-for-premiere-pro/"><u>2024 Approved The Best Professional Template Pack for Premiere Pro</u></a></li>
<li><a href="https://location-fake.techidaily.com/a-detailed-guide-on-faking-your-location-in-mozilla-firefox-on-samsung-galaxy-s24plus-drfone-by-drfone-virtual-android/"><u>A Detailed Guide on Faking Your Location in Mozilla Firefox On Samsung Galaxy S24+ | Dr.fone</u></a></li>
<li><a href="https://win-great.techidaily.com/effective-techniques-to-maintain-your-scanner-and-avoid-breakdowns-tips-from-yl-computing/"><u>Effective Techniques to Maintain Your Scanner and Avoid Breakdowns: Tips From YL Computing</u></a></li>
<li><a href="https://win11-tips.techidaily.com/exploring-uses-for-microsofts-vcplusplus-distribute/"><u>Exploring Uses for Microsoft's VC++ Distribute</u></a></li>
<li><a href="https://some-techniques.techidaily.com/fuse-rhythms-into-powerpoint-layouts-for-2024/"><u>Fuse Rhythms Into PowerPoint Layouts for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/holographic-horizons-reimagined-movies-for-2024/"><u>Holographic Horizons Reimagined Movies for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/immerse-in-visual-creation-best-3d-model-and-rendering-tools-reviewed-for-2024/"><u>Immerse in Visual Creation Best 3D Model & Rendering Tools Reviewed for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-from-speech-to-text-your-all-inclusive-gdoc-training-guide/"><u>In 2024, From Speech to Text Your All-Inclusive GDoc Training Guide</u></a></li>
<li><a href="https://solve-marvelous.techidaily.com/masterful-mobile-tools-abbyys-guide-to-enhancing-smartphone-productivity-with-ocr/"><u>Masterful Mobile Tools: ABBYY's Guide to Enhancing Smartphone Productivity with OCR</u></a></li>
<li><a href="https://video-content-creator.techidaily.com/new-in-2024-the-ultimate-mp4-video-editing-tutorial-for-mac-and-windows-users/"><u>New In 2024, The Ultimate MP4 Video Editing Tutorial for Mac and Windows Users</u></a></li>
</ul></div>

