---
title: "Securing Your PC: A Step-by-Step Guide to Locking Windows 11 with Command Line"
date: 2024-11-10T11:43:04.255Z
updated: 2024-11-13T08:49:14.347Z
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

### Key Takeaways

* To lock your Windows PC using Command Prompt, run "**Rundll32.exe user32.dll,LockWorkStation"** in the Command Prompt
* To set the lock screen timeout, run "**powercfg.exe /SETACVALUEINDEX SCHEME\_CURRENT SUB\_VIDEO VIDEOCONLOCK <time>"** in Command Prompt as Admin
* Activate the lock screen timeout setting by running "**powercfg.exe /SETACTIVE SCHEME\_CURRENT"** after you set the timeout.

 One of the first rules of cyber security is to always lock your PC before stepping away. While it may not be the quickest way to lock your Windows 10 PC, you can do it using the Command Prompt.

##  Lock Your Windows 10 PC Using Command Prompt

 First, [open the Command Prompt](https://android-frp.techidaily.com/in-2024-step-by-step-tutorial-how-to-bypass-oppo-a78-frp-by-drfone-android/) on your PC by opening the Start menu, typing “cmd” in the Windows Search bar, and then selecting “Command Prompt” from the search results.

![Click the Start button, search for 'cmd,' then open 'Command Prompt.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/1-launch-cmd.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2105860/7443" target="_top" id="2105860">
  <img src="//a.impactradius-go.com/display-ad/7443-2105860" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2105860/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Command Prompt will now open. Here, run this command to lock your Windows 10 PC.

Rundll32.exe user32.dll,LockWorkStation

![Locking your PC with Command Prompt.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/2-lock-pc-command-prompt.png) 

 Once executed, your PC will be locked. You'll have to sign back in with your PIN, password, or whatever sign-in method you usually use.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2087408/7443" target="_top" id="2087408">
  <img src="//a.impactradius-go.com/display-ad/7443-2087408" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2087408/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Set the Lock Screen Timeout Setting Using Command Prompt

 Once you’ve locked your PC, the lock screen will generally be displayed for a certain amount of time before it time outs. You can set the amount of time that needs to pass before timing out using the Command Prompt.

 To do this, you’ll need to [open Command Prompt as an admin](https://screen-mirror.techidaily.com/how-to-screen-mirroring-xiaomi-14-ultra-drfone-by-drfone-android/). Do so by typing “cmd” in the Windows Search bar and then right-clicking “Command Prompt” from the results. Next, select “Run As Administrator” from the menu that appears.

![Launching Command Prompt as admin.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/3-launch-cmd.png) 

<!-- affiliate ads begin -->
<span id="1982508">
					<video width="576" height="240" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1982508.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/22993-1982508">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1982508.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:360px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fhomestyler.sjv.io%2Fc%2F5597632%2F1982508%2F22993'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1982508/22993" style="position:absolute;visibility:hidden;" border="0" />
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

<!-- affiliate ads begin -->
<a href="https://unicoeye.pxf.io/c/5597632/2134224/18498" target="_top" id="2134224">
  <img src="//a.impactradius-go.com/display-ad/18498-2134224" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://unicoeye.pxf.io/i/5597632/2134224/18498" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://on-screen-recording.techidaily.com/new-2024-approved-how-to-enable-grid-view-on-google-meet-to-see-every-participant/"><u>[New] 2024 Approved How to Enable Grid View on Google Meet to See Every Participant?</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-free-3d-text-psd-goldmine-top-selections/"><u>[New] Free 3D Text PSD Goldmine - Top Selections</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-improving-sound-speeds-a-guide-for-safe-spotify-use/"><u>[New] Improving Sound Speeds A Guide for Safe Spotify Use</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-get-perfect-film-endings-for-your-projects-on-the-house/"><u>[Updated] Get Perfect Film Endings for Your Projects - On the House</u></a></li>
<li><a href="https://facebook-video-share.techidaily.com/updated-in-2024-charting-your-path-to-success-in-youtubes-earnings-system/"><u>[Updated] In 2024, Charting Your Path to Success in YouTube's Earnings System</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-exploring-interactive-boundaries-the-vision-of-mixed-reality/"><u>2024 Approved Exploring Interactive Boundaries The Vision of Mixed Reality</u></a></li>
<li><a href="https://snapchat-videos.techidaily.com/2024-approved-how-to-effectively-archive-snapchat-videos-on-mobile-phones/"><u>2024 Approved How to Effectively Archive Snapchat Videos on Mobile Phones</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-in-depth-review-samsungs-immersive-360-degree-camera/"><u>2024 Approved In-Depth Review Samsung's Immersive 360-Degree Camera</u></a></li>
<li><a href="https://windows11.techidaily.com/activating-telnet-on-windows-3-key-methods/"><u>Activating Telnet on Windows: 3 Key Methods</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-fitness-beatdowns-20-electrifying-tunes-for-your-exercising-playlist/"><u>In 2024, Fitness Beatdowns 20 Electrifying Tunes for Your Exercising Playlist</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-innovative-audio-dramatic-writing/"><u>In 2024, Innovative Audio Dramatic Writing</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-innovative-shooting-with-drones-in-media/"><u>In 2024, Innovative Shooting with Drones in Media</u></a></li>
<li><a href="https://extra-support.techidaily.com/in-2024-precision-zoom-sound-reclaiming-clarity/"><u>In 2024, Precision Zoom Sound Reclaiming Clarity</u></a></li>
<li><a href="https://win-answers.techidaily.com/resolving-the-modern-warfare-pcxbox-dev-6034-bug-a-comprehensive-guide/"><u>Resolving the Modern Warfare PC/Xbox DEV-6034 Bug: A Comprehensive Guide</u></a></li>
<li><a href="https://buynow-info.techidaily.com/softbox-luxe-start-limostudio-agg814-breakdown/"><u>SoftBox Luxe Start: LimoStudio AGG814 Breakdown</u></a></li>
<li><a href="https://win-howtos.techidaily.com/solutions-for-resolving-windows-error-code-0xc0000098/"><u>Solutions for Resolving Windows Error Code 0xC0000098</u></a></li>
<li><a href="https://techidaily.com/things-you-dont-know-about-tecno-spark-20c-reset-code-drfone-by-drfone-reset-android-reset-android/"><u>Things You Dont Know About Tecno Spark 20C Reset Code | Dr.fone</u></a></li>
</ul></div>

