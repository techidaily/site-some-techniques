---
title: Efficiently Refresh Your Ubuntu's DNS Cache - A Comprehensive Tutorial
date: 2024-12-22T21:11:47.548Z
updated: 2024-12-24T17:17:35.881Z
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

##  What Does Flushing the DNS Cache Do?

 Flushing the DNS cache tells your computer to forget all the stored name and IP address pairs it has collected. That means any connection request that requires resolving from a name to an IP address requires your computer to query an outside source such as your local router or an external DNS service. The response will be cached.

 Over time, your DNS cache will be populated by new entries, some of which are likely to be updated versions of older, stale cache entries. It’s an easy and safe operation. If you ever experience networking or internet flakiness, flushing your DNS cache is a good first step in troubleshooting.

##  Flushing the DNS Cache on Ubuntu

 On Ubuntu, the DNS service is on by default. If it’s your computer, and you know you haven’t turned the resolved daemon off, then DNS will be on. It’s easy to check, which is handy if you need to work on someone else’s computer, and they can't tell you whether DNS is on or off.

 The command to use is straightforward. We’re using the systemctl command because we need to check on a part of the systemd collection of utilities, namely systemd-resolved. This is the systemd name resolving daemon.

systemctl is-active systemd-resolved

![Checking whether the resolved daemon is running on Ubuntu](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/1-14.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/9Q8Feep0Rc0?si=YkPhRxXGvrRRMJtb" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 The response will either be “active” or “inactive.”

 To verify that flushing the buffers actually does something, we can take a peek at the number of entries in the cache. We’ll check again, once we’ve flushed the buffers. This time, we’re using the resolvectl command to manipulate systemd-resolved directly.

resolvectl statistics

![Checking the size of the DNS cache on Ubuntu](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/2-15.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/kiW7sLvL65k?si=IHSeRFsYCrfqpn2o" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Because this is a fresh installation of Ubuntu, there are relatively few entries in the cache. Regardless, when we flush the DNS buffers we expect to see that number drop to zero.

resolvectl flush-caches

![Flushing the DNS cache on Ubuntu](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/3-14.png) 

 We’re silently returned to the command line. No output means everything went well. Let’s see what our cache size is now.

resolvectl statistics

![Verifying the DNS cache is empty on Ubuntu](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/4-13.png) 

 Our cache size is zero, just as we predicted.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/UCqHbpxQGP4?si=XGkajFHdqyoKNAFM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Don’t Forget Your Browser's Cache

 Your internet browsers have their own caches. If you’re flushing your DNS buffers to try to remove a problem, make a point of doing the same for your browsers.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/PKZUYice-ws?si=L8iMa9T3h7TMSWdQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/Wy0uYNNdMDM?si=5ir7EHlr0CkpcYOT" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Click the “Clear Host Cache” button. There’s no visible feedback to let you know anything has actually happened, but behind the scenes it has. Google Chrome’s DNS cache has been emptied.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/gkdZ3A1mock?si=2zeR5GtTU2VujM_w" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://some-techniques.techidaily.com/new-find-the-best-online-subtitle-converters-for-no-cost/"><u>[New] Find the Best Online Subtitle Converters for No Cost</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-harness-ai-to-generate-prime-video-titles/"><u>[New] Harness AI to Generate Prime Video Titles</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-hide-your-identity-share-your-life-instagram-live-secrets/"><u>[New] Hide Your Identity, Share Your Life - Instagram Live Secrets</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-expert-timekeeping-tools-without-a-price/"><u>[Updated] Expert Timekeeping Tools Without a Price</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-gigglegallery-log-in-and-make-magic-videos/"><u>[Updated] GiggleGallery Log In and Make Magic Videos</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-how-to-harness-iphones-full-potential-for-landscapes/"><u>[Updated] How to Harness iPhone's Full Potential for Landscapes</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-immerse-in-world-heritage-through-vr/"><u>[Updated] Immerse in World Heritage Through VR</u></a></li>
<li><a href="https://win-solutions.techidaily.com/clogs-and-backups/"><u>Clogs And Backups:</u></a></li>
<li><a href="https://games-able.techidaily.com/discovering-the-power-of-game-mode-in-apples-macos-sonoma-platform/"><u>Discovering the Power of Game Mode in Apple's macOS Sonoma Platform</u></a></li>
<li><a href="https://discover-dash.techidaily.com/easy-diy-method-for-uploading-your-old-vhs-videos-onto-a-dvd-using-your-computer/"><u>Easy DIY Method for Uploading Your Old VHS Videos Onto a DVD Using Your Computer</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-fabricate-jocular-images-share-via-giphy/"><u>In 2024, Fabricate Jocular Images, Share via Giphy</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-first-rate-6-software-for-visual-text-conversion/"><u>In 2024, First-Rate 6 Software for Visual Text Conversion</u></a></li>
<li><a href="https://instagram-video-files.techidaily.com/in-2024-leverage-loops-for-stirring-instagram-engagement-and-likes/"><u>In 2024, Leverage Loops for Stirring Instagram Engagement & Likes</u></a></li>
<li><a href="https://buynow-reviews.techidaily.com/in-depth-look-at-the-microsoft-surface-pro-7-enhanced-efficiency-and-familiar-features/"><u>In-Depth Look at the Microsoft Surface Pro 7: Enhanced Efficiency and Familiar Features</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/theoretical-exploration-rethinking-the-analogy-between-the-internet-and-traditional-libraries/"><u>Theoretical Exploration: Rethinking the Analogy Between the Internet and Traditional Libraries</u></a></li>
<li><a href="https://some-approaches.techidaily.com/transform-messy-scripts-microsoft-onenotes-new-handwriting-smoothing-feature/"><u>Transform Messy Scripts: Microsoft OneNote's New Handwriting Smoothing Feature</u></a></li>
<li><a href="https://tech-hub.techidaily.com/transform-your-interactions-top-9-incentives-that-make-chatgpt-plus-a-must-have-upgrade/"><u>Transform Your Interactions: Top 9 Incentives That Make ChatGPT Plus a Must-Have Upgrade!</u></a></li>
<li><a href="https://solve-luxury.techidaily.com/ultimate-walkthrough-bring-back-life-to-iphone-models-15141312-with-a-simple-icloud-backup-recovery/"><u>Ultimate Walkthrough: Bring Back Life to iPhone Models (15/14/13/12) with a Simple iCloud Backup Recovery</u></a></li>
<li><a href="https://some-approaches.techidaily.com/44k344kn44ki5qmf6io95aplusplus5bplusc44gu54sh5paz44km44kn44ow44kr44ov44ks57ch5y2y44gr44kq44oz44op44kk44oz44gn5asj5oplusb44gz44klic0g44oi44o044kh44ot/"><u>シェア機能対応の無料ウェブカフを簡単にオンラインで変換する - モヴァビ</u></a></li>
</ul></div>

