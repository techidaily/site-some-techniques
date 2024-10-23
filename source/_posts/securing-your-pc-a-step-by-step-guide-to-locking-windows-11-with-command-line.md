---
title: "Securing Your PC: A Step-by-Step Guide to Locking Windows 11 with Command Line"
date: 2024-10-18T19:56:31.018Z
updated: 2024-10-23T16:57:20.225Z
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
<a href="https://aligracehair.sjv.io/c/5597632/1975816/19272" target="_top" id="1975816">
  <img src="//a.impactradius-go.com/display-ad/19272-1975816" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1975816/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Lock Your Windows 10 PC Using Command Prompt

 First, [open the Command Prompt](https://android-frp.techidaily.com/in-2024-step-by-step-tutorial-how-to-bypass-oppo-a78-frp-by-drfone-android/) on your PC by opening the Start menu, typing “cmd” in the Windows Search bar, and then selecting “Command Prompt” from the search results.

![Click the Start button, search for 'cmd,' then open 'Command Prompt.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/1-launch-cmd.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2012420/19272" target="_top" id="2012420">
  <img src="//a.impactradius-go.com/display-ad/19272-2012420" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2012420/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Command Prompt will now open. Here, run this command to lock your Windows 10 PC.

Rundll32.exe user32.dll,LockWorkStation

![Locking your PC with Command Prompt.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/2-lock-pc-command-prompt.png) 

 Once executed, your PC will be locked. You'll have to sign back in with your PIN, password, or whatever sign-in method you usually use.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1934258/19272" target="_top" id="1934258">
  <img src="//a.impactradius-go.com/display-ad/19272-1934258" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1934258/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Set the Lock Screen Timeout Setting Using Command Prompt

 Once you’ve locked your PC, the lock screen will generally be displayed for a certain amount of time before it time outs. You can set the amount of time that needs to pass before timing out using the Command Prompt.

 To do this, you’ll need to [open Command Prompt as an admin](https://screen-mirror.techidaily.com/how-to-screen-mirroring-xiaomi-14-ultra-drfone-by-drfone-android/). Do so by typing “cmd” in the Windows Search bar and then right-clicking “Command Prompt” from the results. Next, select “Run As Administrator” from the menu that appears.

![Launching Command Prompt as admin.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/3-launch-cmd.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2037356/7443" target="_top" id="2037356">
  <img src="//a.impactradius-go.com/display-ad/7443-2037356" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2037356/7443" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://youtube-docs.techidaily.com/024-approved-vimeo-and-youtube-the-ultimate-showdown/"><u>[New] 2024 Approved Vimeo and YouTube The Ultimate Showdown</u></a></li>
<li><a href="https://remote-screen-capture.techidaily.com/new-prime-video-cameras-that-will-elevate-your-twitch-channel-for-2024/"><u>[New] Prime Video Cameras That Will Elevate Your Twitch Channel for 2024</u></a></li>
<li><a href="https://fox-helps.techidaily.com/updated-2024-approved-ultimate-image-booster-intense-visual-upgrade/"><u>[Updated] 2024 Approved Ultimate Image Booster Intense Visual Upgrade</u></a></li>
<li><a href="https://youtube-tips.techidaily.com/ed-in-2024-youtube-subscriber-chart-5-most-subscribed-youtuber/"><u>[Updated] In 2024, YouTube Subscriber Chart - 5 Most Subscribed YouTuber</u></a></li>
<li><a href="https://some-skills.techidaily.com/updated-the-ultimate-guide-stop-snippet-playback-on-youtube/"><u>[Updated] The Ultimate Guide Stop Snippet Playback on YouTube</u></a></li>
<li><a href="https://some-approaches.techidaily.com/1726027504838-7/"><u>「静止画を創造的な動画に生まれ変わらせる:最新の7つのツールベストセレクション」</u></a></li>
<li><a href="https://win-webster.techidaily.com/complete-step-by-step-tutorial-retrieve-deleted-items-from-palworld/"><u>Complete Step-by-Step Tutorial: Retrieve Deleted Items From Palworld</u></a></li>
<li><a href="https://fake-location.techidaily.com/in-2024-5-hassle-free-solutions-to-fake-location-on-find-my-friends-of-oneplus-nord-ce-3-5g-drfone-by-drfone-virtual-android/"><u>In 2024, 5 Hassle-Free Solutions to Fake Location on Find My Friends Of OnePlus Nord CE 3 5G | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/troubleshooting-breakdown-of-preinstalled-applications-in-specific-windows-11-machines/"><u>Troubleshooting Breakdown of Preinstalled Applications in Specific Windows 11 Machines</u></a></li>
<li><a href="https://some-techniques.techidaily.com/troubleshooting-guide-why-wont-my-new-ssd-appear-on-windows-discover-solutions/"><u>Troubleshooting Guide: Why Won't My New SSD Appear on Windows? Discover Solutions</u></a></li>
<li><a href="https://some-techniques.techidaily.com/ubuntu-tips-concealing-taskbar-and-launcher-a-comprehensive-guide/"><u>Ubuntu Tips: Concealing Taskbar & Launcher - A Comprehensive Guide</u></a></li>
<li><a href="https://some-techniques.techidaily.com/understanding-quicktime-player-a-comprehensive-guide/"><u>Understanding QuickTime Player: A Comprehensive Guide</u></a></li>
<li><a href="https://some-techniques.techidaily.com/understanding-the-role-of-ntuserdat-in-windows-systems/"><u>Understanding the Role of NTUSER.DAT in Windows Systems</u></a></li>
<li><a href="https://some-techniques.techidaily.com/upgrade-now-secure-your-windows-11-professional-copy-with-a-staggering-87-savings-opportunity/"><u>Upgrade Now: Secure Your Windows 11 Professional Copy with a Staggering 87% Savings Opportunity!</u></a></li>
<li><a href="https://fox-cloud.techidaily.com/visual-impact-techniques-for-warped-image-content-for-2024/"><u>Visual Impact Techniques for Warped Image Content for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/why-microsofts-upscaler-is-essential-the-key-attraction-of-upgrading-to-a-copilotplus-gaming-pc/"><u>Why Microsoft's Upscaler Is Essential: The Key Attraction of Upgrading to a CoPilot+ Gaming PC</u></a></li>
</ul></div>

