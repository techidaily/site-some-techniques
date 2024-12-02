---
title: Effective Techniques to Minimize or Remove Taskbar Visibility on Windows 10 Systems
date: 2024-11-25T06:49:00.092Z
updated: 2024-12-01T21:55:57.608Z
tags:
  - deals
categories:
  - tech
thumbnail: https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/feature-image.jpg
---

## Effective Techniques to Minimize or Remove Taskbar Visibility on Windows 10 Systems

### Quick Links

* [Automatically Hide the Taskbar in Settings](https://screen-video-capture.techidaily.com/new-2024-approved-capturing-every-moment-with-switch-hd-tech/)
* [Automatically Hide the Taskbar Using Command Prompt](https://instagram-videos.techidaily.com/updated-in-2024-achieve-flawless-video-for-instagram-perfection/)
* [Hide Taskbar with a PowerShell Command](https://some-techniques.techidaily.com/updated-excellence-in-video-selecting-peak-frame-rates-for-slow-motion-effects/)

### Key Takeaways

* You can save screen space by automatically hiding the taskbar on Windows 10.
* To hide the taskbar, right-click empty space on your desktop, then go to Personalization > Taskbar, and enable the toggle next to "Automatically Hide."
* Alternatively, you can use the Command Prompt or PowerShell to toggle the auto-hide option.

 The [Windows taskbar](https://remote-screen-capture.techidaily.com/updated-your-essential-guide-to-unmissable-gaming-adventures-for-2024/) is great for quickly accessing frequently used applications on your computer. However, some users prefer to hide it in order to save screen space. Here's how to hide the taskbar on Windows 10.

##  Automatically Hide the Taskbar in Settings

 To automatically hide your taskbar, right-click anywhere on your PC's desktop and select "Personalize" from the pop-up menu.

![Right-click empty space on your desktop, then select 'Personalize.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/right-click-personalize.png) 

 The "Settings" window will appear. In the left-hand pane, select "Taskbar." From here, toggle the slider to "On" under "Automatically Hide The Taskbar In Desktop Mode." If your PC is able to switch over to tablet mode, you can hide the taskbar by toggling that option to "On," as well.

![Select the 'Taskbar' tab, then enable 'Automatically hide the taskbar in desktop mode' and 'automatically hide the taskbar in tablet mode.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/taskbar-settings.png) 

 You can also right-click the taskbar and select "Taskbar Settings" to access the same Settings window, if you prefer that.

![Right-click the taskbar, then select 'Taskbar Settings.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/taskbar-settings-on-taskbar.png) 

 Your taskbar will now automatically hide. This means that, unless you get a notification from an app in the taskbar or you hover your mouse over where the taskbar should be, it won't show up.

**![GIF showing the taskbar auto hiding](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/06/GIF-showing-the-taskbar-auto-hiding.gif)** 

 You can undo these settings by toggling the sliders back to the "Off" position.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/cKRBWf1EDZo?si=CTNd4q450biit4eM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Automatically Hide the Taskbar Using Command Prompt

 If you're feeling like a hacker, you can also toggle the auto-hide option between on and off by running [commands using the Command Prompt](https://some-knowledge.techidaily.com/how-to-leverage-slug-lines-in-articles-for-2024/).

 First, [open the Command Prompt](https://android-frp.techidaily.com/in-2024-step-by-step-tutorial-how-to-bypass-oppo-a78-frp-by-drfone-android/) by typing "command prompt" in the Windows Search bar and then select the "Command Prompt" app from the search results.

![Search 'command prompt' in the Start menu search, then open the result.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/run-command-prompt.png) 

 In Command Prompt, run this command to toggle the taskbar automatically hide option to on:

powershell -command "&{$p='HKCU:SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\StuckRects3';$v=(Get-ItemProperty -Path $p).Settings;$v[8]=3;&Set-ItemProperty -Path $p -Name Settings -Value $v;&Stop-Process -f -ProcessName explorer}"

![toggle autohide option to on from command prompt](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/06/toggle-autohide-option-to-on-from-command-prompt.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/y3VlwHTQQMs?si=BXYwD1pKiaTuev4y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 And to toggle the taskbar auto-hide option to off, run this command:

powershell -command "&{$p='HKCU:SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\StuckRects3';$v=(Get-ItemProperty -Path $p).Settings;$v[8]=2;&Set-ItemProperty -Path $p -Name Settings -Value $v;&Stop-Process -f -ProcessName explorer}"

![toggle autohide option to off from command prompt](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/06/toggle-autohide-option-to-off-from-command-prompt.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/-0Ww1YIIUe4?si=cQ-Gkh9UCJABuPZU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/3koT_-kvbks?si=sQV7FzPiz6GYITrE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Hide Taskbar with a PowerShell Command

 You may have noticed that the command we used in Command Prompt actually invoked PowerShell first. You can skip the middleman and just run it with PowerShell directly, if you want.

 Search for "PowerShell" in the Start menu search, then launch it. It doesn't need to be run as administrator, but it won't hurt anything if you do.

![Search for 'powershell' in the Start menu search bar, then click "Open' or 'Run as Administrator.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/launch-powershell.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/NC0rdKEQ98o?si=HYgqC8CxF_WTO5if" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 To auto-hide your taskbar, copy and paste the following command into PowerShell:

$p='HKCU:SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\StuckRects3';$v=(Get-ItemProperty -Path $p).Settings;$v[8]=3;&Set-ItemProperty -Path $p -Name Settings -Value $v;&Stop-Process -f -ProcessName explorer

![The command to auto-hide the taskbar in PowerShell.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/powershell-command.png) 

 If you want to re-enable your taskbar, you need to change "$v\[8\]=3" to "$v\[8\]=2" instead. Your complete command will look like this:

$p='HKCU:SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\StuckRects3';$v=(Get-ItemProperty -Path $p).Settings;$v[8]=2;&Set-ItemProperty -Path $p -Name Settings -Value $v;&Stop-Process -f -ProcessName explorer

![Re-enable the taskbar through PowerShell.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/reenable.png) 

 If you just don't like how the taskbar looks, you may want to try [customizing the taskbar](https://remote-screen-capture.techidaily.com/updated-your-essential-guide-to-unmissable-gaming-adventures-for-2024/) instead of hiding it. There are even third-party apps, like [Start11](https://www.stardock.com/products/start11/), that give you even more granular control.

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
<li><a href="https://some-techniques.techidaily.com/new-immersive-vr-bicycle-journeys-to-try/"><u>[New] Immersive VR Bicycle Journeys to Try</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/updated-2024-approved-top-10-premium-android-and-pc-compatible-video-editors/"><u>[Updated] 2024 Approved Top 10 Premium Android & PC-Compatible Video Editors</u></a></li>
<li><a href="https://youtube-tips.techidaily.com/ed-2024-approved-understanding-youtubes-privacy-options-for-viewers/"><u>[Updated] 2024 Approved Understanding YouTube's Privacy Options for Viewers</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-hasten-haste-in-videos-with-top-apps-android/"><u>[Updated] Hasten Haste in Videos with Top Apps, Android</u></a></li>
<li><a href="https://extra-tips.techidaily.com/2024-approved-charting-your-course-to-windows-11-compliance/"><u>2024 Approved Charting Your Course to Windows 11 Compliance</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-fostering-an-online-oasis-paving-the-way-for-a-prolific-youtube-presence/"><u>2024 Approved Fostering an Online Oasis Paving the Way for a Prolific Youtube Presence</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-here-is-how-asmr-helps-with-sleep-and-best-asmrtist-recommendation/"><u>2024 Approved Here Is How ASMR Helps with Sleep & Best ASMRtist Recommendation</u></a></li>
<li><a href="https://article-files.techidaily.com/2024-approved-instagram-meets-tiktok-syncing-social-media/"><u>2024 Approved Instagram Meets TikTok Syncing Social Media</u></a></li>
<li><a href="https://win-blog.techidaily.com/a-complete-guide-to-fixing-slow-loading-times-in-rainbow-six-siege/"><u>A Complete Guide to Fixing Slow Loading Times in Rainbow Six Siege</u></a></li>
<li><a href="https://tech-hub.techidaily.com/chatbot-interaction-patterns-for-realistic-discussions/"><u>Chatbot Interaction Patterns for Realistic Discussions</u></a></li>
<li><a href="https://win-amazing.techidaily.com/get-the-latest-free-updates-for-netgear-a6210-drivers-compatible-with-windows-8-and-7-systems/"><u>Get the Latest Free Updates for Netgear A6210 Drivers Compatible with Windows 8 & 7 Systems</u></a></li>
<li><a href="https://some-techniques.techidaily.com/illustrators-playground-navigating-through-top-8-iphone-drawing-tools-for-2024/"><u>Illustrators' Playground Navigating Through Top 8 iPhone Drawing Tools for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-extracting-stills-for-windows-11-video-projects/"><u>In 2024, Extracting Stills for Windows 11 Video Projects</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-flashback-filmmaking-top-tricks-from-80s-vhs-to-enhance-todays-edits/"><u>In 2024, Flashback Filmmaking Top Tricks From 80S VHS to Enhance Today’s Edits</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-flawless-coexistence-of-linktree-and-tiktok-biographies/"><u>In 2024, Flawless Coexistence of Linktree and TikTok Biographies</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-free-srt-translator-showdown-the-best-eight-in-ranking/"><u>In 2024, Free SRT Translator Showdown The Best Eight in Ranking</u></a></li>
<li><a href="https://extra-resources.techidaily.com/innovative-strategies-to-enhance-tiktoks/"><u>Innovative Strategies to Enhance TikToks</u></a></li>
<li><a href="https://techno-recovery.techidaily.com/listen-up-here-are-13-true-crime-stories-to-keep-you-hooked/"><u>Listen Up! Here Are 13 True Crime Stories to Keep You Hooked</u></a></li>
<li><a href="https://location-social.techidaily.com/why-your-whatsapp-location-is-not-updating-and-how-to-fix-on-samsung-galaxy-m34-drfone-by-drfone-virtual-android/"><u>Why Your WhatsApp Location is Not Updating and How to Fix On Samsung Galaxy M34 | Dr.fone</u></a></li>
</ul></div>

