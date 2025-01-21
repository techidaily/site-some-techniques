---
title: "Comprehensive Tutorial: Adjusting System Time and Date with Timedatectl in Linux Systems"
date: 2025-01-15T20:33:19.060Z
updated: 2025-01-21T16:55:55.122Z
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

##  Getting Started With timedatectl

 To see the current data and time and other values, use the `timedatectl` command with the status operator.

timedatectl status

![The output from the tidedatectl command using the status operator](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/01/1-4.png) 

 Actually, you can drop the status and you'll still get the same output.

timedatectl

![The output from the timedatectl command with no operator](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/01/2-4.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/SyMZxS9479s?si=0T6zZpyN2LBftFTM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/_SbYznUy_zY?si=ThBkP934r3mizi48" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Setting the Time Zone

 If you look through the unfiltered list of time zones supported by `timedatectl` you'll see places as well as time zones. To set a time zone you can specify it by name like EST or GMT, or you can pick a location in the same time zone as you, like London or New York.

 Resetting your time zone isn't something you'll be doing often, but perhaps you've moved home or you're working away for a while and want to localize your laptop. If you need to reset your time zone, pick a location in the time zone you want to use.

 We'll set this computer to mountain time, which is the same time zone as Edmonton. We'll then see how the settings have changed.

timedatectl set-timezone "America/Edmonton"

timedatectl

![New time zone and time settings](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/01/6-4.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/gSKkJrJ57EA?si=WDOmInPE9EgQa_tB" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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

 The date and time have changed. Also, note the computer is using a false UTC time. We're also informed that the system clock is not being synchronized and the NTP service is inactive.

 If you have internet access, as soon as you restore the time synchronization service the time is retrieved and all of the details are correctly reset.

sudo systemctl start systemd-timesyncd.service

timedatectl

![Restarting the NTP service and restoring the correct time values](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/01/9-4.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/jvwX82j3ci0?si=gAWoovjXgs3m1d7S" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/1dR4tF3VgyU?si=AJipgqZsNNxsRsBW" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 I think they've made their feelings clear.

 To restore the real-time clock to UTC, use this command:

timedatectl set-local-rtc 0

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/Nyp7-xVwqHA?si=XCuZbpKLFIdrGQQh" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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
<li><a href="https://youtube-webster.techidaily.com/024-approved-scouring-for-meaningful-youtube-discussions/"><u>[New] 2024 Approved Scouring for Meaningful YouTube Discussions</u></a></li>
<li><a href="https://youtube-tips.techidaily.com/udget-friendly-broadcaster-gear-for-video-voyeurs/"><u>[New] Budget-Friendly Broadcaster Gear for Video Voyeurs</u></a></li>
<li><a href="https://instagram-video-files.techidaily.com/new-in-2024-essential-tips-for-utilizing-instagram-story-sections/"><u>[New] In 2024, Essential Tips for Utilizing Instagram Story Sections</u></a></li>
<li><a href="https://facebook-video-recording.techidaily.com/new-simplified-guide-youtube-and-facebook-integration/"><u>[New] Simplified Guide YouTube and Facebook Integration</u></a></li>
<li><a href="https://facebook-video-recording.techidaily.com/new-transforming-your-facebook-history-a-look-back-video-guide/"><u>[New] Transforming Your Facebook History A Look Back Video Guide</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-generate-sharable-gifs-with-a-laugh-twist-giphy/"><u>[Updated] Generate Sharable Gifs with a Laugh Twist, Giphy</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-how-to-download-final-cut-pro-for-free/"><u>[Updated] How to Download Final Cut Pro for Free?</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-in-depth-photo-editing-via-vsco-a-compreeved-guide/"><u>[Updated] In-Depth Photo Editing via VSCO A Compreeved Guide</u></a></li>
<li><a href="https://extra-hints.techidaily.com/2024-approved-a-brief-overview-understanding-vr-jargon/"><u>2024 Approved A Brief Overview Understanding VR Jargon</u></a></li>
<li><a href="https://article-knowledge.techidaily.com/in-2024-affordable-airborium-wonders-best-bargain-drones-list/"><u>In 2024, Affordable Airborium Wonders Best Bargain Drones List</u></a></li>
<li><a href="https://youtube-lab.techidaily.com/24-complete-guidebook-to-evaluating-your-videos-impact-and-earning-power/"><u>In 2024, Complete Guidebook to Evaluating Your Video's Impact and Earning Power</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-how-video-testimonials-shape-perception-and-trust/"><u>In 2024, How Video Testimonials Shape Perception and Trust</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-ingenious-stop-motion-cinema-ranking-the-best-15/"><u>In 2024, Ingenious Stop-Motion Cinema - Ranking the Best 15</u></a></li>
<li><a href="https://ai-video-apps.techidaily.com/new-transform-mp4-videos-into-mp3-audio-files-top-converters-for-2024/"><u>New Transform MP4 Videos Into MP3 Audio Files Top Converters for 2024</u></a></li>
</ul></div>

