---
title: Efficiently Refresh Your Ubuntu's DNS Cache - A Comprehensive Tutorial
date: 2024-11-06T17:28:09.214Z
updated: 2024-11-14T03:00:17.071Z
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
<a href="https://zebaoaffiliateprogram.pxf.io/c/5597632/2137972/21526" target="_top" id="2137972">
  <img src="//a.impactradius-go.com/display-ad/21526-2137972" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://zebaoaffiliateprogram.pxf.io/i/5597632/2137972/21526" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  What Is DNS Caching?

 The [domain name system](https://instagram-clips.techidaily.com/new-2024-approved-revealing-the-top-10-hidden-story-supporters/) (DNS) service eats names and spits out numbers. It’s the service that lets us talk about network names or internet domain names, instead of learning a load of IP addresses. The DNS service translates internet domain names into IP addresses so that our connection requests and network traffic can be directed toward the correct server. Matching names to IP addresses is called _resolving_.

 Internet DNS lookups are cascaded through a hierarchy of servers, known as precursor DNS servers, root name servers, top-level domain servers, and authoritative name servers. Lookups are very fast, but they’re not instantaneous.

 To reduce the time it takes to return an answer to a DNS request, precursor DNS servers cache their most recent queries and answers. If someone has recently made the same DNS request, the server can return that value to your computer without having to involve any of the other servers.

 Your router at home probably caches local network device names and IP addresses, and it may even cache responses from external DNS servers.

 If the answer to a DNS request is found in the precursor server's cache, no further servers need to be contacted. The answer is sent back from the cache. Similarly, if you try to connect to a local network device using its network device name, your router provides the IP address.

 Using cached data might be faster than a full DNS lookup, but it is predicated on the assumption that the stored values are still valid. If the IP address of the website or local network device has changed, your computer won’t be able to talk to it.

 Ubuntu adds its own cache to the mix. By default, the [systemd](https://facebook-clips.techidaily.com/2024-approved-restore-order-fixing-compromised-fb-profile/)\-resolved service is enabled. This caches DNS requests and responses. If a single cache entry (or the whole cache for that matter) becomes corrupted, you can experience connectivity issues with remote servers, web resources, and local devices.

##  What Does Flushing the DNS Cache Do?

 Flushing the DNS cache tells your computer to forget all the stored name and IP address pairs it has collected. That means any connection request that requires resolving from a name to an IP address requires your computer to query an outside source such as your local router or an external DNS service. The response will be cached.

 Over time, your DNS cache will be populated by new entries, some of which are likely to be updated versions of older, stale cache entries. It’s an easy and safe operation. If you ever experience networking or internet flakiness, flushing your DNS cache is a good first step in troubleshooting.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1972698/19272" target="_top" id="1972698">
  <img src="//a.impactradius-go.com/display-ad/19272-1972698" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1972698/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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
<a href="https://dhgate.sjv.io/c/5597632/1172027/12108" target="_top" id="1172027">
  <img src="//a.impactradius-go.com/display-ad/12108-1172027" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://dhgate.sjv.io/i/5597632/1172027/12108" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Because this is a fresh installation of Ubuntu, there are relatively few entries in the cache. Regardless, when we flush the DNS buffers we expect to see that number drop to zero.

resolvectl flush-caches

![Flushing the DNS cache on Ubuntu](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/3-14.png) 

 We’re silently returned to the command line. No output means everything went well. Let’s see what our cache size is now.

resolvectl statistics

![Verifying the DNS cache is empty on Ubuntu](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/4-13.png) 

 Our cache size is zero, just as we predicted.

<!-- affiliate ads begin -->
<a href="https://ephamedtechinc.pxf.io/c/5597632/2137203/26400" target="_top" id="2137203">
  <img src="//a.impactradius-go.com/display-ad/26400-2137203" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://ephamedtechinc.pxf.io/i/5597632/2137203/26400" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Don’t Forget Your Browser's Cache

 Your internet browsers have their own caches. If you’re flushing your DNS buffers to try to remove a problem, make a point of doing the same for your browsers.

###  Flushing the DNS Cache in Firefox

 Open a new tab in Firefox, enter this text in the URL address bar, and hit Enter:

about:networking

![Selecting the DNS option in the Firefox sidebar](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/5-10.png) 

 Click the "DNS" entry in the sidebar.

![The Clear DNS Cache button on Firefox](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/6-10.png) 

 Firefox shows you the most recent entries added to the DNS cache. To clear the cache, click the “Clear DNS Cache” button. I had to refresh the page to see the change, but the cache was definitely purged.

![The Firefox DNS page with no entries, showing the cache has been purged](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/7-11.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1938698/19272" target="_top" id="1938698">
  <img src="//a.impactradius-go.com/display-ad/19272-1938698" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1938698/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

###  Flushing the DNS Cache in Google Chrome

 To do the same operation in Google Chrome, enter this in the URL address bar and hit the Enter key:

chrome://net-internals/#dns

![The Firefox DNS page with no entries, showing the cache has been purged](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/8-10.png) 

 Click the “Clear Host Cache” button. There’s no visible feedback to let you know anything has actually happened, but behind the scenes it has. Google Chrome’s DNS cache has been emptied.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2135401/19272" target="_top" id="2135401">
  <img src="//a.impactradius-go.com/display-ad/19272-2135401" border="0" alt="https://techidaily.com" width="320" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135401/19272" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://screen-capture.techidaily.com/new-2024-approved-lightning-labs-loading-slides-in-ppt/"><u>[New] 2024 Approved Lightning Labs Loading Slides in PPT</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-future-of-animation-unveiled-selection-of-state-of-the-art-modelling-apps/"><u>[New] Future of Animation Unveiled Selection of State-of-the-Art Modelling Apps</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-hearing-beginnings-mastering-volume-control-in-adobe-audition/"><u>[New] Hearing Beginnings Mastering Volume Control in Adobe Audition</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-how-to-use-luts-to-spark-ar-and-download-free-lut/"><u>[New] How to Use LUTs to Spark AR & Download Free LUT</u></a></li>
<li><a href="https://facebook-video-recording.techidaily.com/new-in-2024-facebook-faults-recovering-login-credentials-quickly/"><u>[New] In 2024, Facebook Faults? Recovering Login Credentials Quickly</u></a></li>
<li><a href="https://fox-access.techidaily.com/updated-2024-approved-principles-of-momentum-reversal-in-filming/"><u>[Updated] 2024 Approved Principles of Momentum Reversal in Filming</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-flicker-studio-the-complete-lightroom-alternatives-guide/"><u>[Updated] Flicker Studio The Complete Lightroom Alternatives Guide</u></a></li>
<li><a href="https://win-solutions.techidaily.com/fixing-the-black-screen-of-death-in-resident-evil-village-a-comprehensive-guide/"><u>Fixing the 'Black Screen of Death' In Resident Evil Village: A Comprehensive Guide</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-finding-value-in-sport-photography-cameras-for-the-price-conscious/"><u>In 2024, Finding Value in Sport Photography – Cameras for the Price-Conscious</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-implement-shutter-speed-blurring-in-psx/"><u>In 2024, Implement Shutter Speed Blurring in PSX</u></a></li>
<li><a href="https://fox-direct.techidaily.com/in-2024-metaverse-masterpieces-transforming-images-into-memetic-hits/"><u>In 2024, Metaverse Masterpieces Transforming Images Into Memetic Hits</u></a></li>
<li><a href="https://android-frp.techidaily.com/in-2024-samsung-galaxy-s23plus-adb-format-tool-for-pc-vs-other-unlocking-tools-which-one-is-the-best-by-drfone-android/"><u>In 2024, Samsung Galaxy S23+ ADB Format Tool for PC vs. Other Unlocking Tools Which One is the Best?</u></a></li>
<li><a href="https://data-wizards.techidaily.com/rebuildvidhelper-free-tool-for-vids-in-need/"><u>RebuildVidHelper: Free Tool for Vids in Need</u></a></li>
<li><a href="https://techidaily.com/things-you-dont-know-about-oneplus-ace-2-reset-code-drfone-by-drfone-reset-android-reset-android/"><u>Things You Dont Know About OnePlus Ace 2 Reset Code | Dr.fone</u></a></li>
</ul></div>

