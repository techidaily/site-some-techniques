---
title: "Quick Troubleshooting: How to Immediately Close a Frozen Program on Your Windows 10 PC"
date: 2024-12-10T20:28:15.856Z
updated: 2024-12-15T16:48:46.571Z
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/mMYEK2gtY5c?si=ytxNz_JHZkTrwb4b" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/S0b9szh8vEk?si=NlGzpJ6MN_SJNk5A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 With Task Manager open, select the task you want to force quit and then select “End Task.”

 If you don't see the name of the app in the list here, click "More Details" and find it in the list on the Processes tab.

![Select the app you want to force quit, then click 'End Task.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/2-select-the-app-and-hit-end-task.png) 

 The frozen program will now close.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/kTHQrw8e1gk?si=gTPIa7KjhSZ0Vz97" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Force Quit an App Using Command Prompt

 You can find and force quit tasks from the Command Prompt. [Open Command Prompt](https://android-frp.techidaily.com/in-2024-step-by-step-tutorial-how-to-bypass-oppo-a78-frp-by-drfone-android/) by typing **cmd** in the Windows search bar, and then selecting the “Command Prompt” app from the search results.

![Search 'cmd' in the Start Menu search, then launch Command Prompt.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/3-launch-command-prompt.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/U_aNKnMTPjo?si=Og_mEt7NP3Fbsg2n" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 In Command Prompt, type **tasklist** and press "Enter." Once executed, Command Prompt will display a list of currently running programs, services, and tasks.

![The tasklist command running in Command Prompt.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/4-tasklist.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/E1ax-vnGdeo?si=bgTkOhOEwDTlRQE3" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://instagram-videos.techidaily.com/new-behind-the-scenes-insights-for-instagram-story-audience-for-2024/"><u>[New] Behind the Scenes Insights for Instagram Story Audience for 2024</u></a></li>
<li><a href="https://eaxpv-info.techidaily.com/new-in-2024-from-lengthy-video-to-captivating-animation-create-gifs-with-ease/"><u>[New] In 2024, From Lengthy Video to Captivating Animation - Create Gifs with Ease</u></a></li>
<li><a href="https://some-guidance.techidaily.com/new-the-ultimate-guide-to-picking-prime-stream-services/"><u>[New] The Ultimate Guide to Picking Prime Stream Services</u></a></li>
<li><a href="https://facebook-video-share.techidaily.com/new-whos-at-the-apex-youtube-subscribers-ranking/"><u>[New] Who's at the Apex? YouTube Subscribers Ranking</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/updated-four-pillars-of-mobile-video-acquisition-igtv-edition/"><u>[Updated] Four Pillars of Mobile Video Acquisition IGTV Edition</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-expert-tips-for-a-seamless-google-podcast-upload-experience/"><u>2024 Approved Expert Tips for a Seamless Google Podcast Upload Experience</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-exploring-magix-music-creators-capabilities/"><u>2024 Approved Exploring Magix Music Creator's Capabilities</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-exploring-magix-vpxs-innovative-editing-capabilities/"><u>2024 Approved Exploring Magix VPX's Innovative Editing Capabilities</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-from-novice-to-notable-launching-a-trending-solo-show/"><u>2024 Approved From Novice to Notable Launching a Trending Solo Show</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-ideal-modeling-software-for-animation-professionals/"><u>2024 Approved Ideal Modeling Software for Animation Professionals</u></a></li>
<li><a href="https://vimeo-videos.techidaily.com/comprehensive-list-of-vimeo-downloader-utilities-for-2024/"><u>Comprehensive List of Vimeo Downloader Utilities for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/expert-tips-for-stunning-photos-on-iphones-for-2024/"><u>Expert Tips for Stunning Photos on iPhones for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/flight-in-the-smallest-form-a-compreenasive-look-at-dji-sparks-miniature-wonders-for-2024/"><u>Flight in the Smallest Form A Compreenasive Look at DJI Spark's Miniature Wonders for 2024</u></a></li>
<li><a href="https://desktop-recording.techidaily.com/how-to-record-internal-audio-on-android-video-or-gameplay/"><u>How to Record Internal Audio on Android [Video or Gameplay]</u></a></li>
<li><a href="https://android-location-track.techidaily.com/in-2024-top-6-appsservices-to-trace-any-oppo-a78-5g-location-by-mobile-number-drfone-by-drfone-virtual-android/"><u>In 2024, Top 6 Apps/Services to Trace Any Oppo A78 5G Location By Mobile Number | Dr.fone</u></a></li>
</ul></div>

