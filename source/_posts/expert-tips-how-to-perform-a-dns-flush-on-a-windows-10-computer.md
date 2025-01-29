---
title: "Expert Tips: How to Perform a DNS Flush on a Windows 10 Computer"
date: 2025-01-22T20:17:58.407Z
updated: 2025-01-28T23:14:46.915Z
tags:
  - deals
categories:
  - tech
thumbnail: https://thmb.techidaily.com/af6a241ce73781e980e91fb32b5f340b0c43ca449b76945212041b79725c225d.jpg
---

## Expert Tips: How to Perform a DNS Flush on a Windows 10 Computer

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/9hsPbiic0O8?si=58mZ2Cu6wicQfsUP" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

### Quick Links

* [What Does the DNS Cache Do?](https://screen-video-capture.techidaily.com/new-2024-approved-simplified-game-recording-setups-for-stardew-villagers/)
* [Flushing Your DNS Cache](https://facebook-video-share.techidaily.com/updated-swipe-right-on-creativity-youtubes-top-techniques-for-greenscreens/)

### Key Takeaways

* The DNS cache stores information that translates domain names into IP addresses, saving time when you connect to websites.
* Flushing your PC's DNS cache can help fix internet connection issues caused by corrupted, outdated, or poisoned cache.
* To flush your DNS Cache, run "ipconfig /flushdns" in Command Prompt or PowerShell, or just restart your PC.

 A problem with your PC's DNS cache can result in trouble connecting to the internet. If you've tried the usual tricks [like clearing your browser cache and cookies](https://howto.techidaily.com/top-10-fixes-for-phone-keep-disconnecting-from-wi-fi-on-huawei-nova-y71-drfone-by-drfone-fix-android-problems-fix-android-problems/), flushing Windows 10's DNS may fix your problem.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/XA_wP7rS9ww?si=LarMG3sEHAhSoL6q" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  What Does the DNS Cache Do? 

 A [Domain Network System (DNS) server](https://instagram-clips.techidaily.com/new-2024-approved-revealing-the-top-10-hidden-story-supporters/) is what translates familiar domain names like howtogeek.com into the IP addresses computers use to connect with each other. When a program tries to connect to a domain name like google.com or facebook.com, your computer queries a DNS server on the internet to get the corresponding numerical IP address. To save time, Windows 10 stores a copy of the information it gets from DNS servers locally on your PC. This is called the DNS cache.

 Your PC's DNS cache can save time, but if something goes wrong with it, it can cause connection errors. The DNS cache can become corrupted, where the information relating IP addresses to domain names is lost due to a glitch. The cache can also become outdated, meaning that either the domain name or the IP address of the site you're trying to reach has changed since the cache was last updated. The DNS cache can also be poisoned, where it is [given incorrect information by DNS servers](https://vimeo-videos.techidaily.com/new-in-2024-premium-downloader-suite-for-vimeo-content/). DNS cache poisoning can be accidental, but it can also be used maliciously to steal login credentials or other sensitive data.

 The DNS cache affects all internet traffic on your PC, so if you're having trouble with only one program or a single website, the problem probably isn't your DNS cache. If you can't reach a specific website, you can use a tool like [IsItDownRightNow](https://www.isitdownrightnow.com/) to check the website's status. If a single application isn't able to connect to the internet, try [checking your firewall settings](https://screen-mirror.techidaily.com/in-2024-how-to-cast-apple-iphone-7-to-chromecast-drfone-by-drfone-ios/).

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/aknYnDfODro?si=zONIVzA9FFq0rLOD" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Flushing Your DNS Cache

 The DNS cache is not stored as a file on your PC, it is stored in system memory. System memory gets cleared every time your computer powers off, which is part of the reason [why restarting your computer fixes so many problems](https://android-pokemon-go.techidaily.com/in-2024-all-you-need-to-know-about-mega-greninja-for-motorola-moto-g13-drfone-by-drfone-virtual-android/). It also means the simplest way to flush your DNS cache is to restart your PC.

 If you want to manually flush your DNS cache on Windows 10, you can use Command Prompt or Windows PowerShell. Some commands must be "[Run as administrator](https://android-location.techidaily.com/in-2024-10-fake-gps-location-apps-on-android-of-your-samsung-galaxy-xcover-6-pro-tactical-edition-drfone-by-drfone-virtual/)," but it doesn't matter in this case.

 To launch Command Prompt, click the start button, type "cmd" or "command prompt" into the search bar on the Start menu, and then hit Enter.

![Running Command Prompt from the Start Menu.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/11/run-command-prompt.png) 

 Alternatively, you can use Windows PowerShell. Click the Start button, type "powershell" into the search bar in the Start menu, and hit Enter.

![Enter "PowerShell" in the Start Menu search.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/11/run-powershell.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/1rCjQ09iG7s?si=Si1fUBric8MH1VHI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 With either Command Prompt or Windows PowerShell opened, enter the following command:

        `ipconfig /flushdns`
    
 If the DNS cache was flushed, you should see the "Successfully flushed the DNS Resolver Cache" message. You can now close the window.

 If you're using PowerShell 5 (which is still default on Windows 10) your Window will be blue instead of black. 

![The DNS Cache has been flushed successfully in PowerShell.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/11/flush-dns-powershell.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/o-sRtqHdEYY?si=NMTMQVxJsUaoguqh" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 You can now test the websites or application you were having problems with. Is it working? If you're still experiencing problems, you'll have to try [other internet connection troubleshooting steps](https://article-posts.techidaily.com/pioneering-medical-messaging-in-digital-advertising/).

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
<li><a href="https://vimeo-videos.techidaily.com/new-2024-approved-captioning-videos-efficiently-on-vimeo-platform/"><u>[New] 2024 Approved Captioning Videos Efficiently on Vimeo Platform</u></a></li>
<li><a href="https://fox-cloud.techidaily.com/new-tiktok-linking-made-simple-and-irreversible-for-2024/"><u>[New] TikTok Linking Made Simple and Irreversible for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-top-handheld-video-stabilizer-equipment-to-help-shoot-smooth-scenes/"><u>[New] Top Handheld Video Stabilizer Equipment To Help Shoot Smooth Scenes</u></a></li>
<li><a href="https://video-capture.techidaily.com/updated-2024-approved-live-video-logging-on-mac-free/"><u>[Updated] 2024 Approved Live Video Logging on Mac, Free</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-illuminating-your-android-videos-a-quick-guide/"><u>[Updated] Illuminating Your Android Videos A Quick Guide</u></a></li>
<li><a href="https://fox-hovers.techidaily.com/updated-transcendence-in-music-mixing-crossfade-unveiled/"><u>[Updated] Transcendence in Music Mixing Crossfade Unveiled</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-explore-uncharted-territories-with-these-iphone-vr-apps/"><u>2024 Approved Explore Uncharted Territories with These iPhone VR Apps</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-exploring-the-realm-of-physical-interaction-tech/"><u>2024 Approved Exploring the Realm of Physical Interaction Tech</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-filming-availability-pledge-downloading-rights/"><u>2024 Approved Filming Availability Pledge Downloading Rights</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-find-the-perfect-phone-shot-blur/"><u>2024 Approved Find the Perfect Phone Shot Blur</u></a></li>
<li><a href="https://youtube-tips.techidaily.com/ing-your-youtube-earnings-strategies-for-monetizing-short-videos/"><u>Boosting Your YouTube Earnings Strategies for Monetizing Short Videos</u></a></li>
<li><a href="https://technical-tips.techidaily.com/exploring-ios-16-tips-for-leveraging-the-upgraded-lock-screen-on-your-iphone-cnet-guides/"><u>Exploring IOS 16: Tips for Leveraging the Upgraded Lock Screen on Your iPhone | CNET Guides</u></a></li>
<li><a href="https://some-techniques.techidaily.com/fast-track-choosing-best-pc-game-speed-extensions-for-2024/"><u>Fast Track Choosing Best PC Game Speed Extensions for 2024</u></a></li>
<li><a href="https://easy-unlock-android.techidaily.com/forgot-pattern-lock-heres-how-you-can-unlock-oppo-reno-10-pro-5g-pattern-lock-screen-by-drfone-android/"><u>Forgot Pattern Lock? Heres How You Can Unlock Oppo Reno 10 Pro 5G Pattern Lock Screen</u></a></li>
<li><a href="https://change-location.techidaily.com/in-2024-5-best-route-generator-apps-you-should-try-on-xiaomi-redmi-note-12t-pro-drfone-by-drfone-virtual-android/"><u>In 2024, 5 Best Route Generator Apps You Should Try On Xiaomi Redmi Note 12T Pro | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-fabricate-funny-face-filters-giphy-style/"><u>In 2024, Fabricate Funny Face Filters Giphy Style</u></a></li>
<li><a href="https://unlock-android.techidaily.com/in-2024-top-4-sim-location-trackers-to-easily-find-your-lost-tecno-camon-20-device-by-drfone-android/"><u>In 2024, Top 4 SIM Location Trackers To Easily Find Your Lost Tecno Camon 20 Device</u></a></li>
</ul></div>

