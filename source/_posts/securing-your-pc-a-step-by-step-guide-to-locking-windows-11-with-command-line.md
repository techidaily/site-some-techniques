---
title: "Securing Your PC: A Step-by-Step Guide to Locking Windows 11 with Command Line"
date: 2025-01-13T16:27:52.089Z
updated: 2025-01-15T16:17:02.146Z
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/RBN1gYY5hUs?si=p89CMiMzeJzU0wGu" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

### Key Takeaways

* To lock your Windows PC using Command Prompt, run "**Rundll32.exe user32.dll,LockWorkStation"** in the Command Prompt
* To set the lock screen timeout, run "**powercfg.exe /SETACVALUEINDEX SCHEME\_CURRENT SUB\_VIDEO VIDEOCONLOCK <time>"** in Command Prompt as Admin
* Activate the lock screen timeout setting by running "**powercfg.exe /SETACTIVE SCHEME\_CURRENT"** after you set the timeout.

 One of the first rules of cyber security is to always lock your PC before stepping away. While it may not be the quickest way to lock your Windows 10 PC, you can do it using the Command Prompt.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/-yZKNLxj3po?si=-RbF6nCJEVlHWP-M" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Lock Your Windows 10 PC Using Command Prompt

 First, [open the Command Prompt](https://android-frp.techidaily.com/in-2024-step-by-step-tutorial-how-to-bypass-oppo-a78-frp-by-drfone-android/) on your PC by opening the Start menu, typing “cmd” in the Windows Search bar, and then selecting “Command Prompt” from the search results.

![Click the Start button, search for 'cmd,' then open 'Command Prompt.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/1-launch-cmd.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/O7ChChlyX2o?si=7pMKdN1NZig1kYek" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Command Prompt will now open. Here, run this command to lock your Windows 10 PC.

Rundll32.exe user32.dll,LockWorkStation

![Locking your PC with Command Prompt.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/2-lock-pc-command-prompt.png) 

 Once executed, your PC will be locked. You'll have to sign back in with your PIN, password, or whatever sign-in method you usually use.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/nWu29cqFjZA?si=TNZyCbPq68PQ0JIb" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/DBMTAJBx-X4?si=sje5pFJXiHzJJGbP" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://facebook-video-share.techidaily.com/new-android-audio-alchemy-selecting-the-top-free-downloader-apps-from-youtube-for-2024/"><u>[New] Android Audio Alchemy Selecting the Top Free Downloader Apps From YouTube for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-fostering-friendship-through-conversations-with-viewers/"><u>[New] Fostering Friendship Through Conversations With Viewers</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-from-camera-to-feed-ig-photo-tutorial/"><u>[New] From Camera to Feed IG Photo Tutorial</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-hacks-for-hassle-free-podcast-streaming/"><u>[New] Hacks for Hassle-Free Podcast Streaming</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/new-in-2024-mastering-the-art-of-secretive-insta-story-consumption/"><u>[New] In 2024, Mastering the Art of Secretive Insta Story Consumption</u></a></li>
<li><a href="https://facebook-video-footage.techidaily.com/updated-in-2024-cutting-edge-techniques-for-private-yt-content-dissemination-in-gmail/"><u>[Updated] In 2024, Cutting-Edge Techniques for Private YT Content Dissemination in Gmail</u></a></li>
<li><a href="https://apple-account.techidaily.com/apple-id-locked-for-security-reasons-on-apple-iphone-14-find-the-best-solution-here-by-drfone-ios/"><u>Apple ID Locked for Security Reasons On Apple iPhone 14? Find the Best Solution Here</u></a></li>
<li><a href="https://blue-screen-error.techidaily.com/fixing-the-failed-hardware-abstraction-layer-hal-start-up-issue-in-windows-10/"><u>Fixing the Failed Hardware Abstraction Layer (HAL) Start-Up Issue in Windows 10</u></a></li>
<li><a href="https://some-techniques.techidaily.com/gopro-time-lapse-tips-create-epic-time-lapse-video-for-2024/"><u>GoPro Time Lapse Tips Create Epic Time Lapse Video for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/grasping-the-heart-of-narrative-design-for-2024/"><u>Grasping the Heart of Narrative Design for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-expert-tips-the-finest-7-wet-proof-recorders/"><u>In 2024, Expert Tips The Finest 7 Wet-Proof Recorders</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-fine-tune-viewing-the-ultimate-zoom-journey/"><u>In 2024, Fine-Tune Viewing The Ultimate Zoom Journey</u></a></li>
<li><a href="https://smart-video-creator.techidaily.com/new-ditch-final-cut-pro-x-10-free-and-paid-alternatives-to-consider-for-2024/"><u>New Ditch Final Cut Pro X? 10 Free and Paid Alternatives to Consider for 2024</u></a></li>
<li><a href="https://fox-place.techidaily.com/onedrive-windows/"><u>OneDriveの自動更新とファイル同期 - Windows環境で</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/understanding-user-choices-customizing-your-experience/"><u>Understanding User Choices: Customizing Your Experience</u></a></li>
</ul></div>

