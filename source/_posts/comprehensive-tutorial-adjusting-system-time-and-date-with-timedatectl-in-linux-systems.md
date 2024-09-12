---
title: "Comprehensive Tutorial: Adjusting System Time and Date with Timedatectl in Linux Systems"
date: 2024-09-11T20:15:20.532Z
updated: 2024-09-12T20:15:20.532Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://thmb.techidaily.com/8d6fc5e965f8f403ab26d9d65a1bca0fa8c0fcf476d607d4885f74d57cfde7c9.jpg
---

## Comprehensive Tutorial: Adjusting System Time and Date with Timedatectl in Linux Systems

### Quick Links

* [It's All Relative](https://win-dash.techidaily.com/secure-your-vr-experience-download-oculus-drivers-for-all-windows-os/)
* [Getting Started With timedatectl](https://howto.techidaily.com/why-does-my-vivo-y55s-5g-2023-keep-turning-off-by-itself-6-fixes-are-here-drfone-by-drfone-fix-android-problems-fix-android-problems/)
* [Setting the Time Zone](https://buynow-reviews.techidaily.com/comprehensive-review-of-the-smart-ring-video-doorbell-pro/)
* [Manually Setting the Time and Date](https://ai-vdieo-software.techidaily.com/the-ultimate-list-of-avi-video-cutters-16-best-options-for-windows-mac-and-android-users/)
* [RTC: UTC or LTZ?](https://howto.techidaily.com/cellular-network-not-available-for-voice-calls-on-lava-yuva-3-pro-drfone-by-drfone-fix-android-problems-fix-android-problems/)
* [Set It and Forget It](https://on-screen-recording.techidaily.com/updated-2024-approved-mp4-screen-grabber-free-easy-access/)

 The Linux `timedatectl` command lets you set your time, date, and timezone for your system clock and your real-time clock. Spare a moment, and we'll show you how it all works.

##  It's All Relative

 Your computer's treatment of time is one of those things that you might expect to be pretty straightforward. At least, until you start to look into it.

 The Linux system clock counts the number of seconds since [the Unix epoch](https://extra-lessons.techidaily.com/5-leading-edge-4k-tvs-for-gamers/). This was at 00:00:00 on Jan. 1, 1970, UTC. UTC stands for universal time coordinated but it is usually said as coordinated universal time or just universal time. This is the time standard by which the world manages and regulates time. Different time zones apply an offset to UTC to obtain their local time. Some time zones are ahead of UTC and others are behind it.

 The system clock in Linux computers is software-based. Obviously, it cannot run when the computer is powered off. Another clock, a battery-backed hardware-based real-time clock, is able to run when the computer is off. Its purpose is to tell the system clock what time it is whenever Linux boots up. Unless access to a network time protocol (NTP) server is possible.

 NTP servers are servers that provide accurate time information to computers that request it. If you boot up your computer or laptop and there is no internet access—or it hasn't been [configured to use NTP servers](https://access.redhat.com/documentation/en-us/red%5Fhat%5Fenterprise%5Flinux/7/html/system%5Fadministrators%5Fguide/ch-configuring%5Fntp%5Fusing%5Fntpd)—the real-time clock is used to prime the system clock instead of an NTP Server.

 The system clock is always in UTC. Any application that needs to acquire the local time needs to:

* Access the system clock and obtain UTC
* Know what time zone it is in and apply the correct offset
* Take into account whether [daylight savings time](https://tech-haven.techidaily.com/website-metamorphosis-understanding-the-effects-of-cognitive-computing-on-seo-practices/) is in effect

 The conversion from UTC to local time is done by the application, not the system clock. Or, more accurately, the conversion is performed by the time and date libraries that the application is linked to. That's why it is vital that your computer knows which timezone it is, what UTC time is, how many seconds have passed since the Unix epoch, and whether daylight savings time is in effect.

 On systemd-based Linux distributions, we use the `timedatectl` command to see or change those settings and values.

<!-- affiliate ads begin -->
<a href="https://bluettius.sjv.io/c/5597632/2139118/17108" target="_top" id="2139118">
  <img src="//a.impactradius-go.com/display-ad/17108-2139118" border="0" alt="https://techidaily.com" width="468" height="60"/>
</a>
<img height="0" width="0" src="https://bluettius.sjv.io/i/5597632/2139118/17108" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Getting Started With timedatectl

 To see the current data and time and other values, use the `timedatectl` command with the status operator.

timedatectl status

![The output from the tidedatectl command using the status operator](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/01/1-4.png) 

 Actually, you can drop the status and you'll still get the same output.

timedatectl

![The output from the timedatectl command with no operator](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/01/2-4.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2115918/19272" target="_top" id="2115918">
  <img src="//a.impactradius-go.com/display-ad/19272-2115918" border="0" alt="https://techidaily.com" width="336" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2115918/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Both sets of output show:

* **Local Time**: The time the computer thinks it is, according to its time zone.
* **Universal Time**: The UTC time.
* **RTC Time**: The time the real-time clock is using. Usually, this is UTC.
* **Time zone**: Information regarding the configured time zone.
* **System Clock Synchronized**: Whether the system clock is synchronized with an NTP server.
* **NTP Service**: Whether the computer's NTP service is active.
* **RTC in local TZ**: Whether the real-time clock is using the local time instead of UTC.

 You can see how many time zones the `timedatectl` command supports by typing:

timedatectl list-timezones | wc -l

![Counting the timedatectl time zones](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/01/3-5.png) 

 That's way more than there are [timezones in the world](https://www.timeanddate.com/time/current-number-time-zones.html). If we [pipe the output](https://review-topics.techidaily.com/how-to-transfer-whatsapp-from-iphone-11-pro-to-other-iphone-11-pro-devices-drfone-by-drfone-transfer-whatsapp-from-ios-transfer-whatsapp-from-ios/) into `grep` and filter out the entries for "America" and pipe that [into less](https://win-amazing.techidaily.com/hp-scanjet-driver-updates-available-install-now-for-enhanced-performance-on-windows-systems/), we can scroll through a more manageable list.

timedatectl list-timezones | grep "America/" | less

![Filtering out American time zones with grep](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/01/4-4.png) 

 As you review that list you'll see "America" is taken to have its widest possible meaning. The second thing you'll notice is most of the entries aren't actual time zones.

!["American" time zone list in less](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/01/5-4.png) 

<!-- affiliate ads begin -->
<a href="https://ephamedtechinc.pxf.io/c/5597632/2137207/26400" target="_top" id="2137207">
  <img src="//a.impactradius-go.com/display-ad/26400-2137207" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://ephamedtechinc.pxf.io/i/5597632/2137207/26400" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

<!-- affiliate ads begin -->
<a href="https://unicoeye.pxf.io/c/5597632/2134242/18498" target="_top" id="2134242">
  <img src="//a.impactradius-go.com/display-ad/18498-2134242" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://unicoeye.pxf.io/i/5597632/2134242/18498" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Setting the Time Zone

 If you look through the unfiltered list of time zones supported by `timedatectl` you'll see places as well as time zones. To set a time zone you can specify it by name like EST or GMT, or you can pick a location in the same time zone as you, like London or New York.

 Resetting your time zone isn't something you'll be doing often, but perhaps you've moved home or you're working away for a while and want to localize your laptop. If you need to reset your time zone, pick a location in the time zone you want to use.

 We'll set this computer to mountain time, which is the same time zone as Edmonton. We'll then see how the settings have changed.

timedatectl set-timezone "America/Edmonton"

timedatectl

![New time zone and time settings](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/01/6-4.png) 

 Our time zone has been changed, our local time has altered, and our offset from UTC has increased.

##  Manually Setting the Time and Date

 Although manually setting the time and date is possible, usually you won't need to. Using time synchronization and NTP is the preferred way to keep your computer's time and date accurate. If you try to change your computers' date or time you'll probably get an error, telling you that time synchronization is in use.

timedatectl set-time 10:30:00

![You can't set the time if time synchronization is in force](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/01/7-4.png) 

<!-- affiliate ads begin -->
<a href="https://ephamedtechinc.pxf.io/c/5597632/2136624/26400" target="_top" id="2136624">
  <img src="//a.impactradius-go.com/display-ad/26400-2136624" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://ephamedtechinc.pxf.io/i/5597632/2136624/26400" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Use this command to turn off the time synchronization service:

sudo systemctl stop systemd-timesyncd.service

 You can set the time, the date, or both using the `timedatectl` set-time operator. dates are in year-month-day order YYY-MM-DD, and time is in hours-minutes-seconds order HH:MM:SS. We're going to set the time and date with this command:

timedatectl set-time "2022-01-30 10:30:00"

 We'll then check that the changes have taken place, using `timedatectl`.

timedatectl

![Manually setting the time and date](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/01/8-5.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2132161/7443" target="_top" id="2132161">
  <img src="//a.impactradius-go.com/display-ad/7443-2132161" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2132161/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 The date and time have changed. Also, note the computer is using a false UTC time. We're also informed that the system clock is not being synchronized and the NTP service is inactive.

 If you have internet access, as soon as you restore the time synchronization service the time is retrieved and all of the details are correctly reset.

sudo systemctl start systemd-timesyncd.service

timedatectl

![Restarting the NTP service and restoring the correct time values](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/01/9-4.png) 

<!-- affiliate ads begin -->
<a href="https://review-au.sjv.io/c/5597632/2098702/14409" target="_top" id="2098702">
  <img src="//a.impactradius-go.com/display-ad/14409-2098702" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://review-au.sjv.io/i/5597632/2098702/14409" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  RTC: UTC or LTZ?

 It's possible to have your real-time clock set to your local time zone time instead of to UTC—possible, but inadvisable. If you make the change, you'll see a warning about the dire effects this may have on your system in the future.

 The reason for showing you this method is you might encounter a machine where they are having strange issues with their time settings. This is how to set the real-time clock back to UTC.

 First, we'll need to set it to the local time zone.

timedatectl set-local-rtc 1

 Then we'll ask `timedatectl` for its status.

timedatectl

![Setting the real-time clock to the local time zone, and the warning that accompanies that](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/01/10-4.png) 

<!-- affiliate ads begin -->
<span id="1793213">
					<video width="864" height="1296" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1793213.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/19135-1793213">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1793213.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:540px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Ftinyland.pxf.io%2Fc%2F5597632%2F1793213%2F19135'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1793213/19135" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 I think they've made their feelings clear.

 To restore the real-time clock to UTC, use this command:

timedatectl set-local-rtc 0

##  Set It and Forget It

 Unless you made an error during the installation of your Linux distribution, or you relocate there's usually no reason to be modifying the settings of your system and real-time clocks.

 Set the system clock to your time zone, the real-time clock to UTC, and make sure you're system is polling a network time protocol server. That's the default state after most installations.

 If they're all set, your computer's time systems will look after themselves.

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
<li><a href="https://facebook-video-footage.techidaily.com/new-dominating-viewers-spaces-channel-empire-rules-for-2024/"><u>[New] Dominating Viewers' Spaces Channel Empire Rules for 2024</u></a></li>
<li><a href="https://on-screen-recording.techidaily.com/updated-2024-approved-elite-nintendo-switch-battle-selection-max-156/"><u>[Updated] 2024 Approved Elite Nintendo Switch Battle Selection (Max 156)</u></a></li>
<li><a href="https://fox-access.techidaily.com/updated-in-2024-revolutionizing-real-estate-with-metaverse-ads/"><u>[Updated] In 2024, Revolutionizing Real Estate with Metaverse Ads</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/updated-understanding-the-dynamics-of-ig-reels-vs-ig-stories-for-2024/"><u>[Updated] Understanding the Dynamics of IG Reels Vs IG Stories for 2024</u></a></li>
<li><a href="https://screen-video-capture.techidaily.com/2024-approved-pixels-and-players-advanced-tactics-for-recording-gaming/"><u>2024 Approved Pixels and Players Advanced Tactics for Recording Gaming</u></a></li>
<li><a href="https://video-screen-grab.techidaily.com/best-free-open-source-video-conferencing-software-ranked-by-industry/"><u>Best Free Open Source Video Conferencing Software Ranked by Industry</u></a></li>
<li><a href="https://sound-issues.techidaily.com/how-to-activate-your-dolby-digital-live-sound-drivers-on-a-windows-11-pc/"><u>How To Activate Your Dolby Digital Live Sound Drivers on a Windows 11 PC</u></a></li>
<li><a href="https://extra-approaches.techidaily.com/inside-microsofts-visionary-hololens-innovation-for-2024/"><u>Inside Microsoft's Visionary HoloLens Innovation for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/introducing-bing-chat-ai-the-future-of-mobile-conversations-on-your-devices-dashboard/"><u>Introducing Bing Chat AI: The Future of Mobile Conversations on Your Device's Dashboard</u></a></li>
<li><a href="https://some-techniques.techidaily.com/introducing-dall-e-microsofts-new-image-creation-feature-in-bing-chat/"><u>Introducing DALL-E: Microsoft's New Image Creation Feature in Bing Chat</u></a></li>
<li><a href="https://some-techniques.techidaily.com/introducing-ps5-compatible-virtual-reality-the-demand-for-a-playstation-vr-2-version-on-pc/"><u>Introducing PS5 Compatible Virtual Reality: The Demand for a PlayStation VR 2 Version on PC</u></a></li>
<li><a href="https://some-techniques.techidaily.com/introducing-stable-diffusion-xl-v10-a-new-era-of-improved-digital-artistry-begins/"><u>Introducing Stable Diffusion XL v1.0 - A New Era of Improved Digital Artistry Begins</u></a></li>
<li><a href="https://some-techniques.techidaily.com/mastering-midjourney-a-guide-to-producing-perfect-visuals-using-these-6-tips/"><u>Mastering MidJourney: A Guide to Producing Perfect Visuals Using These 6 Tips</u></a></li>
<li><a href="https://some-techniques.techidaily.com/navigating-digital-assets-how-to-distinguish-between-crypto-tokens-and-coins/"><u>Navigating Digital Assets: How to Distinguish Between Crypto Tokens and Coins</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/next-big-thing-10-games-that-inspire-gta-v-for-2024/"><u>Next Big Thing 10 Games That Inspire GTA V for 2024</u></a></li>
</ul></div>

