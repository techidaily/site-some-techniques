---
title: Efficiently Refresh Your Ubuntu's DNS Cache - A Comprehensive Tutorial
date: 2024-11-29T00:56:52.344Z
updated: 2024-12-02T04:25:13.048Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/12/case-bash.jpg
---

## Efficiently Refresh Your Ubuntu's DNS Cache - A Comprehensive Tutorial

### Quick Links

* [What Is DNS Caching?](https://iphone-unlock.techidaily.com/3-easy-ways-to-factory-reset-a-locked-apple-iphone-x-without-itunes-drfone-by-drfone-ios/)
* [What Does Flushing the DNS Cache Do?](https://location-fake.techidaily.com/8-solutions-to-fix-find-my-friends-location-not-available-on-honor-70-lite-5g-drfone-by-drfone-virtual-android/)
* [Flushing the DNS Cache on Ubuntu](https://vimeo-videos.techidaily.com/updated-in-2024-the-complete-guide-to-earnings-via-vimeo-ads/)
* [Don’t Forget Your Browser's Cache](https://youtube-tips.techidaily.com/ed-2024-approved-brightening-up-your-youtube-pixels/)
* [Remember to Flush Your DNS Cache](https://some-knowledge.techidaily.com/new-full-exploration-of-picsarts-new-features/)

### Key Takeaways

* Flushing the DNS cache on Ubuntu with "resolvectl flush-caches" can help troubleshoot connectivity issues and improve network performance.
* DNS caching reduces the time it takes to return DNS requests, but outdated or corrupt entries will cause problems.
* Remember to also clear the DNS cache in your internet browsers to ensure all cached data is cleared for troubleshooting.

 The domain name resolving service is enabled by default in Ubuntu. That’s fine, it performs a useful service. But it’s worth periodically flushing its buffers, especially if you get flaky connectivity.

##  What Is DNS Caching?

 The [domain name system](https://instagram-clips.techidaily.com/new-2024-approved-revealing-the-top-10-hidden-story-supporters/) (DNS) service eats names and spits out numbers. It’s the service that lets us talk about network names or internet domain names, instead of learning a load of IP addresses. The DNS service translates internet domain names into IP addresses so that our connection requests and network traffic can be directed toward the correct server. Matching names to IP addresses is called _resolving_.

 Internet DNS lookups are cascaded through a hierarchy of servers, known as precursor DNS servers, root name servers, top-level domain servers, and authoritative name servers. Lookups are very fast, but they’re not instantaneous.

 To reduce the time it takes to return an answer to a DNS request, precursor DNS servers cache their most recent queries and answers. If someone has recently made the same DNS request, the server can return that value to your computer without having to involve any of the other servers.

 Your router at home probably caches local network device names and IP addresses, and it may even cache responses from external DNS servers.

 If the answer to a DNS request is found in the precursor server's cache, no further servers need to be contacted. The answer is sent back from the cache. Similarly, if you try to connect to a local network device using its network device name, your router provides the IP address.

 Using cached data might be faster than a full DNS lookup, but it is predicated on the assumption that the stored values are still valid. If the IP address of the website or local network device has changed, your computer won’t be able to talk to it.

 Ubuntu adds its own cache to the mix. By default, the [systemd](https://facebook-clips.techidaily.com/2024-approved-restore-order-fixing-compromised-fb-profile/)\-resolved service is enabled. This caches DNS requests and responses. If a single cache entry (or the whole cache for that matter) becomes corrupted, you can experience connectivity issues with remote servers, web resources, and local devices.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/9Sj2QNA-JXI?si=V-_h73iE3VlE214k" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  What Does Flushing the DNS Cache Do?

 Flushing the DNS cache tells your computer to forget all the stored name and IP address pairs it has collected. That means any connection request that requires resolving from a name to an IP address requires your computer to query an outside source such as your local router or an external DNS service. The response will be cached.

 Over time, your DNS cache will be populated by new entries, some of which are likely to be updated versions of older, stale cache entries. It’s an easy and safe operation. If you ever experience networking or internet flakiness, flushing your DNS cache is a good first step in troubleshooting.

##  Flushing the DNS Cache on Ubuntu

 On Ubuntu, the DNS service is on by default. If it’s your computer, and you know you haven’t turned the resolved daemon off, then DNS will be on. It’s easy to check, which is handy if you need to work on someone else’s computer, and they can't tell you whether DNS is on or off.

 The command to use is straightforward. We’re using the systemctl command because we need to check on a part of the systemd collection of utilities, namely systemd-resolved. This is the systemd name resolving daemon.

systemctl is-active systemd-resolved

![Checking whether the resolved daemon is running on Ubuntu](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/1-14.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/kiW7sLvL65k?si=IHSeRFsYCrfqpn2o" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 The response will either be “active” or “inactive.”

 To verify that flushing the buffers actually does something, we can take a peek at the number of entries in the cache. We’ll check again, once we’ve flushed the buffers. This time, we’re using the resolvectl command to manipulate systemd-resolved directly.

resolvectl statistics

![Checking the size of the DNS cache on Ubuntu](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/2-15.png) 

 Because this is a fresh installation of Ubuntu, there are relatively few entries in the cache. Regardless, when we flush the DNS buffers we expect to see that number drop to zero.

resolvectl flush-caches

![Flushing the DNS cache on Ubuntu](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/3-14.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/jvwX82j3ci0?si=gAWoovjXgs3m1d7S" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 We’re silently returned to the command line. No output means everything went well. Let’s see what our cache size is now.

resolvectl statistics

![Verifying the DNS cache is empty on Ubuntu](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/4-13.png) 

 Our cache size is zero, just as we predicted.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/May-pLCUkEA?si=PGlcFZAlsp3S3beI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Don’t Forget Your Browser's Cache

 Your internet browsers have their own caches. If you’re flushing your DNS buffers to try to remove a problem, make a point of doing the same for your browsers.

###  Flushing the DNS Cache in Firefox

 Open a new tab in Firefox, enter this text in the URL address bar, and hit Enter:

about:networking

![Selecting the DNS option in the Firefox sidebar](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/5-10.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/sXLLPY11of0?si=-3YNnpnO0wbc0K_-" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Click the "DNS" entry in the sidebar.

![The Clear DNS Cache button on Firefox](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/6-10.png) 

 Firefox shows you the most recent entries added to the DNS cache. To clear the cache, click the “Clear DNS Cache” button. I had to refresh the page to see the change, but the cache was definitely purged.

![The Firefox DNS page with no entries, showing the cache has been purged](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/7-11.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/Q-mXUpVQijU?si=f1MzflPJ8-bD2_iQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

###  Flushing the DNS Cache in Google Chrome

 To do the same operation in Google Chrome, enter this in the URL address bar and hit the Enter key:

chrome://net-internals/#dns

![The Firefox DNS page with no entries, showing the cache has been purged](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/8-10.png) 

 Click the “Clear Host Cache” button. There’s no visible feedback to let you know anything has actually happened, but behind the scenes it has. Google Chrome’s DNS cache has been emptied.

##  Remember to Flush Your DNS Cache

 Corrupt or wrong DNS entries can be the root cause of many unwanted networking behaviors. If you’re trying to isolate the issue, flushing your DNS buffers will remove them from the list of possibilities.

 It’s easy to do, so it makes sense to do it as a first step. And with a bit of luck, your issue might be solved.

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
<li><a href="https://youtube-zero.techidaily.com/024-approved-transform-your-videos-expert-choices-for-thumbnails/"><u>[New] 2024 Approved Transform Your Videos Expert Choices for Thumbnails</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-explore-the-depths-of-video-clarity-comprehensive-guide-to-vce-22/"><u>[New] Explore the Depths of Video Clarity - Comprehensive Guide to VCE 2.2</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-high-end-humor-scripts/"><u>[New] High-End Humor Scripts</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-finding-the-best-fit-essential-tips-to-choose-your-ideal-4k-monitor/"><u>[Updated] Finding the Best Fit Essential Tips to Choose Your Ideal 4K Monitor</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-free-iphones-masterclass-perfect-your-pictures-with-simple-edits/"><u>2024 Approved FREE iPhones Masterclass Perfect Your Pictures with Simple Edits</u></a></li>
<li><a href="https://some-techniques.techidaily.com/explore-the-highest-rated-virtual-reality-games-for-2024/"><u>Explore the Highest-Rated Virtual Reality Games for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-exclusive-selection-of-high-caliber-free-luts/"><u>In 2024, Exclusive Selection of High-Caliber Free LUTs</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-expert-advice-where-to-download-high-quality-background-music/"><u>In 2024, Expert Advice Where to Download High-Quality Background Music</u></a></li>
<li><a href="https://bypass-frp.techidaily.com/in-2024-top-5-tecno-pova-5-pro-bypass-frp-tools-for-pc-that-actually-work-by-drfone-android/"><u>In 2024, Top 5 Tecno Pova 5 Pro Bypass FRP Tools for PC That Actually Work</u></a></li>
<li><a href="https://some-skills.techidaily.com/in-2024-transitioning-from-sierra-to-legacy-os-el-capitan/"><u>In 2024, Transitioning From Sierra To Legacy OS - El Capitan</u></a></li>
<li><a href="https://fox-info.techidaily.com/logo-design-101-tips-to-make-your-podcast-stand-out/"><u>Logo Design 101 Tips to Make Your Podcast Stand Out</u></a></li>
<li><a href="https://howto.techidaily.com/reasons-for-nubia-red-magic-9-proplus-stuck-on-startup-screen-and-ways-to-fix-them-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>Reasons for Nubia Red Magic 9 Pro+ Stuck on Startup Screen and Ways To Fix Them | Dr.fone</u></a></li>
<li><a href="https://hardware-help.techidaily.com/step-by-step-guide-to-downloading-and-installing-aoc-monitor-drivers-on-windows-versions-11108/"><u>Step-by-Step Guide to Downloading and Installing AOC Monitor Drivers on Windows (Versions 11/10/8)</u></a></li>
<li><a href="https://tech-renaissance.techidaily.com/top-7-entertaining-web-based-adventures-for-children/"><u>Top 7 Entertaining Web-Based Adventures for Children</u></a></li>
<li><a href="https://win-awesome.techidaily.com/troubleshooting-addressing-the-issue-of-unavailable-disks-for-backup-storage-solutions/"><u>Troubleshooting: Addressing the Issue of Unavailable Disks for Backup Storage Solutions</u></a></li>
<li><a href="https://vp-tips.techidaily.com/unlocking-todays-insights-new-york-times-puzzle-405-solutions-and-analysis/"><u>Unlocking Today's Insights: New York Times Puzzle #405 - Solutions & Analysis</u></a></li>
</ul></div>

