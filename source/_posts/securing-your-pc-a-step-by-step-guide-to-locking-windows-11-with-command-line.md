---
title: "Securing Your PC: A Step-by-Step Guide to Locking Windows 11 with Command Line"
date: 2024-10-07T04:34:12.438Z
updated: 2024-10-11T18:09:53.337Z
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
<a href="https://appsumo.8odi.net/c/5597632/2068433/7443" target="_top" id="2068433">
  <img src="//a.impactradius-go.com/display-ad/7443-2068433" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2068433/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

### Key Takeaways

* To lock your Windows PC using Command Prompt, run "**Rundll32.exe user32.dll,LockWorkStation"** in the Command Prompt
* To set the lock screen timeout, run "**powercfg.exe /SETACVALUEINDEX SCHEME\_CURRENT SUB\_VIDEO VIDEOCONLOCK <time>"** in Command Prompt as Admin
* Activate the lock screen timeout setting by running "**powercfg.exe /SETACTIVE SCHEME\_CURRENT"** after you set the timeout.

 One of the first rules of cyber security is to always lock your PC before stepping away. While it may not be the quickest way to lock your Windows 10 PC, you can do it using the Command Prompt.

##  Lock Your Windows 10 PC Using Command Prompt

 First, [open the Command Prompt](https://android-frp.techidaily.com/in-2024-step-by-step-tutorial-how-to-bypass-oppo-a78-frp-by-drfone-android/) on your PC by opening the Start menu, typing “cmd” in the Windows Search bar, and then selecting “Command Prompt” from the search results.

![Click the Start button, search for 'cmd,' then open 'Command Prompt.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/1-launch-cmd.png) 

 Command Prompt will now open. Here, run this command to lock your Windows 10 PC.

Rundll32.exe user32.dll,LockWorkStation

![Locking your PC with Command Prompt.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/2-lock-pc-command-prompt.png) 

<!-- affiliate ads begin -->
<a href="https://25home.pxf.io/c/5597632/2148650/16836" target="_top" id="2148650">
  <img src="//a.impactradius-go.com/display-ad/16836-2148650" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://25home.pxf.io/i/5597632/2148650/16836" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Once executed, your PC will be locked. You'll have to sign back in with your PIN, password, or whatever sign-in method you usually use.

<!-- affiliate ads begin -->
<span id="1498635">
					<video width="320" height="320" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1498635.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/17326-1498635">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1498635.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:200px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fancheer.sjv.io%2Fc%2F5597632%2F1498635%2F17326'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1498635/17326" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://bluetties.sjv.io/c/5597632/2141687/17094" target="_top" id="2141687">
  <img src="//a.impactradius-go.com/display-ad/17094-2141687" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://bluetties.sjv.io/i/5597632/2141687/17094" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://screen-capture.techidaily.com/new-2024-approved-vocal-variety-at-your-fingertips-top-7-speech-modification-apps-reviewed/"><u>[New] 2024 Approved Vocal Variety at Your Fingertips Top 7 Speech Modification Apps Reviewed</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-giroptic-360cam-complete-review/"><u>[New] Giroptic 360Cam Complete Review</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-how-much-will-it-cost-to-shoot-a-music-video/"><u>[New] How Much Will It Cost To Shoot A Music Video?</u></a></li>
<li><a href="https://screen-activity-recording.techidaily.com/new-streamlabs-obs-review-and-alternative/"><u>[New] Streamlabs OBS Review and Alternative</u></a></li>
<li><a href="https://youtube-webster.techidaily.com/ed-2024-approved-unlocking-the-secrets-to-successful-rapid-subscribing-on-youtube/"><u>[Updated] 2024 Approved Unlocking the Secrets to Successful Rapid Subscribing on YouTube</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-film-timeframe-determining-gb-storage-requirement/"><u>[Updated] Film Timeframe Determining GB Storage Requirement</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-getting-the-most-out-of-pc-hdr-videos/"><u>[Updated] Getting the Most Out of PC HDR Videos</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-how-does-vegaspros-2019-version-improve-gaming/"><u>[Updated] How Does VegasPro's 2019 Version Improve Gaming</u></a></li>
<li><a href="https://facebook-video-footage.techidaily.com/updated-maximize-screen-time-top-10-free-youtube-playlist-extractors/"><u>[Updated] Maximize Screen Time Top 10 Free YouTube Playlist Extractors</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-hilarityhatcher-create-comedy-with-a-click/"><u>2024 Approved HilarityHatcher Create Comedy with a Click</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-how-to-adjust-your-photovideo-with-3dlut-mobile/"><u>2024 Approved How to Adjust Your Photo/Video with 3DLUT Mobile</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/how-can-i-get-more-stardust-in-pokemon-go-on-tecno-camon-20-drfone-by-drfone-virtual-android/"><u>How can I get more stardust in pokemon go On Tecno Camon 20? | Dr.fone</u></a></li>
<li><a href="https://technical-tips.techidaily.com/how-to-bridge-a-laptop-and-bluetooth-speaker-via-wireless-technology/"><u>How To Bridge A Laptop And Bluetooth Speaker Via Wireless Technology</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-gopros-deep-sea-capturing-unforgettable-underwater-scenes/"><u>In 2024, GoPro's Deep Sea Capturing Unforgettable Underwater Scenes</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-humorhub-join-the-fun-filled-world/"><u>In 2024, HumorHub Join the Fun-Filled World</u></a></li>
<li><a href="https://android-location-track.techidaily.com/in-2024-top-7-phone-number-locators-to-track-oppo-a18-location-drfone-by-drfone-virtual-android/"><u>In 2024, Top 7 Phone Number Locators To Track Oppo A18 Location | Dr.fone</u></a></li>
<li><a href="https://pokemon-go-android.techidaily.com/in-2024-what-pokemon-evolve-with-a-dawn-stone-for-honor-80-pro-straight-screen-edition-drfone-by-drfone-virtual-android/"><u>In 2024, What Pokémon Evolve with A Dawn Stone For Honor 80 Pro Straight Screen Edition? | Dr.fone</u></a></li>
<li><a href="https://common-error.techidaily.com/revive-your-windows-10-touchscreen-top-5-easy-methods/"><u>Revive Your Windows 10 Touchscreen: Top 5 Easy Methods</u></a></li>
<li><a href="https://vp-tips.techidaily.com/ultimate-guide-to-free-dvd-ripper-tools-the-best-picks-for-legally-copying-your-movies-and-shows-at-zero-cost/"><u>Ultimate Guide to Free DVD Ripper Tools: The Best Picks for Legally Copying Your Movies and Shows at Zero Cost</u></a></li>
</ul></div>

