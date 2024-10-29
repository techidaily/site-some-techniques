---
title: "Securing Your PC: A Step-by-Step Guide to Locking Windows 11 with Command Line"
date: 2024-10-24T16:36:59.726Z
updated: 2024-10-29T17:41:48.326Z
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

<!-- affiliate ads begin -->
<a href="https://25home.pxf.io/c/5597632/2148640/16836" target="_top" id="2148640">
  <img src="//a.impactradius-go.com/display-ad/16836-2148640" border="0" alt="https://techidaily.com" width="234" height="60"/>
</a>
<img height="0" width="0" src="https://25home.pxf.io/i/5597632/2148640/16836" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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

<!-- affiliate ads begin -->
<a href="https://zebaoaffiliateprogram.pxf.io/c/5597632/2137973/21526" target="_top" id="2137973">
  <img src="//a.impactradius-go.com/display-ad/21526-2137973" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://zebaoaffiliateprogram.pxf.io/i/5597632/2137973/21526" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Once executed, your PC will be locked. You'll have to sign back in with your PIN, password, or whatever sign-in method you usually use.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2037355/7443" target="_top" id="2037355">
  <img src="//a.impactradius-go.com/display-ad/7443-2037355" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2037355/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Set the Lock Screen Timeout Setting Using Command Prompt

 Once you’ve locked your PC, the lock screen will generally be displayed for a certain amount of time before it time outs. You can set the amount of time that needs to pass before timing out using the Command Prompt.

 To do this, you’ll need to [open Command Prompt as an admin](https://screen-mirror.techidaily.com/how-to-screen-mirroring-xiaomi-14-ultra-drfone-by-drfone-android/). Do so by typing “cmd” in the Windows Search bar and then right-clicking “Command Prompt” from the results. Next, select “Run As Administrator” from the menu that appears.

![Launching Command Prompt as admin.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/3-launch-cmd.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1997657/19272" target="_top" id="1997657">
  <img src="//a.impactradius-go.com/display-ad/19272-1997657" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1997657/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 With Command Prompt open, run this command.

powercfg.exe /SETACVALUEINDEX SCHEME_CURRENT SUB_VIDEO VIDEOCONLOCK <time>

 Replace `<time>` with your desired amount of time in seconds. That means if you want to time out the lock screen after two minutes, you’d enter this command:

powercfg.exe /SETACVALUEINDEX SCHEME_CURRENT SUB_VIDEO VIDEOCONLOCK 120

![Change the timeout to 120.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/4-changing-timeout-to-120.png) 

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
<li><a href="https://some-techniques.techidaily.com/new-expert-techniques-for-transforming-mp4-files-with-vlc/"><u>[New] Expert Techniques for Transforming MP4 Files with VLC</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-exploring-hololens-by-microsoft-a-3d-dream-come-true/"><u>[New] Exploring HoloLens by Microsoft A 3D Dream Come True</u></a></li>
<li><a href="https://youtube-tips.techidaily.com/our-pathway-to-a-clutter-free-device-with-video-deletion-tips-for-2024/"><u>[New] Your Pathway to a Clutter-Free Device with Video Deletion Tips for 2024</u></a></li>
<li><a href="https://article-posts.techidaily.com/updated-2024-approved-colors-unveiled-the-comprehensive-tutorial/"><u>[Updated] 2024 Approved Colors Unveiled The Comprehensive Tutorial</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-from-shopping-spree-to-stardom-editing-your-haul-video/"><u>2024 Approved From Shopping Spree to Stardom Editing Your Haul Video</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-funimate-masterclass-gameplay-enhancement/"><u>2024 Approved Funimate Masterclass Gameplay Enhancement</u></a></li>
<li><a href="https://howto.techidaily.com/android-screen-stuck-general-nokia-105-classic-partly-screen-unresponsive-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>Android Screen Stuck General Nokia 105 Classic Partly Screen Unresponsive | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/free-and-paid-iphone-photo-experience-top-app-lineup-for-2024/"><u>Free & Paid iPhone Photo Experience - Top App Lineup for 2024</u></a></li>
<li><a href="https://youtube-clips.techidaily.com/harnessing-ambiance-with-thoughtful-lighting/"><u>Harnessing Ambiance with Thoughtful Lighting</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-innovating-with-iphone-for-complete-360-video-capture/"><u>In 2024, Innovating with iPhone for Complete 360 Video Capture</u></a></li>
<li><a href="https://ios-unlock.techidaily.com/in-2024-iphone-is-disabled-here-is-the-way-to-unlock-disabled-apple-iphone-12-by-drfone-ios/"><u>In 2024, iPhone Is Disabled? Here Is The Way To Unlock Disabled Apple iPhone 12</u></a></li>
<li><a href="https://activate-lock.techidaily.com/in-2024-the-10-best-tools-to-bypass-icloud-activation-lock-on-apple-iphone-se-you-should-try-out-by-drfone-ios/"><u>In 2024, The 10 Best Tools to Bypass iCloud Activation Lock On Apple iPhone SE You Should Try Out</u></a></li>
<li><a href="https://android-unlock.techidaily.com/the-ultimate-guide-to-meizu-pattern-lock-screen-everything-you-need-to-know-by-drfone-android/"><u>The Ultimate Guide to Meizu Pattern Lock Screen Everything You Need to Know</u></a></li>
<li><a href="https://discover-brilliant.techidaily.com/verstandnis-von-4k-ultra-hd-video-die-vollstandige-anleitung/"><u>Verständnis Von 4K Ultra HD-Video: Die Vollständige Anleitung</u></a></li>
</ul></div>

