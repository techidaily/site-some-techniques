---
title: "Securing Your PC: A Step-by-Step Guide to Locking Windows 11 with Command Line"
date: 2025-02-05T19:31:04.282Z
updated: 2025-02-09T19:12:46.614Z
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/XS1nQCe95LU?si=A2dhdFkSAI61_nKA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Lock Your Windows 10 PC Using Command Prompt

 First, [open the Command Prompt](https://android-frp.techidaily.com/in-2024-step-by-step-tutorial-how-to-bypass-oppo-a78-frp-by-drfone-android/) on your PC by opening the Start menu, typing “cmd” in the Windows Search bar, and then selecting “Command Prompt” from the search results.

![Click the Start button, search for 'cmd,' then open 'Command Prompt.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/1-launch-cmd.png) 

 Command Prompt will now open. Here, run this command to lock your Windows 10 PC.

Rundll32.exe user32.dll,LockWorkStation

![Locking your PC with Command Prompt.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/2-lock-pc-command-prompt.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/h5uImbOWmTg?si=z4kP-R0QbXbBAJTa" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Once executed, your PC will be locked. You'll have to sign back in with your PIN, password, or whatever sign-in method you usually use.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/n-66V-LRK3Y?si=fNeB2pXCePeQli6E" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Set the Lock Screen Timeout Setting Using Command Prompt

 Once you’ve locked your PC, the lock screen will generally be displayed for a certain amount of time before it time outs. You can set the amount of time that needs to pass before timing out using the Command Prompt.

 To do this, you’ll need to [open Command Prompt as an admin](https://screen-mirror.techidaily.com/how-to-screen-mirroring-xiaomi-14-ultra-drfone-by-drfone-android/). Do so by typing “cmd” in the Windows Search bar and then right-clicking “Command Prompt” from the results. Next, select “Run As Administrator” from the menu that appears.

![Launching Command Prompt as admin.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/3-launch-cmd.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/TJCye_oCTTw?si=6bVyBphcSgSFdyuq" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 With Command Prompt open, run this command.

powercfg.exe /SETACVALUEINDEX SCHEME_CURRENT SUB_VIDEO VIDEOCONLOCK <time>

 Replace `<time>` with your desired amount of time in seconds. That means if you want to time out the lock screen after two minutes, you’d enter this command:

powercfg.exe /SETACVALUEINDEX SCHEME_CURRENT SUB_VIDEO VIDEOCONLOCK 120

![Change the timeout to 120.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/4-changing-timeout-to-120.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/PKZUYice-ws?si=L8iMa9T3h7TMSWdQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://some-techniques.techidaily.com/new-from-zip-to-sub-transforming-compressed-texts-to-srt-format/"><u>[New] From Zip to Sub Transforming Compressed Texts to SRT Format</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-how-to-make-your-solitary-voice-resonate/"><u>[New] How To Make Your Solitary Voice Resonate</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-ignite-social-media-fanfare-master-these-9-instagram-commandments/"><u>[New] Ignite Social Media Fanfare Master These 9 Instagram Commandments</u></a></li>
<li><a href="https://screen-recording.techidaily.com/new-unlocking-the-power-of-skype-recordings-on-windows-and-mac-for-2024/"><u>[New] Unlocking the Power of Skype Recordings on Windows & Mac for 2024</u></a></li>
<li><a href="https://youtube-lab.techidaily.com/ed-best-soundshapers-for-content-makers-on-youtube-for-2024/"><u>[Updated] Best Soundshapers for Content Makers on YouTube for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-explore-free-fcp-download-options/"><u>[Updated] Explore FREE FCP Download Options</u></a></li>
<li><a href="https://extra-skills.techidaily.com/updated-is-inshot-the-best-of-the-best-expert-reviews-speak-up/"><u>[Updated] Is InShot The Best of the Best? Expert Reviews Speak Up</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-from-everyday-use-to-extraordinary-virtual-adventures-smartphone-vr-conversion-guide/"><u>2024 Approved From Everyday Use to Extraordinary Virtual Adventures Smartphone-VR Conversion Guide</u></a></li>
<li><a href="https://fox-info.techidaily.com/2024-approved-premium-internet-spots-for-glossy-3d-text-effects/"><u>2024 Approved Premium Internet Spots for Glossy 3D Text Effects</u></a></li>
<li><a href="https://fake-location.techidaily.com/how-to-change-netflix-location-to-get-more-country-version-on-xiaomi-14-drfone-by-drfone-virtual-android/"><u>How to Change Netflix Location to Get More Country Version On Xiaomi 14 | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-explore-virtual-worlds-pcs-1-list-of-vr-360-game-streamers/"><u>In 2024, Explore Virtual Worlds PC's #1 List of VR 360 Game Streamers</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-innovations-in-hand-tracking-and-gesture-detection/"><u>In 2024, Innovations in Hand Tracking and Gesture Detection</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/innovative-techniques-improve-your-hp-laptop-screen-recordings/"><u>Innovative Techniques Improve Your HP Laptop Screen Recordings</u></a></li>
<li><a href="https://youtube-sure.techidaily.com/r-the-art-of-youtube-visibility-two-steps/"><u>Master the Art of YouTube Visibility (Two Steps)</u></a></li>
<li><a href="https://ai-video-tools.techidaily.com/updated-in-2024-fcpx-video-accessibility-adding-subtitles-and-captions/"><u>Updated In 2024, FCPX Video Accessibility Adding Subtitles and Captions</u></a></li>
</ul></div>

