---
title: "Securing Your PC: A Step-by-Step Guide to Locking Windows 11 with Command Line"
date: 2024-11-17T19:03:20.685Z
updated: 2024-11-23T17:28:19.503Z
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/uV3vm805eX0?si=YSPcsFxBcJmoxLsU&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

### Key Takeaways

* To lock your Windows PC using Command Prompt, run "**Rundll32.exe user32.dll,LockWorkStation"** in the Command Prompt
* To set the lock screen timeout, run "**powercfg.exe /SETACVALUEINDEX SCHEME\_CURRENT SUB\_VIDEO VIDEOCONLOCK <time>"** in Command Prompt as Admin
* Activate the lock screen timeout setting by running "**powercfg.exe /SETACTIVE SCHEME\_CURRENT"** after you set the timeout.

 One of the first rules of cyber security is to always lock your PC before stepping away. While it may not be the quickest way to lock your Windows 10 PC, you can do it using the Command Prompt.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/YezPJZzPJ8Q?si=xF1t4BQHFquzvnzE&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Lock Your Windows 10 PC Using Command Prompt

 First, [open the Command Prompt](https://android-frp.techidaily.com/in-2024-step-by-step-tutorial-how-to-bypass-oppo-a78-frp-by-drfone-android/) on your PC by opening the Start menu, typing “cmd” in the Windows Search bar, and then selecting “Command Prompt” from the search results.

![Click the Start button, search for 'cmd,' then open 'Command Prompt.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/1-launch-cmd.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/6xGqSETroqA?si=4C1GPgXi-AksR_oO&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Command Prompt will now open. Here, run this command to lock your Windows 10 PC.

Rundll32.exe user32.dll,LockWorkStation

![Locking your PC with Command Prompt.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/2-lock-pc-command-prompt.png) 

 Once executed, your PC will be locked. You'll have to sign back in with your PIN, password, or whatever sign-in method you usually use.

##  Set the Lock Screen Timeout Setting Using Command Prompt

 Once you’ve locked your PC, the lock screen will generally be displayed for a certain amount of time before it time outs. You can set the amount of time that needs to pass before timing out using the Command Prompt.

 To do this, you’ll need to [open Command Prompt as an admin](https://screen-mirror.techidaily.com/how-to-screen-mirroring-xiaomi-14-ultra-drfone-by-drfone-android/). Do so by typing “cmd” in the Windows Search bar and then right-clicking “Command Prompt” from the results. Next, select “Run As Administrator” from the menu that appears.

![Launching Command Prompt as admin.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/3-launch-cmd.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/2NU63YqpVqw?si=uoJs0-nZYAkILqXx&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 With Command Prompt open, run this command.

powercfg.exe /SETACVALUEINDEX SCHEME_CURRENT SUB_VIDEO VIDEOCONLOCK <time>

 Replace `<time>` with your desired amount of time in seconds. That means if you want to time out the lock screen after two minutes, you’d enter this command:

powercfg.exe /SETACVALUEINDEX SCHEME_CURRENT SUB_VIDEO VIDEOCONLOCK 120

![Change the timeout to 120.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/4-changing-timeout-to-120.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/-0Ww1YIIUe4?si=cQ-Gkh9UCJABuPZU&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://some-techniques.techidaily.com/new-explore-free-online-music-beat-detection-tools/"><u>[New] Explore Free Online Music Beat Detection Tools</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-ideal-3d-software-for-creating-animation/"><u>[New] Ideal 3D Software for Creating Animation</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/new-instagram-selfie-verification-everything-you-need-to-know/"><u>[New] Instagram Selfie Verification - Everything You Need to Know</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-how-to-make-collage-for-facebook-instantly/"><u>[Updated] How to Make Collage for Facebook Instantly</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-from-idea-to-gif-your-ultimate-blueprint/"><u>2024 Approved From Idea to GIF Your Ultimate Blueprint</u></a></li>
<li><a href="https://some-skills.techidaily.com/2024-approved-unlocking-sierras-icloud-drives-for-all-access/"><u>2024 Approved Unlocking Sierra's iCloud Drives for All-Access</u></a></li>
<li><a href="https://buynow-info.techidaily.com/comprehensive-assessment-of-the-latest-iphone-13-features/"><u>Comprehensive Assessment of the Latest iPhone 13 Features</u></a></li>
<li><a href="https://unlock-android.techidaily.com/everything-you-need-to-know-about-lock-screen-settings-on-your-vivo-y200e-5g-by-drfone-android/"><u>Everything You Need to Know about Lock Screen Settings on your Vivo Y200e 5G</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/explodierende-popularitat-von-freemium-ai-tools-die-funf-besten-programme-zur-wiederherstellung-ihrer-alten-fotos-finden-sie-hier/"><u>Explodierende Popularität Von Freemium AI-Tools - Die Fünf Besten Programme Zur Wiederherstellung Ihrer Alten Fotos Finden Sie Hier!</u></a></li>
<li><a href="https://android-frp.techidaily.com/hassle-free-ways-to-remove-frp-lock-on-meizuwithwithout-a-pc-by-drfone-android/"><u>Hassle-Free Ways to Remove FRP Lock on Meizuwith/without a PC</u></a></li>
<li><a href="https://location-social.techidaily.com/in-2024-3-things-you-must-know-about-fake-snapchat-location-on-xiaomi-14-pro-drfone-by-drfone-virtual-android/"><u>In 2024, 3 Things You Must Know about Fake Snapchat Location On Xiaomi 14 Pro | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-from-obscurity-to-fame-elevate-your-tiktok-unboxing-videos/"><u>In 2024, From Obscurity to Fame Elevate Your TikTok Unboxing Videos</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-how-to-effortlessly-blur-images-captured-by-iphones-4-methods/"><u>In 2024, How to Effortlessly Blur Images Captured by iPhones (4 Methods)</u></a></li>
<li><a href="https://android-location-track.techidaily.com/in-2024-how-to-spy-on-text-messages-from-computer-and-realme-12-pro-5g-drfone-by-drfone-virtual-android/"><u>In 2024, How to Spy on Text Messages from Computer & Realme 12 Pro 5G | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-innovate-in-note-taking-with-mematic-platform/"><u>In 2024, Innovate in Note-Taking with Mematic Platform</u></a></li>
<li><a href="https://extra-hints.techidaily.com/top-7-affordable-4k-mirrorless-cameras-(1000/"><u>Top 7 Affordable 4K Mirrorless Cameras <$1,000</u></a></li>
</ul></div>

