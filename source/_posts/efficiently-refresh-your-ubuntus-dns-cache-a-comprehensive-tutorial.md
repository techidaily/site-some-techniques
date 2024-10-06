---
title: Efficiently Refresh Your Ubuntu's DNS Cache - A Comprehensive Tutorial
date: 2024-10-02T21:11:51.269Z
updated: 2024-10-06T01:14:05.361Z
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

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2144274/7443" target="_top" id="2144274">
  <img src="//a.impactradius-go.com/display-ad/7443-2144274" border="0" alt="https://techidaily.com" width="600" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2144274/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  What Is DNS Caching?

 The [domain name system](https://instagram-clips.techidaily.com/new-2024-approved-revealing-the-top-10-hidden-story-supporters/) (DNS) service eats names and spits out numbers. It’s the service that lets us talk about network names or internet domain names, instead of learning a load of IP addresses. The DNS service translates internet domain names into IP addresses so that our connection requests and network traffic can be directed toward the correct server. Matching names to IP addresses is called _resolving_.

 Internet DNS lookups are cascaded through a hierarchy of servers, known as precursor DNS servers, root name servers, top-level domain servers, and authoritative name servers. Lookups are very fast, but they’re not instantaneous.

 To reduce the time it takes to return an answer to a DNS request, precursor DNS servers cache their most recent queries and answers. If someone has recently made the same DNS request, the server can return that value to your computer without having to involve any of the other servers.

 Your router at home probably caches local network device names and IP addresses, and it may even cache responses from external DNS servers.

 If the answer to a DNS request is found in the precursor server's cache, no further servers need to be contacted. The answer is sent back from the cache. Similarly, if you try to connect to a local network device using its network device name, your router provides the IP address.

 Using cached data might be faster than a full DNS lookup, but it is predicated on the assumption that the stored values are still valid. If the IP address of the website or local network device has changed, your computer won’t be able to talk to it.

 Ubuntu adds its own cache to the mix. By default, the [systemd](https://facebook-clips.techidaily.com/2024-approved-restore-order-fixing-compromised-fb-profile/)\-resolved service is enabled. This caches DNS requests and responses. If a single cache entry (or the whole cache for that matter) becomes corrupted, you can experience connectivity issues with remote servers, web resources, and local devices.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1902319/19272" target="_top" id="1902319">
  <img src="//a.impactradius-go.com/display-ad/19272-1902319" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1902319/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  What Does Flushing the DNS Cache Do?

 Flushing the DNS cache tells your computer to forget all the stored name and IP address pairs it has collected. That means any connection request that requires resolving from a name to an IP address requires your computer to query an outside source such as your local router or an external DNS service. The response will be cached.

 Over time, your DNS cache will be populated by new entries, some of which are likely to be updated versions of older, stale cache entries. It’s an easy and safe operation. If you ever experience networking or internet flakiness, flushing your DNS cache is a good first step in troubleshooting.

##  Flushing the DNS Cache on Ubuntu

 On Ubuntu, the DNS service is on by default. If it’s your computer, and you know you haven’t turned the resolved daemon off, then DNS will be on. It’s easy to check, which is handy if you need to work on someone else’s computer, and they can't tell you whether DNS is on or off.

 The command to use is straightforward. We’re using the systemctl command because we need to check on a part of the systemd collection of utilities, namely systemd-resolved. This is the systemd name resolving daemon.

systemctl is-active systemd-resolved

![Checking whether the resolved daemon is running on Ubuntu](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/1-14.png) 

 The response will either be “active” or “inactive.”

 To verify that flushing the buffers actually does something, we can take a peek at the number of entries in the cache. We’ll check again, once we’ve flushed the buffers. This time, we’re using the resolvectl command to manipulate systemd-resolved directly.

resolvectl statistics

![Checking the size of the DNS cache on Ubuntu](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/2-15.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2151866/7443" target="_top" id="2151866">
  <img src="//a.impactradius-go.com/display-ad/7443-2151866" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2151866/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Because this is a fresh installation of Ubuntu, there are relatively few entries in the cache. Regardless, when we flush the DNS buffers we expect to see that number drop to zero.

resolvectl flush-caches

![Flushing the DNS cache on Ubuntu](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/3-14.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1885947/19272" target="_top" id="1885947">
  <img src="//a.impactradius-go.com/display-ad/19272-1885947" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1885947/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 We’re silently returned to the command line. No output means everything went well. Let’s see what our cache size is now.

resolvectl statistics

![Verifying the DNS cache is empty on Ubuntu](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/4-13.png) 

 Our cache size is zero, just as we predicted.

##  Don’t Forget Your Browser's Cache

 Your internet browsers have their own caches. If you’re flushing your DNS buffers to try to remove a problem, make a point of doing the same for your browsers.

<!-- affiliate ads begin -->
<a href="https://versadesk.pxf.io/c/5597632/1828647/21290" target="_top" id="1828647">
  <img src="//a.impactradius-go.com/display-ad/21290-1828647" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://versadesk.pxf.io/i/5597632/1828647/21290" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

###  Flushing the DNS Cache in Firefox

 Open a new tab in Firefox, enter this text in the URL address bar, and hit Enter:

about:networking

![Selecting the DNS option in the Firefox sidebar](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/5-10.png) 

 Click the "DNS" entry in the sidebar.

![The Clear DNS Cache button on Firefox](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/6-10.png) 

 Firefox shows you the most recent entries added to the DNS cache. To clear the cache, click the “Clear DNS Cache” button. I had to refresh the page to see the change, but the cache was definitely purged.

![The Firefox DNS page with no entries, showing the cache has been purged](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/7-11.png) 

###  Flushing the DNS Cache in Google Chrome

 To do the same operation in Google Chrome, enter this in the URL address bar and hit the Enter key:

chrome://net-internals/#dns

![The Firefox DNS page with no entries, showing the cache has been purged](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/8-10.png) 

 Click the “Clear Host Cache” button. There’s no visible feedback to let you know anything has actually happened, but behind the scenes it has. Google Chrome’s DNS cache has been emptied.

<!-- affiliate ads begin -->
<a href="https://wigfever.sjv.io/c/5597632/2014854/22899" target="_top" id="2014854">
  <img src="//a.impactradius-go.com/display-ad/22899-2014854" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://wigfever.sjv.io/i/5597632/2014854/22899" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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
<li><a href="https://remote-screen-capture.techidaily.com/updated-comprehensive-mp4-video-downloader-review-for-2024/"><u>[Updated] Comprehensive MP4 Video Downloader Review for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-explore-virtual-worlds-pcs-1-list-of-vr-360-game-streamers/"><u>[Updated] Explore Virtual Worlds PC's #1 List of VR 360 Game Streamers</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-incorporating-side-content-a-filmmakers-guide/"><u>[Updated] Incorporating Side Content A Filmmaker's Guide</u></a></li>
<li><a href="https://some-approaches.techidaily.com/updated-the-peak-of-data-preservation-cloud-service-guide/"><u>[Updated] The Peak of Data Preservation Cloud Service Guide</u></a></li>
<li><a href="https://howto.techidaily.com/7-solutions-to-fix-chrome-crashes-or-wont-open-on-itel-a05s-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>7 Solutions to Fix Chrome Crashes or Wont Open on Itel A05s | Dr.fone</u></a></li>
<li><a href="https://hardware-help.techidaily.com/essential-z370p-d3-motherboard-drivers-secure-and-fast-download-options/"><u>Essential Z370P D3 Motherboard Drivers – Secure & Fast Download Options</u></a></li>
<li><a href="https://some-techniques.techidaily.com/fists-vs-followers-choosing-the-champion-for-2024/"><u>Fists vs Followers Choosing the Champion for 2024</u></a></li>
<li><a href="https://win-howtos.techidaily.com/how-to-restore-functionality-of-your-steelseries-arctis-5s-built-in-mic/"><u>How to Restore Functionality of Your SteelSeries Arctis 5'S Built-In Mic</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-extract-srt-from-zip-simple-subtitle-file-creation-tips/"><u>In 2024, Extract SRT From ZIP Simple Subtitle File Creation Tips</u></a></li>
<li><a href="https://mondly-stories.techidaily.com/1719576550079-mondly-is-now-available-on-huawei-appgallery/"><u>Mondly Is Now Available On Huawei AppGallery</u></a></li>
<li><a href="https://extra-information.techidaily.com/muzik-pathway-tamil-music-to-your-phones-chime/"><u>Muzik Pathway Tamil Music to Your Phone's Chime</u></a></li>
<li><a href="https://youtube-zero.techidaily.com/nstagram-way-of-showcasing-youtube-videos-for-2024/"><u>The Instagram Way of Showcasing YouTube Videos for 2024</u></a></li>
<li><a href="https://win-blog.techidaily.com/warzone-screen-tearing-effective-solutions-and-fixes/"><u>Warzone Screen Tearing: Effective Solutions & Fixes</u></a></li>
</ul></div>

