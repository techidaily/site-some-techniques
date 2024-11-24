---
title: Effective Techniques to Minimize or Remove Taskbar Visibility on Windows 10 Systems
date: 2024-11-19T21:27:42.338Z
updated: 2024-11-23T16:38:25.462Z
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

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/H2cXnI9oOvM?si=3nz2sBB124ln-83T&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 The "Settings" window will appear. In the left-hand pane, select "Taskbar." From here, toggle the slider to "On" under "Automatically Hide The Taskbar In Desktop Mode." If your PC is able to switch over to tablet mode, you can hide the taskbar by toggling that option to "On," as well.

![Select the 'Taskbar' tab, then enable 'Automatically hide the taskbar in desktop mode' and 'automatically hide the taskbar in tablet mode.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/taskbar-settings.png) 

 You can also right-click the taskbar and select "Taskbar Settings" to access the same Settings window, if you prefer that.

![Right-click the taskbar, then select 'Taskbar Settings.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/taskbar-settings-on-taskbar.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/MPoakxUNf9o?si=S-ppSqzHzN9VrxC7&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Your taskbar will now automatically hide. This means that, unless you get a notification from an app in the taskbar or you hover your mouse over where the taskbar should be, it won't show up.

**![GIF showing the taskbar auto hiding](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/06/GIF-showing-the-taskbar-auto-hiding.gif)** 

 You can undo these settings by toggling the sliders back to the "Off" position.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/YwOwUI47FuU?si=NK7IEELjx7_SJSl2&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Automatically Hide the Taskbar Using Command Prompt

 If you're feeling like a hacker, you can also toggle the auto-hide option between on and off by running [commands using the Command Prompt](https://some-knowledge.techidaily.com/how-to-leverage-slug-lines-in-articles-for-2024/).

 First, [open the Command Prompt](https://android-frp.techidaily.com/in-2024-step-by-step-tutorial-how-to-bypass-oppo-a78-frp-by-drfone-android/) by typing "command prompt" in the Windows Search bar and then select the "Command Prompt" app from the search results.

![Search 'command prompt' in the Start menu search, then open the result.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/run-command-prompt.png) 

 In Command Prompt, run this command to toggle the taskbar automatically hide option to on:

powershell -command "&{$p='HKCU:SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\StuckRects3';$v=(Get-ItemProperty -Path $p).Settings;$v[8]=3;&Set-ItemProperty -Path $p -Name Settings -Value $v;&Stop-Process -f -ProcessName explorer}"

![toggle autohide option to on from command prompt](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/06/toggle-autohide-option-to-on-from-command-prompt.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/yr0yS_Ywrjs?si=QxzYiX1KmUaExmlo&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 And to toggle the taskbar auto-hide option to off, run this command:

powershell -command "&{$p='HKCU:SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\StuckRects3';$v=(Get-ItemProperty -Path $p).Settings;$v[8]=2;&Set-ItemProperty -Path $p -Name Settings -Value $v;&Stop-Process -f -ProcessName explorer}"

![toggle autohide option to off from command prompt](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/06/toggle-autohide-option-to-off-from-command-prompt.png) 

##  Hide Taskbar with a PowerShell Command

 You may have noticed that the command we used in Command Prompt actually invoked PowerShell first. You can skip the middleman and just run it with PowerShell directly, if you want.

 Search for "PowerShell" in the Start menu search, then launch it. It doesn't need to be run as administrator, but it won't hurt anything if you do.

![Search for 'powershell' in the Start menu search bar, then click "Open' or 'Run as Administrator.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/launch-powershell.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/58KlTPHv8dU?si=7ICagyNgrao7OkVO&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://youtube-blog.techidaily.com/024-approved-essential-info-on-crafting-engaging-yt-shorts/"><u>[New] 2024 Approved Essential Info on Crafting Engaging YT Shorts</u></a></li>
<li><a href="https://eaxpv-info.techidaily.com/new-2024-approved-flipping-scripts-generating-parody-content/"><u>[New] 2024 Approved Flipping Scripts Generating Parody Content</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-fundamentals-of-animated-branding/"><u>[New] Fundamentals of Animated Branding</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-how-to-combine-videos-on-iphone/"><u>[New] How to Combine Videos on iPhone</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/updated-how-to-screen-record-netflix-on-mac-for-2024/"><u>[Updated] How to Screen Record Netflix on Mac for 2024</u></a></li>
<li><a href="https://youtube-webster.techidaily.com/ed-in-2024-ecological-architecture-merging-nature-and-city-planning/"><u>[Updated] In 2024, Ecological Architecture Merging Nature and City Planning</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-exploring-next-gen-coding-is-av1-superior-to-vp9/"><u>2024 Approved Exploring Next-Gen Coding Is AV1 Superior to VP9?</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-funnyframefinder-your-source-for-meme-creation-online/"><u>2024 Approved FunnyFrameFinder Your Source for Meme Creation Online</u></a></li>
<li><a href="https://win-tips.techidaily.com/effortless-video-retrieval-from-nbc-sports-with-superior-downloader-app/"><u>Effortless Video Retrieval From NBC Sports with Superior Downloader App</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-foundations-of-easing-volume-control-in-audition/"><u>In 2024, Foundations of Easing Volume Control in Audition</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-garmin-virb-ultra-30-action-camera-review/"><u>In 2024, Garmin VIRB Ultra 30 Action Camera Review</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/maintain-peaceful-posting-dismiss-ig-recommendations/"><u>Maintain Peaceful Posting Dismiss IG Recommendations</u></a></li>
<li><a href="https://fox-access.techidaily.com/the-ultimate-list-of-top-5-iphone-podcast-software/"><u>The Ultimate List of Top 5 iPhone Podcast Software</u></a></li>
<li><a href="https://fake-location.techidaily.com/what-is-fake-gps-location-pro-and-is-it-good-on-oppo-reno-8t-drfone-by-drfone-virtual-android/"><u>What is Fake GPS Location Pro and Is It Good On Oppo Reno 8T? | Dr.fone</u></a></li>
</ul></div>

