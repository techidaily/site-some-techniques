---
title: "Quick Troubleshooting: How to Immediately Close a Frozen Program on Your Windows 10 PC"
date: 2024-10-01T01:50:00.043Z
updated: 2024-10-06T04:51:47.127Z
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

<!-- affiliate ads begin -->
<a href="https://review-au.sjv.io/c/5597632/2135315/14409" target="_top" id="2135315">
  <img src="//a.impactradius-go.com/display-ad/14409-2135315" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://review-au.sjv.io/i/5597632/2135315/14409" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Try a Keyboard Shortcut

 It's frustrating when an app you're using suddenly freezes. We’ve all done it—exasperatingly clicking the “X” button at least 20 times to close the frozen program. There’s a better way.

 With the frozen application in focus, press Alt+F4 on your keyboard to close it. If the Windows desktop is in focus instead, you'll see a "Shut Down Windows" prompt instead.

 This won't always work—some frozen applications just won't respond.

![Press Alt+F4 to force close an app. If you press Alt+F4 while the desktop is selected, you'll see a 'Shut Down Windows' window appear.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/0-altf4-restart-okay-1.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2049390/7443" target="_top" id="2049390">
  <img src="//a.impactradius-go.com/display-ad/7443-2049390" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2049390/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Force Quit Using Task Manager

 As the name implies, [Task Manager](https://some-skills.techidaily.com/new-unveiling-the-secret-sauce-for-massive-tiktok-content-grabs/) is a tool that shows which apps are currently running (as well as other information like resource usage and process stats) and allows you to manage them appropriately.

 To [open Task Manager](https://youtube-blog.techidaily.com/24-top-15-gaming-capture-utilities/), you can press Ctrl+Shift+Esc on your keyboard or right-click the Windows task bar and select “Task Manager” from the menu.

![Right-click the taskbar and select 'Task Manager.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/1-open-task-manager.png) 

<!-- affiliate ads begin -->
<a href="https://unicoeye.pxf.io/c/5597632/2134223/18498" target="_top" id="2134223">
  <img src="//a.impactradius-go.com/display-ad/18498-2134223" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://unicoeye.pxf.io/i/5597632/2134223/18498" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 With Task Manager open, select the task you want to force quit and then select “End Task.”

 If you don't see the name of the app in the list here, click "More Details" and find it in the list on the Processes tab.

![Select the app you want to force quit, then click 'End Task.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/2-select-the-app-and-hit-end-task.png) 

 The frozen program will now close.

##  Force Quit an App Using Command Prompt

 You can find and force quit tasks from the Command Prompt. [Open Command Prompt](https://android-frp.techidaily.com/in-2024-step-by-step-tutorial-how-to-bypass-oppo-a78-frp-by-drfone-android/) by typing **cmd** in the Windows search bar, and then selecting the “Command Prompt” app from the search results.

![Search 'cmd' in the Start Menu search, then launch Command Prompt.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/3-launch-command-prompt.png) 

 In Command Prompt, type **tasklist** and press "Enter." Once executed, Command Prompt will display a list of currently running programs, services, and tasks.

![The tasklist command running in Command Prompt.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/4-tasklist.png) 

 The list can admittedly be a bit overwhelming, so just remember to append .exe to the end of the program name. Once you’re ready to force quit the program, execute this command:

taskkill /im <program>.exe

 So, if I wanted to force quit Notepad, I’d run this command:

taskkill /im notepad.exe

![Ending the Notepad process with the taskkill command.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/5-kill-notepad.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2135371/19272" target="_top" id="2135371">
  <img src="//a.impactradius-go.com/display-ad/19272-2135371" border="0" alt="https://techidaily.com" width="320" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135371/19272" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://some-techniques.techidaily.com/updated-exploring-metaverse-ranking-best-8-vr-headsets/"><u>[Updated] Exploring Metaverse Ranking Best 8 VR Headsets</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-film-star-access-pass-talent-release/"><u>[Updated] Film Star Access Pass - Talent Release</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-infusing-interactive-elements-incorrante-youtube-music-into-videography/"><u>[Updated] Infusing Interactive Elements Incorrante YouTube Music Into Videography</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-innovative-approaches-to-harvest-large-amounts-of-tiktok-media/"><u>2024 Approved Innovative Approaches to Harvest Large Amounts of TikTok Media</u></a></li>
<li><a href="https://some-skills.techidaily.com/2024-approved-stream-control-duo-deciding-between-xsplit-and-obs-tech/"><u>2024 Approved Stream Control Duo Deciding Between XSplit and OBS Tech</u></a></li>
<li><a href="https://win-able.techidaily.com/1723012161402-cyberpunk-2077-update-2024-bug-exposed-solutions-inside/"><u>Cyberpunk 2077 Update 2024 Bug Exposed - Solutions Inside!</u></a></li>
<li><a href="https://some-techniques.techidaily.com/full-guide-to-google-docs-speech-to-text-service-for-2024/"><u>Full Guide to Google Docs Speech to Text Service for 2024</u></a></li>
<li><a href="https://instagram-video-files.techidaily.com/in-2024-exploring-the-validity-of-instagram-photos/"><u>In 2024, Exploring the Validity of Instagram Photos</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-from-novice-to-notable-launching-a-trending-solo-show/"><u>In 2024, From Novice to Notable Launching a Trending Solo Show</u></a></li>
<li><a href="https://some-techniques.techidaily.com/innovative-techniques-for-superior-recordings-with-audacity-for-2024/"><u>Innovative Techniques for Superior Recordings with Audacity for 2024</u></a></li>
<li><a href="https://extra-resources.techidaily.com/lg-bp350-evaluation-size-resolution-and-connectivity/"><u>LG BP350 Evaluation - Size, Resolution, and Connectivity</u></a></li>
<li><a href="https://tech-haven.techidaily.com/optimizing-product-understanding-through-chatgpts-personas/"><u>Optimizing Product Understanding Through ChatGPT's Personas</u></a></li>
<li><a href="https://tiktok-clips.techidaily.com/perfect-your-tiktok-presence-with-siri-commands-and-features/"><u>Perfect Your TikTok Presence with Siri Commands and Features</u></a></li>
<li><a href="https://extra-tips.techidaily.com/pinnacle-spotlight-tapes/"><u>Pinnacle Spotlight Tapes</u></a></li>
<li><a href="https://location-social.techidaily.com/why-your-whatsapp-location-is-not-updating-and-how-to-fix-on-vivo-s18-pro-drfone-by-drfone-virtual-android/"><u>Why Your WhatsApp Location is Not Updating and How to Fix On Vivo S18 Pro | Dr.fone</u></a></li>
</ul></div>

