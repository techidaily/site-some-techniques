---
title: "Quick Troubleshooting: How to Immediately Close a Frozen Program on Your Windows 10 PC"
date: 2024-10-19T21:58:42.337Z
updated: 2024-10-23T17:12:19.487Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://thmb.techidaily.com/45e28f9a2bd574b9cc2fe65fd885cbbf79b57e7d44fbc8bb793a1cd727c98e95.jpg
---

## Quick Troubleshooting: How to Immediately Close a Frozen Program on Your Windows 10 PC

### Quick Links

* [Try a Keyboard Shortcut](https://instagram-clips.techidaily.com/the-key-to-viral-instagram-posts/)
* [Force Quit Using Task Manager](https://android-unlock.techidaily.com/in-2024-forgot-pattern-lock-heres-how-you-can-unlock-samsung-galaxy-s24-pattern-lock-screen-by-drfone-android/)
* [Force Quit an App Using Command Prompt](https://fox-links.techidaily.com/expertly-crafted-images-with-lut-techniques-in-photoshop-cs6-for-2024/)

### Key Takeaways

* Try pressing Alt+F4 to force-close an app.
* Open Task Manager, select the frozen app, and click "End Task" to force quit it.
* Run "tasklist" in Command Prompt find tasks, and then use "taskkill /im <program>.exe" to force quit the app.

 It’s not uncommon for an application to stop responding on Windows 10\. When it happens, you can force the app to shut down, effectively unfreezing said application. Here’s how to force quit an app on Windows 10.

##  Try a Keyboard Shortcut

 It's frustrating when an app you're using suddenly freezes. We’ve all done it—exasperatingly clicking the “X” button at least 20 times to close the frozen program. There’s a better way.

 With the frozen application in focus, press Alt+F4 on your keyboard to close it. If the Windows desktop is in focus instead, you'll see a "Shut Down Windows" prompt instead.

 This won't always work—some frozen applications just won't respond.

![Press Alt+F4 to force close an app. If you press Alt+F4 while the desktop is selected, you'll see a 'Shut Down Windows' window appear.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/0-altf4-restart-okay-1.png) 

##  Force Quit Using Task Manager

 As the name implies, [Task Manager](https://some-skills.techidaily.com/new-unveiling-the-secret-sauce-for-massive-tiktok-content-grabs/) is a tool that shows which apps are currently running (as well as other information like resource usage and process stats) and allows you to manage them appropriately.

 To [open Task Manager](https://youtube-blog.techidaily.com/24-top-15-gaming-capture-utilities/), you can press Ctrl+Shift+Esc on your keyboard or right-click the Windows task bar and select “Task Manager” from the menu.

![Right-click the taskbar and select 'Task Manager.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/1-open-task-manager.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2135395/19272" target="_top" id="2135395">
  <img src="//a.impactradius-go.com/display-ad/19272-2135395" border="0" alt="https://techidaily.com" width="125" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135395/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 With Task Manager open, select the task you want to force quit and then select “End Task.”

 If you don't see the name of the app in the list here, click "More Details" and find it in the list on the Processes tab.

![Select the app you want to force quit, then click 'End Task.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/2-select-the-app-and-hit-end-task.png) 

 The frozen program will now close.

##  Force Quit an App Using Command Prompt

 You can find and force quit tasks from the Command Prompt. [Open Command Prompt](https://android-frp.techidaily.com/in-2024-step-by-step-tutorial-how-to-bypass-oppo-a78-frp-by-drfone-android/) by typing **cmd** in the Windows search bar, and then selecting the “Command Prompt” app from the search results.

![Search 'cmd' in the Start Menu search, then launch Command Prompt.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/3-launch-command-prompt.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2135349/19272" target="_top" id="2135349">
  <img src="//a.impactradius-go.com/display-ad/19272-2135349" border="0" alt="https://techidaily.com" width="120" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135349/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 In Command Prompt, type **tasklist** and press "Enter." Once executed, Command Prompt will display a list of currently running programs, services, and tasks.

![The tasklist command running in Command Prompt.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/4-tasklist.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2130874/7443" target="_top" id="2130874">
  <img src="//a.impactradius-go.com/display-ad/7443-2130874" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2130874/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 The list can admittedly be a bit overwhelming, so just remember to append .exe to the end of the program name. Once you’re ready to force quit the program, execute this command:

taskkill /im <program>.exe

 So, if I wanted to force quit Notepad, I’d run this command:

taskkill /im notepad.exe

![Ending the Notepad process with the taskkill command.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/5-kill-notepad.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2047411/19272" target="_top" id="2047411">
  <img src="//a.impactradius-go.com/display-ad/19272-2047411" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2047411/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 A success message will be returned, letting you know you’ve successfully force quit the problematic application.

---

 Of course, you can always reboot or shut down your PC to close an app that's really stuck.

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
<li><a href="https://snapchat-videos.techidaily.com/new-2024-approved-quick-and-easy-capturing-the-perfect-mac-snapped-footage/"><u>[New] 2024 Approved Quick & Easy Capturing the Perfect Mac-Snapped Footage</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-google-ar-decorations-and-their-competing-products/"><u>[New] Google AR Decorations & Their Competing Products</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-ideal-extras-for-enhancing-dji-phantom-4/"><u>[New] Ideal Extras for Enhancing DJI Phantom 4</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/new-top-mac-visual-seize-methods-reviewed-limit-156-chars/"><u>[New] Top Mac Visual Seize Methods Reviewed (Limit 156 Chars)</u></a></li>
<li><a href="https://remote-screen-capture.techidaily.com/updated-in-2024-gameplay-in-focus-scrutinizing-screen-recorders/"><u>[Updated] In 2024, Gameplay in Focus Scrutinizing Screen Recorders</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-in-depth-zoom-guidance-for-virtual-team-spaces-in-msteams/"><u>[Updated] In-Depth Zoom Guidance for Virtual Team Spaces in MSTEAMS</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-initial-steps-towards-perfect-transitional-sound-levels/"><u>[Updated] Initial Steps Towards Perfect Transitional Sound Levels</u></a></li>
<li><a href="https://blue-screen-error.techidaily.com/evonik-industries-ag/"><u>Evonik Industries AG</u></a></li>
<li><a href="https://sound-issues.techidaily.com/how-to-resolve-windows-n-11-issues-with-unresponsive-headphones/"><u>How to Resolve Windows N 11 Issues with Unresponsive Headphones</u></a></li>
<li><a href="https://extra-lessons.techidaily.com/illuminating-seamless-transitions-in-song-production-crossfade/"><u>Illuminating Seamless Transitions in Song Production (Crossfade)</u></a></li>
<li><a href="https://some-techniques.techidaily.com/illuminating-the-future-luminances-influence-on-hdr-for-2024/"><u>Illuminating the Future Luminance’s Influence on HDR for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-explore-the-highest-rated-virtual-reality-games/"><u>In 2024, Explore the Highest-Rated Virtual Reality Games</u></a></li>
<li><a href="https://tech-renaissance.techidaily.com/popular-british-shows-to-binge-watch-on-netflix-now/"><u>Popular British Shows to Binge-Watch on Netflix Now</u></a></li>
<li><a href="https://youtube-docs.techidaily.com/ts-to-smoothly-resolving-youtube-short-issues-for-2024/"><u>Secrets to Smoothly Resolving YouTube Short Issues for 2024</u></a></li>
<li><a href="https://buynow-reviews.techidaily.com/ultimate-guide-to-totobays-2nd-generation-wake-up-light-top-pick-on-a-tight-budget/"><u>Ultimate Guide to Totobay's 2Nd Generation Wake-Up Light: Top Pick on a Tight Budget</u></a></li>
</ul></div>

