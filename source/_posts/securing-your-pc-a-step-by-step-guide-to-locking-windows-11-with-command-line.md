---
title: "Securing Your PC: A Step-by-Step Guide to Locking Windows 11 with Command Line"
date: 2025-01-27T00:15:27.994Z
updated: 2025-01-29T05:13:56.846Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://thmb.techidaily.com/07cfabd2fe9acb782e30cca8205dc0f557a2c3371dbf02532bc0633c00063d56.jpg
---

## Securing Your PC: A Step-by-Step Guide to Locking Windows 11 with Command Line

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/15TKQ-BOENI?si=Ri4B2AuxAdi0Bglz" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

### Quick Links

* [Lock Your Windows 10 PC Using Command Prompt](https://vp-tips.techidaily.com/new-audiovisual-adaptability-in-free-fire-for-2024/)
* [Set the Lock Screen Timeout Setting Using Command Prompt](https://eaxpv-info.techidaily.com/new-finding-a-different-way-to-naming-your-channel-with-filmora-for-2024/)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/eu4vwlZcMvM?si=4vEczfVU4BUUFP-t" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

### Key Takeaways

* To lock your Windows PC using Command Prompt, run "**Rundll32.exe user32.dll,LockWorkStation"** in the Command Prompt
* To set the lock screen timeout, run "**powercfg.exe /SETACVALUEINDEX SCHEME\_CURRENT SUB\_VIDEO VIDEOCONLOCK <time>"** in Command Prompt as Admin
* Activate the lock screen timeout setting by running "**powercfg.exe /SETACTIVE SCHEME\_CURRENT"** after you set the timeout.

 One of the first rules of cyber security is to always lock your PC before stepping away. While it may not be the quickest way to lock your Windows 10 PC, you can do it using the Command Prompt.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/RBN1gYY5hUs?si=p89CMiMzeJzU0wGu" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Lock Your Windows 10 PC Using Command Prompt

 First, [open the Command Prompt](https://android-frp.techidaily.com/in-2024-step-by-step-tutorial-how-to-bypass-oppo-a78-frp-by-drfone-android/) on your PC by opening the Start menu, typing “cmd” in the Windows Search bar, and then selecting “Command Prompt” from the search results.

![Click the Start button, search for 'cmd,' then open 'Command Prompt.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/1-launch-cmd.png) 

 Command Prompt will now open. Here, run this command to lock your Windows 10 PC.

Rundll32.exe user32.dll,LockWorkStation

![Locking your PC with Command Prompt.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/2-lock-pc-command-prompt.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/-0Ww1YIIUe4?si=cQ-Gkh9UCJABuPZU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Once executed, your PC will be locked. You'll have to sign back in with your PIN, password, or whatever sign-in method you usually use.

##  Set the Lock Screen Timeout Setting Using Command Prompt

 Once you’ve locked your PC, the lock screen will generally be displayed for a certain amount of time before it time outs. You can set the amount of time that needs to pass before timing out using the Command Prompt.

 To do this, you’ll need to [open Command Prompt as an admin](https://screen-mirror.techidaily.com/how-to-screen-mirroring-xiaomi-14-ultra-drfone-by-drfone-android/). Do so by typing “cmd” in the Windows Search bar and then right-clicking “Command Prompt” from the results. Next, select “Run As Administrator” from the menu that appears.

![Launching Command Prompt as admin.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/3-launch-cmd.png) 

 With Command Prompt open, run this command.

powercfg.exe /SETACVALUEINDEX SCHEME_CURRENT SUB_VIDEO VIDEOCONLOCK <time>

 Replace `<time>` with your desired amount of time in seconds. That means if you want to time out the lock screen after two minutes, you’d enter this command:

powercfg.exe /SETACVALUEINDEX SCHEME_CURRENT SUB_VIDEO VIDEOCONLOCK 120

![Change the timeout to 120.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/4-changing-timeout-to-120.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/C3cJe7Wgn6I?si=EckDFML-VJ_2sYz8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://some-techniques.techidaily.com/new-free-lut-heaven-the-10-finest-and-accessible-resources/"><u>[New] Free LUT Heaven The 10 Finest and Accessible Resources</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-imagememe-magic-instant-jokes/"><u>[New] ImageMeme Magic Instant Jokes</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-expert-analysis-of-sonys-high-definition-video-gear/"><u>[Updated] Expert Analysis of Sony's High-Definition Video Gear</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-harnessing-the-full-spectrum-of-vsco-filters/"><u>[Updated] Harnessing the Full Spectrum of VSCO Filters</u></a></li>
<li><a href="https://win-data.techidaily.com/comment-utiliser-tutosysprep-avec-windows-et-pour-preparer-et-diffuser-des-images-systeme-une-methode-optimale/"><u>Comment Utiliser TutoSysprep Avec Windows eT Pour Préparer Et Diffuser Des Images Système : Une Méthode Optimale</u></a></li>
<li><a href="https://win-amazing.techidaily.com/download-and-install-the-latest-amd-radeon-rx-590-drivers-on-your-pc/"><u>Download & Install the Latest AMD Radeon RX 590 Drivers on Your PC</u></a></li>
<li><a href="https://tech-hub.techidaily.com/empower-your-wrist-tech-discover-chatgpts-revolutionary-effects-on-smartwatches/"><u>Empower Your Wrist Tech: Discover ChatGPT's Revolutionary Effects on Smartwatches</u></a></li>
<li><a href="https://some-techniques.techidaily.com/expert-recommended-steadicams-for-professional-dslr-work-for-2024/"><u>Expert-Recommended Steadicams for Professional DSLR Work for 2024</u></a></li>
<li><a href="https://facebook.techidaily.com/from-scrolling-to-serenity-the-top-10-reasons-to-leave-the-facebook-journey/"><u>From Scrolling to Serenity: The Top 10 Reasons to Leave the Facebook Journey</u></a></li>
<li><a href="https://review-topics.techidaily.com/in-2024-full-guide-to-fix-itoolab-anygo-not-working-on-vivo-t2-pro-5g-drfone-by-drfone-virtual-android/"><u>In 2024, Full Guide to Fix iToolab AnyGO Not Working On Vivo T2 Pro 5G | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-fundamentals-of-narrative-crafting/"><u>In 2024, Fundamentals of Narrative Crafting</u></a></li>
<li><a href="https://fox-cloud.techidaily.com/mastering-object-extraction-in-iphone-photography-with-top-6-apps-for-2024/"><u>Mastering Object Extraction in iPhone Photography with Top 6 Apps for 2024</u></a></li>
<li><a href="https://tech-revival.techidaily.com/not-just-a-phase-disproving-global-cooling-claims/"><u>Not Just a Phase: Disproving Global Cooling Claims</u></a></li>
<li><a href="https://extra-resources.techidaily.com/the-leading-list-for-best-vector-resources/"><u>The Leading List for Best Vector Resources</u></a></li>
<li><a href="https://extra-lessons.techidaily.com/the-ultimate-meme-playbook-no-10-essentials/"><u>The Ultimate Meme Playbook No. 10 Essentials</u></a></li>
</ul></div>

