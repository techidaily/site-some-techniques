---
title: "Comprehensive Tutorial: Adjusting System Time and Date with Timedatectl in Linux Systems"
date: 2024-09-05T05:27:31.507Z
updated: 2024-09-06T05:27:31.507Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://thmb.techidaily.com/8d6fc5e965f8f403ab26d9d65a1bca0fa8c0fcf476d607d4885f74d57cfde7c9.jpg
---

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1918684/19272" target="_top" id="1918684">
  <img src="//a.impactradius-go.com/display-ad/19272-1918684" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1918684/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Comprehensive Tutorial: Adjusting System Time and Date with Timedatectl in Linux Systems

<!-- affiliate ads begin -->
<span id="1975648">
					<video width="128" height="480" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1975648.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/22993-1975648">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1975648.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:80px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fhomestyler.sjv.io%2Fc%2F5597632%2F1975648%2F22993'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1975648/22993" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
### Quick Links

* [It's All Relative](https://win-dash.techidaily.com/secure-your-vr-experience-download-oculus-drivers-for-all-windows-os/)
* [Getting Started With timedatectl](https://howto.techidaily.com/why-does-my-vivo-y55s-5g-2023-keep-turning-off-by-itself-6-fixes-are-here-drfone-by-drfone-fix-android-problems-fix-android-problems/)
* [Setting the Time Zone](https://buynow-reviews.techidaily.com/comprehensive-review-of-the-smart-ring-video-doorbell-pro/)
* [Manually Setting the Time and Date](https://ai-vdieo-software.techidaily.com/the-ultimate-list-of-avi-video-cutters-16-best-options-for-windows-mac-and-android-users/)
* [RTC: UTC or LTZ?](https://howto.techidaily.com/cellular-network-not-available-for-voice-calls-on-lava-yuva-3-pro-drfone-by-drfone-fix-android-problems-fix-android-problems/)
* [Set It and Forget It](https://on-screen-recording.techidaily.com/updated-2024-approved-mp4-screen-grabber-free-easy-access/)

 The Linux `timedatectl` command lets you set your time, date, and timezone for your system clock and your real-time clock. Spare a moment, and we'll show you how it all works.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2030370/7443" target="_top" id="2030370">
  <img src="//a.impactradius-go.com/display-ad/7443-2030370" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2030370/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
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
<a href="https://appsumo.8odi.net/c/5597632/2043594/7443" target="_top" id="2043594">
  <img src="//a.impactradius-go.com/display-ad/7443-2043594" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2043594/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
##  Getting Started With timedatectl

 To see the current data and time and other values, use the `timedatectl` command with the status operator.

timedatectl status

![The output from the tidedatectl command using the status operator](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/01/1-4.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1925489/19272" target="_top" id="1925489">
  <img src="//a.impactradius-go.com/display-ad/19272-1925489" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1925489/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 Actually, you can drop the status and you'll still get the same output.

timedatectl

![The output from the timedatectl command with no operator](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/01/2-4.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1902278/19272" target="_top" id="1902278">
  <img src="//a.impactradius-go.com/display-ad/19272-1902278" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1902278/19272" style="position:absolute;visibility:hidden;" border="0" />
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

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2044586/7443" target="_top" id="2044586">
  <img src="//a.impactradius-go.com/display-ad/7443-2044586" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2044586/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 As you review that list you'll see "America" is taken to have its widest possible meaning. The second thing you'll notice is most of the entries aren't actual time zones.

!["American" time zone list in less](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/01/5-4.png) 

<!-- affiliate ads begin -->
<a href="https://laganoo.pxf.io/c/5597632/1657386/16446" target="_top" id="1657386">
  <img src="//a.impactradius-go.com/display-ad/16446-1657386" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://laganoo.pxf.io/i/5597632/1657386/16446" style="position:absolute;visibility:hidden;" border="0" />
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

 Use this command to turn off the time synchronization service:

sudo systemctl stop systemd-timesyncd.service

 You can set the time, the date, or both using the `timedatectl` set-time operator. dates are in year-month-day order YYY-MM-DD, and time is in hours-minutes-seconds order HH:MM:SS. We're going to set the time and date with this command:

timedatectl set-time "2022-01-30 10:30:00"

 We'll then check that the changes have taken place, using `timedatectl`.

timedatectl

![Manually setting the time and date](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/01/8-5.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1959712/19272" target="_top" id="1959712">
  <img src="//a.impactradius-go.com/display-ad/19272-1959712" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1959712/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 The date and time have changed. Also, note the computer is using a false UTC time. We're also informed that the system clock is not being synchronized and the NTP service is inactive.

 If you have internet access, as soon as you restore the time synchronization service the time is retrieved and all of the details are correctly reset.

sudo systemctl start systemd-timesyncd.service

timedatectl

![Restarting the NTP service and restoring the correct time values](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/01/9-4.png) 

##  RTC: UTC or LTZ?

 It's possible to have your real-time clock set to your local time zone time instead of to UTC—possible, but inadvisable. If you make the change, you'll see a warning about the dire effects this may have on your system in the future.

 The reason for showing you this method is you might encounter a machine where they are having strange issues with their time settings. This is how to set the real-time clock back to UTC.

 First, we'll need to set it to the local time zone.

timedatectl set-local-rtc 1

 Then we'll ask `timedatectl` for its status.

timedatectl

![Setting the real-time clock to the local time zone, and the warning that accompanies that](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/01/10-4.png) 

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
<li><a href="https://video-capture.techidaily.com/new-2024-approved-ancient-warriors-new-battlegrounds-top-games-like-the-japanese-epic/"><u>[New] 2024 Approved  Ancient Warriors, New Battlegrounds  Top Games Like the Japanese Epic</u></a></li>
<li><a href="https://screen-activity-recording.techidaily.com/new-best-practices-8-steps-for-digital-sound-preservation/"><u>[New] Best Practices  8 Steps for Digital Sound Preservation</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/updated-evaluating-sns-hdrs-value-and-alternatives-for-hdr-editing/"><u>[Updated] Evaluating SNS HDR's Value & Alternatives for HDR Editing</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/updated-in-2024-a-step-by-step-approach-to-masterful-screen-recordings-on-hp-systems/"><u>[Updated] In 2024, A Step-by-Step Approach to Masterful Screen Recordings on HP Systems</u></a></li>
<li><a href="https://fox-friendly.techidaily.com/updated-in-2024-how-to-transform-your-in-game-voice-and-sound-presence-naturally-expert-tips-for-free/"><u>[Updated] In 2024, How to Transform Your In-Game Voice and Sound Presence Naturally  Expert Tips for FREE</u></a></li>
<li><a href="https://screen-recording.techidaily.com/updated-visual-voyage-amds-radeon-reborn-for-2024/"><u>[Updated] Visual Voyage  AMD's Radeon Reborn for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/1-digital-workforce-evolution-the-driving-force-behind-corporate-change/"><u>1. Digital Workforce Evolution: The Driving Force Behind Corporate Change</u></a></li>
<li><a href="https://howto.techidaily.com/8-ultimate-fixes-for-google-play-your-realme-c67-5g-isnt-compatible-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>8 Ultimate Fixes for Google Play Your Realme C67 5G Isnt Compatible | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/abbau-von-zahlungsverzogerungen-bei-metro-ag-schnellerer-transaktionsfluss-fur-grosshandler-bis-zu-90/"><u>Abbau Von Zahlungsverzögerungen Bei Metro AG: Schnellerer Transaktionsfluss Für Großhändler Bis Zu 90%%</u></a></li>
<li><a href="https://some-techniques.techidaily.com/enhanced-user-experience-with-advanced-tracking-technology/"><u>Enhanced User Experience with Advanced Tracking Technology</u></a></li>
<li><a href="https://some-techniques.techidaily.com/enhanced-web-analytics-with-the-help-of-cookiebot-technology/"><u>Enhanced Web Analytics with the Help of Cookiebot Technology</u></a></li>
<li><a href="https://some-techniques.techidaily.com/enhancing-online-presence-with-advanced-cookiebot-technology/"><u>Enhancing Online Presence with Advanced Cookiebot Technology</u></a></li>
<li><a href="https://some-techniques.techidaily.com/enhancing-online-visibility-through-strategic-webpage-content-mastery/"><u>Enhancing Online Visibility Through Strategic Webpage Content Mastery</u></a></li>
<li><a href="https://some-techniques.techidaily.com/explorez-clairement-tous-les-bienfaits-de-lutilisation-dabbyy-recognition-server-avec-rewalk/"><u>Explorez Clairement Tous Les Bienfaits De L'utilisation D’ABBYY Recognition Server Avec Rewalk</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/how-to-convert-and-transfer-your-kindle-ebooks-to-a-barnes-and-noble-nook-device/"><u>How to Convert and Transfer Your Kindle eBooks to a Barnes & Noble Nook Device</u></a></li>
<li><a href="https://easy-unlock-android.techidaily.com/in-2024-how-to-unlock-realme-v30t-pattern-lock-if-forgotten-6-ways-by-drfone-android/"><u>In 2024, How to Unlock Realme V30T Pattern Lock if Forgotten? 6 Ways</u></a></li>
<li><a href="https://change-location.techidaily.com/in-2024-preparation-to-beat-giovani-in-pokemon-go-for-vivo-x90s-drfone-by-drfone-virtual-android/"><u>In 2024, Preparation to Beat Giovani in Pokemon Go For Vivo X90S | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/integration-of-abbyy-flexicapture-with-paperstream-nx-manager-maximizing-efficiency-for-pfu-applications/"><u>Integration of ABBYY FlexiCapture with PaperStream NX Manager: Maximizing Efficiency for PFU Applications</u></a></li>
<li><a href="https://some-techniques.techidaily.com/leverage-cookiebot-technology-for-advanced-web-analytics-and-personalization/"><u>Leverage Cookiebot Technology for Advanced Web Analytics and Personalization</u></a></li>
<li><a href="https://some-techniques.techidaily.com/leveraging-advanced-analytics-via-cookiebot-integration/"><u>Leveraging Advanced Analytics via Cookiebot Integration</u></a></li>
<li><a href="https://some-techniques.techidaily.com/masterclass-by-abbyy-enhancing-user-engagement-through-innovative-onboarding-techniques/"><u>Masterclass by ABBYY: Enhancing User Engagement Through Innovative Onboarding Techniques</u></a></li>
<li><a href="https://some-techniques.techidaily.com/mastering-e-invoice-management-in-ap-comprehensive-strategies-using-abbyy-software/"><u>Mastering E-Invoice Management in AP: Comprehensive Strategies Using ABBYY Software</u></a></li>
<li><a href="https://some-techniques.techidaily.com/mastering-financial-exposure-a-comprehensive-guide-on-reducing-libor-contract-vulnerabilities/"><u>Mastering Financial Exposure: A Comprehensive Guide on Reducing LIBOR Contract Vulnerabilities</u></a></li>
<li><a href="https://some-techniques.techidaily.com/neueste-entwicklungen-im-handelskredit-bereich-bewaltigen-sie-die-zukunftigen-hindernisse-mit-kreativitat/"><u>Neueste Entwicklungen Im Handelskredit Bereich: Bewältigen Sie Die Zukünftigen Hindernisse Mit Kreativität</u></a></li>
<li><a href="https://some-techniques.techidaily.com/optimize-with-cookiebot-advanced-tracking-solutions-tailored-for-seo-success/"><u>Optimize with Cookiebot: Advanced Tracking Solutions Tailored for SEO Success</u></a></li>
<li><a href="https://some-techniques.techidaily.com/optimized-engagement-with-advanced-analytics-powered-by-cookiebot-technology/"><u>Optimized Engagement with Advanced Analytics - Powered by Cookiebot Technology</u></a></li>
<li><a href="https://some-techniques.techidaily.com/pioneering-intuitive-cross-modal-transport-systems-exploring-innovations-at-abbyy/"><u>Pioneering Intuitive Cross-Modal Transport Systems: Exploring Innovations at ABBYY</u></a></li>
<li><a href="https://vimeo-videos.techidaily.com/secure-your-media-download-vimeo-to-mp4-for-2024/"><u>Secure Your Media  Download Vimeo to MP4 for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/tech-sector-sees-software-automation-workforce-surge-up-50-within-next-24-months-predictions-for-future-growth/"><u>Tech Sector Sees Software Automation Workforce Surge up 50%% Within Next 24 Months: Predictions for Future Growth</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/the-ultimate-5-star-fluids-and-flows-in-video-games/"><u>The Ultimate 5-Star Fluids and Flows in Video Games</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/time-saving-ways-to-log-vimeo-media/"><u>Time-Saving Ways to Log Vimeo Media</u></a></li>
<li><a href="https://some-techniques.techidaily.com/top-7-essential-competencies-needed-for-successful-navigation-of-transit-and-supply-chain-management-on-the-abbyy-platform/"><u>Top 7 Essential Competencies Needed for Successful Navigation of Transit and Supply Chain Management on the ABBYY Platform</u></a></li>
<li><a href="https://some-techniques.techidaily.com/transforming-organizational-strategy-with-digital-intelligence-insights-from-an-abbyy-expert/"><u>Transforming Organizational Strategy with Digital Intelligence: Insights From an ABBYY Expert</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/tutorial-to-change-vivo-y100i-imei-without-root-a-comprehensive-guide-by-drfone-android/"><u>Tutorial to Change Vivo Y100i IMEI without Root A Comprehensive Guide</u></a></li>
<li><a href="https://some-techniques.techidaily.com/ultimate-guide-mastering-the-art-of-effective-web-pages/"><u>Ultimate Guide: Mastering the Art of Effective Web Pages</u></a></li>
<li><a href="https://change-location.techidaily.com/unova-stone-pokemon-go-evolution-list-and-how-catch-them-for-vivo-t2x-5g-drfone-by-drfone-virtual-android/"><u>Unova Stone Pokémon Go Evolution List and How Catch Them For Vivo T2x 5G | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/user-engagement-boost-with-advanced-cookiebot-technology-solutions/"><u>User Engagement Boost with Advanced Cookiebot Technology Solutions</u></a></li>
<li><a href="https://some-techniques.techidaily.com/zentralisierte-digitale-transformation-der-rechtspraxis-erleben-sie-die-innovation-von-norton-rose-llp-mit-abbyy-foto-und-handschriftserkennung/"><u>Zentralisierte Digitale Transformation Der Rechtspraxis: Erleben Sie Die Innovation Von Norton Rose LLP Mit ABBYY Foto- Und Handschriftserkennung</u></a></li>
<li><a href="https://some-techniques.techidaily.com/1724312721327-abbyy/"><u>ヘルスケア業界での効果的なプロセスマイニング技術 - ABBYYブログ</u></a></li>
</ul></div>
