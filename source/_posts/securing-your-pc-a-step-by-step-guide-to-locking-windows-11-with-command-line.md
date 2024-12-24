---
title: "Securing Your PC: A Step-by-Step Guide to Locking Windows 11 with Command Line"
date: 2024-12-17T18:38:56.332Z
updated: 2024-12-24T21:12:04.533Z
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/XS1nQCe95LU?si=A2dhdFkSAI61_nKA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

### Key Takeaways

* To lock your Windows PC using Command Prompt, run "**Rundll32.exe user32.dll,LockWorkStation"** in the Command Prompt
* To set the lock screen timeout, run "**powercfg.exe /SETACVALUEINDEX SCHEME\_CURRENT SUB\_VIDEO VIDEOCONLOCK <time>"** in Command Prompt as Admin
* Activate the lock screen timeout setting by running "**powercfg.exe /SETACTIVE SCHEME\_CURRENT"** after you set the timeout.

 One of the first rules of cyber security is to always lock your PC before stepping away. While it may not be the quickest way to lock your Windows 10 PC, you can do it using the Command Prompt.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/PKZUYice-ws?si=L8iMa9T3h7TMSWdQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Lock Your Windows 10 PC Using Command Prompt

 First, [open the Command Prompt](https://android-frp.techidaily.com/in-2024-step-by-step-tutorial-how-to-bypass-oppo-a78-frp-by-drfone-android/) on your PC by opening the Start menu, typing “cmd” in the Windows Search bar, and then selecting “Command Prompt” from the search results.

![Click the Start button, search for 'cmd,' then open 'Command Prompt.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/1-launch-cmd.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/4YCkNXJjC3c?si=9Tn8KiqKGTZi1o7E" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Command Prompt will now open. Here, run this command to lock your Windows 10 PC.

Rundll32.exe user32.dll,LockWorkStation

![Locking your PC with Command Prompt.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/2-lock-pc-command-prompt.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/YwOwUI47FuU?si=NK7IEELjx7_SJSl2" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Once executed, your PC will be locked. You'll have to sign back in with your PIN, password, or whatever sign-in method you usually use.

##  Set the Lock Screen Timeout Setting Using Command Prompt

 Once you’ve locked your PC, the lock screen will generally be displayed for a certain amount of time before it time outs. You can set the amount of time that needs to pass before timing out using the Command Prompt.

 To do this, you’ll need to [open Command Prompt as an admin](https://screen-mirror.techidaily.com/how-to-screen-mirroring-xiaomi-14-ultra-drfone-by-drfone-android/). Do so by typing “cmd” in the Windows Search bar and then right-clicking “Command Prompt” from the results. Next, select “Run As Administrator” from the menu that appears.

![Launching Command Prompt as admin.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/3-launch-cmd.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/RJNYTGHVlLc?si=heERQcpMi77lqToE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://visual-screen-recording.techidaily.com/new-in-2024-top-mac-frame-freezes-collection-limit-156-chars/"><u>[New] In 2024, Top Mac Frame Freezes Collection (Limit 156 Chars)</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-excellence-on-the-screen-best-six-video-tools-for-big-sur/"><u>[Updated] Excellence on the Screen Best Six Video Tools for Big Sur</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-explore-the-10-finest-iphone-photo-editors-and-filters/"><u>[Updated] Explore the 10 Finest iPhone Photo Editors & Filters</u></a></li>
<li><a href="https://article-files.techidaily.com/updated-master-windows-11-a-treasure-trove-of-undisclosed-features-for-2024/"><u>[Updated] Master Windows 11 A Treasure Trove of Undisclosed Features for 2024</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/updated-maximizing-zoom-video-details-step-by-step-methods/"><u>[Updated] Maximizing Zoom Video Details Step-by-Step Methods</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/2024-approved-the-secret-to-slowed-movies-mastery-your-step-by-step-guide-on-instagram-reels/"><u>2024 Approved The Secret to Slowed Movies Mastery – Your Step by Step Guide on Instagram Reels</u></a></li>
<li><a href="https://some-techniques.techidaily.com/free-efficient-translation-the-top-8-best-apps-reviewed-for-2024/"><u>Free, Efficient Translation The Top 8 Best Apps Reviewed for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-how-to-smoothly-add-apods-episodes-on-devices/"><u>In 2024, How to Smoothly Add APods Episodes on Devices</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/in-2024-innovative-venues-for-immersive-media/"><u>In 2024, Innovative Venues for Immersive Media</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-top-10-final-cut-pro-plug-ins/"><u>In 2024, Top 10 Final Cut Pro Plug-Ins</u></a></li>
<li><a href="https://fox-links.techidaily.com/leveraging-length-and-style-in-your-instagram-videos-for-2024/"><u>Leveraging Length and Style in Your Instagram Videos for 2024</u></a></li>
<li><a href="https://technical-tips.techidaily.com/messenger-made-accessible-joining-conversations-even-if-you-dont-use-facebook/"><u>Messenger Made Accessible: Joining Conversations Even if You Don't Use Facebook</u></a></li>
<li><a href="https://blog-min.techidaily.com/quick-and-easy-guide-to-moving-videos-onto-an-ipad-top-strategies/"><u>Quick and Easy Guide to Moving Videos Onto an iPad – Top Strategies</u></a></li>
<li><a href="https://fake-location.techidaily.com/spoofing-life360-how-to-do-it-on-motorola-moto-g14-drfone-by-drfone-virtual-android/"><u>Spoofing Life360 How to Do it on Motorola Moto G14? | Dr.fone</u></a></li>
</ul></div>

