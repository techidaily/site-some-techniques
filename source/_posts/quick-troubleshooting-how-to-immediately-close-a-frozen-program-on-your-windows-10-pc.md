---
title: "Quick Troubleshooting: How to Immediately Close a Frozen Program on Your Windows 10 PC"
date: 2024-09-30T02:15:54.138Z
updated: 2024-09-30T18:38:26.848Z
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

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1959712/19272" target="_top" id="1959712">
  <img src="//a.impactradius-go.com/display-ad/19272-1959712" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1959712/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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

 With Task Manager open, select the task you want to force quit and then select “End Task.”

 If you don't see the name of the app in the list here, click "More Details" and find it in the list on the Processes tab.

![Select the app you want to force quit, then click 'End Task.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/2-select-the-app-and-hit-end-task.png) 

<!-- affiliate ads begin -->
<a href="https://zebaoaffiliateprogram.pxf.io/c/5597632/2137974/21526" target="_top" id="2137974">
  <img src="//a.impactradius-go.com/display-ad/21526-2137974" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://zebaoaffiliateprogram.pxf.io/i/5597632/2137974/21526" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 The frozen program will now close.

##  Force Quit an App Using Command Prompt

 You can find and force quit tasks from the Command Prompt. [Open Command Prompt](https://android-frp.techidaily.com/in-2024-step-by-step-tutorial-how-to-bypass-oppo-a78-frp-by-drfone-android/) by typing **cmd** in the Windows search bar, and then selecting the “Command Prompt” app from the search results.

![Search 'cmd' in the Start Menu search, then launch Command Prompt.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/3-launch-command-prompt.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1997643/19272" target="_top" id="1997643">
  <img src="//a.impactradius-go.com/display-ad/19272-1997643" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1997643/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 In Command Prompt, type **tasklist** and press "Enter." Once executed, Command Prompt will display a list of currently running programs, services, and tasks.

![The tasklist command running in Command Prompt.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/4-tasklist.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2068425/7443" target="_top" id="2068425">
  <img src="//a.impactradius-go.com/display-ad/7443-2068425" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2068425/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 The list can admittedly be a bit overwhelming, so just remember to append .exe to the end of the program name. Once you’re ready to force quit the program, execute this command:

taskkill /im <program>.exe

 So, if I wanted to force quit Notepad, I’d run this command:

taskkill /im notepad.exe

![Ending the Notepad process with the taskkill command.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/5-kill-notepad.png) 

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
<li><a href="https://article-posts.techidaily.com/new-action-in-motion-best-surfing-cams-of-2023-update/"><u>[New] Action in Motion Best Surfing Cams of 2023 Update</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-excellence-visuals-appraisal-pinnacle-studio-current-year/"><u>[New] Excellence Visuals Appraisal Pinnacle Studio, Current Year</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-find-your-photo-oasis-a-guide-to-pexels/"><u>[New] Find Your Photo Oasis A Guide to Pexels</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-how-to-save-top-cloud-providers-rates/"><u>[New] How to Save Top Cloud Providers' Rates</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-harmonizing-audio-with-visuals-adding-melodies-to-powerpoint/"><u>[Updated] Harmonizing Audio with Visuals Adding Melodies to PowerPoint</u></a></li>
<li><a href="https://some-tips.techidaily.com/updated-timeless-1980s-filters-and-techniques-in-editing/"><u>[Updated] Timeless 1980S Filters & Techniques in Editing</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-from-compressed-to-captioned-zip-to-srt-effortlessly/"><u>2024 Approved From Compressed To Captioned Zip to .Srt Effortlessly</u></a></li>
<li><a href="https://win-solutions.techidaily.com/como-convertirte-tu-pelicula-mkv-gratis-en-linea-usando-la-herramienta-de-movavi/"><u>Cómo Convertirte Tu Película MKV Gratis en Línea Usando La Herramienta De Movavi</u></a></li>
<li><a href="https://fox-making.techidaily.com/efficient-file-transfer-mastering-the-copy-and-move-box-wizard/"><u>Efficient File Transfer: Mastering the Copy and Move Box Wizard</u></a></li>
<li><a href="https://apple-account.techidaily.com/how-to-fix-apple-id-verification-code-not-working-from-iphone-11-pro-by-drfone-ios/"><u>How To Fix Apple ID Verification Code Not Working From iPhone 11 Pro</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-framework-for-utilizing-movies-as-learning-tools/"><u>In 2024, Framework for Utilizing Movies as Learning Tools</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/process-of-screen-sharing-vivo-y200e-5g-to-pc-detailed-steps-drfone-by-drfone-android/"><u>Process of Screen Sharing Vivo Y200e 5G to PC- Detailed Steps | Dr.fone</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/simple-guide-how-to-effortlessly-move-films-from-your-ipad-to-a-mac/"><u>Simple Guide: How to Effortlessly Move Films From Your iPad to a Mac</u></a></li>
</ul></div>

