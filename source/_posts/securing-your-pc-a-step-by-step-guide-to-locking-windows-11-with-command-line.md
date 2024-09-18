---
title: "Securing Your PC: A Step-by-Step Guide to Locking Windows 11 with Command Line"
date: 2024-09-17T17:38:58.113Z
updated: 2024-09-18T17:33:27.142Z
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

##  Lock Your Windows 10 PC Using Command Prompt

 First, [open the Command Prompt](https://android-frp.techidaily.com/in-2024-step-by-step-tutorial-how-to-bypass-oppo-a78-frp-by-drfone-android/) on your PC by opening the Start menu, typing “cmd” in the Windows Search bar, and then selecting “Command Prompt” from the search results.

![Click the Start button, search for 'cmd,' then open 'Command Prompt.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/1-launch-cmd.png) 

 Command Prompt will now open. Here, run this command to lock your Windows 10 PC.

Rundll32.exe user32.dll,LockWorkStation

![Locking your PC with Command Prompt.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/2-lock-pc-command-prompt.png) 

 Once executed, your PC will be locked. You'll have to sign back in with your PIN, password, or whatever sign-in method you usually use.

<!-- affiliate ads begin -->
<a href="https://zebaoaffiliateprogram.pxf.io/c/5597632/2137973/21526" target="_top" id="2137973">
  <img src="//a.impactradius-go.com/display-ad/21526-2137973" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://zebaoaffiliateprogram.pxf.io/i/5597632/2137973/21526" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Set the Lock Screen Timeout Setting Using Command Prompt

 Once you’ve locked your PC, the lock screen will generally be displayed for a certain amount of time before it time outs. You can set the amount of time that needs to pass before timing out using the Command Prompt.

 To do this, you’ll need to [open Command Prompt as an admin](https://screen-mirror.techidaily.com/how-to-screen-mirroring-xiaomi-14-ultra-drfone-by-drfone-android/). Do so by typing “cmd” in the Windows Search bar and then right-clicking “Command Prompt” from the results. Next, select “Run As Administrator” from the menu that appears.

![Launching Command Prompt as admin.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/3-launch-cmd.png) 

 With Command Prompt open, run this command.

powercfg.exe /SETACVALUEINDEX SCHEME_CURRENT SUB_VIDEO VIDEOCONLOCK <time>

 Replace `<time>` with your desired amount of time in seconds. That means if you want to time out the lock screen after two minutes, you’d enter this command:

powercfg.exe /SETACVALUEINDEX SCHEME_CURRENT SUB_VIDEO VIDEOCONLOCK 120

![Change the timeout to 120.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/4-changing-timeout-to-120.png) 

 This command sets the lock screen timeout setting for your PC if it’s plugged in to a power source. To set the lock screen timeout setting for your PC if it’s running on battery, change`/SETACVALUEINDEX` to`/SETDCVALUEINDEX` and run the command as normal.

 Next, run this command:

powercfg.exe /SETACTIVE SCHEME_CURRENT

![Apply the setting to the currently active scheme.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/5-set-active.png) 

<!-- affiliate ads begin -->
<a href="https://zebaoaffiliateprogram.pxf.io/c/5597632/2137974/21526" target="_top" id="2137974">
  <img src="//a.impactradius-go.com/display-ad/21526-2137974" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://zebaoaffiliateprogram.pxf.io/i/5597632/2137974/21526" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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
<li><a href="https://facebook-video-footage.techidaily.com/new-in-2024-crafting-team-videos-to-foster-viewership-and-following/"><u>[New] In 2024, Crafting Team Videos to Foster Viewership and Following</u></a></li>
<li><a href="https://vp-tips.techidaily.com/new-in-2024-digitize-effortlessly-turn-to-mematic/"><u>[New] In 2024, Digitize Effortlessly - Turn to Mematic</u></a></li>
<li><a href="https://article-helps.techidaily.com/new-in-2024-unveiling-optimal-sites-for-pixel-sounds/"><u>[New] In 2024, Unveiling Optimal Sites for Pixel Sounds</u></a></li>
<li><a href="https://fox-hovers.techidaily.com/updated-2024-approved-zoomed-into-the-core-of-action-films/"><u>[Updated] 2024 Approved Zoomed Into the Core of Action Films</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/updated-collect-premium-audio-for-video-editors-for-2024/"><u>[Updated] Collect Premium Audio for Video Editors for 2024</u></a></li>
<li><a href="https://video-screen-grab.techidaily.com/updated-top-picks-for-retro-play-5-expert-picked-psone-emulators/"><u>[Updated] Top Picks for Retro Play 5 Expert-Picked PsOne Emulators</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/2024-approved-lg-virtual-reality-innovation-a-detailed-review/"><u>2024 Approved LG Virtual Reality Innovation A Detailed Review</u></a></li>
<li><a href="https://some-techniques.techidaily.com/section-3b-five-factaysis/"><u>Section 3B: Five Factaysis</u></a></li>
<li><a href="https://some-techniques.techidaily.com/step-by-step-guide-designing-and-sharing-your-own-customized-sticker-packs-on-telegram/"><u>Step-by-Step Guide: Designing and Sharing Your Own Customized Sticker Packs on Telegram</u></a></li>
<li><a href="https://fake-location.techidaily.com/the-best-8-vpn-hardware-devices-reviewed-on-vivo-t2-pro-5g-drfone-by-drfone-virtual-android/"><u>The Best 8 VPN Hardware Devices Reviewed On Vivo T2 Pro 5G | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/the-cross-talk-between-these-pathways-is-complex-for-example-autophagy-can-serve-as-a-cell-survival-mechanism-but-can-also-facilitate-apoptosis-if-it-fails-47/"><u>The Cross-Talk Between These Pathways Is Complex; for Example, Autophagy Can Serve as a Cell Survival Mechanism but Can Also Facilitate Apoptosis if It Fails to Allewarthe Stress Conditions Within the Cell.</u></a></li>
<li><a href="https://some-techniques.techidaily.com/the-significance-of-the-latest-iphone-os-update-why-ios-18-shakes-up-the-tech-world/"><u>The Significance of the Latest iPhone OS Update: Why iOS 18 Shakes Up the Tech World</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/the-stealthy-lens-approach-to-consuming-instagram-stories-on-desktop-and-mobile-devices/"><u>The Stealthy Lens Approach to Consuming Instagram Stories on Desktop & Mobile Devices</u></a></li>
<li><a href="https://some-techniques.techidaily.com/top-14-multiplayer-co-op-mobile-games-for-enjoying-time-together-on-android/"><u>Top 14 Multiplayer Co-Op Mobile Games for Enjoying Time Together on Android</u></a></li>
<li><a href="https://some-techniques.techidaily.com/top-6-amazing-ways-to-enhance-your-experience-with-samsung-dex/"><u>Top 6 Amazing Ways to Enhance Your Experience with Samsung DeX</u></a></li>
<li><a href="https://some-techniques.techidaily.com/transform-your-smartphone-into-an-enhanced-nintendo-switch-experience-with-just-one-gadget/"><u>Transform Your Smartphone Into an Enhanced Nintendo Switch Experience with Just One Gadget</u></a></li>
</ul></div>

