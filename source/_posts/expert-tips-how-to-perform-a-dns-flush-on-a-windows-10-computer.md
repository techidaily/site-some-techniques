---
title: "Expert Tips: How to Perform a DNS Flush on a Windows 10 Computer"
date: 2024-11-18T02:13:21.512Z
updated: 2024-11-23T23:19:51.126Z
tags:
  - deals
categories:
  - tech
thumbnail: https://thmb.techidaily.com/af6a241ce73781e980e91fb32b5f340b0c43ca449b76945212041b79725c225d.jpg
---

## Expert Tips: How to Perform a DNS Flush on a Windows 10 Computer

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/LW6wNx3XAj8?si=VaIuFIIx8MM_RhUR&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

### Quick Links

* [What Does the DNS Cache Do?](https://screen-video-capture.techidaily.com/new-2024-approved-simplified-game-recording-setups-for-stardew-villagers/)
* [Flushing Your DNS Cache](https://facebook-video-share.techidaily.com/updated-swipe-right-on-creativity-youtubes-top-techniques-for-greenscreens/)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/0dOfcihxjiw?si=_fkp1S1Uw0N1dp6b&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

### Key Takeaways

* The DNS cache stores information that translates domain names into IP addresses, saving time when you connect to websites.
* Flushing your PC's DNS cache can help fix internet connection issues caused by corrupted, outdated, or poisoned cache.
* To flush your DNS Cache, run "ipconfig /flushdns" in Command Prompt or PowerShell, or just restart your PC.

 A problem with your PC's DNS cache can result in trouble connecting to the internet. If you've tried the usual tricks [like clearing your browser cache and cookies](https://howto.techidaily.com/top-10-fixes-for-phone-keep-disconnecting-from-wi-fi-on-huawei-nova-y71-drfone-by-drfone-fix-android-problems-fix-android-problems/), flushing Windows 10's DNS may fix your problem.

##  What Does the DNS Cache Do? 

 A [Domain Network System (DNS) server](https://instagram-clips.techidaily.com/new-2024-approved-revealing-the-top-10-hidden-story-supporters/) is what translates familiar domain names like howtogeek.com into the IP addresses computers use to connect with each other. When a program tries to connect to a domain name like google.com or facebook.com, your computer queries a DNS server on the internet to get the corresponding numerical IP address. To save time, Windows 10 stores a copy of the information it gets from DNS servers locally on your PC. This is called the DNS cache.

 Your PC's DNS cache can save time, but if something goes wrong with it, it can cause connection errors. The DNS cache can become corrupted, where the information relating IP addresses to domain names is lost due to a glitch. The cache can also become outdated, meaning that either the domain name or the IP address of the site you're trying to reach has changed since the cache was last updated. The DNS cache can also be poisoned, where it is [given incorrect information by DNS servers](https://vimeo-videos.techidaily.com/new-in-2024-premium-downloader-suite-for-vimeo-content/). DNS cache poisoning can be accidental, but it can also be used maliciously to steal login credentials or other sensitive data.

 The DNS cache affects all internet traffic on your PC, so if you're having trouble with only one program or a single website, the problem probably isn't your DNS cache. If you can't reach a specific website, you can use a tool like [IsItDownRightNow](https://www.isitdownrightnow.com/) to check the website's status. If a single application isn't able to connect to the internet, try [checking your firewall settings](https://screen-mirror.techidaily.com/in-2024-how-to-cast-apple-iphone-7-to-chromecast-drfone-by-drfone-ios/).

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/XoC2TGp1PLY?si=iH9xs76NhWn4pP-E&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Flushing Your DNS Cache

 The DNS cache is not stored as a file on your PC, it is stored in system memory. System memory gets cleared every time your computer powers off, which is part of the reason [why restarting your computer fixes so many problems](https://android-pokemon-go.techidaily.com/in-2024-all-you-need-to-know-about-mega-greninja-for-motorola-moto-g13-drfone-by-drfone-virtual-android/). It also means the simplest way to flush your DNS cache is to restart your PC.

 If you want to manually flush your DNS cache on Windows 10, you can use Command Prompt or Windows PowerShell. Some commands must be "[Run as administrator](https://android-location.techidaily.com/in-2024-10-fake-gps-location-apps-on-android-of-your-samsung-galaxy-xcover-6-pro-tactical-edition-drfone-by-drfone-virtual/)," but it doesn't matter in this case.

 To launch Command Prompt, click the start button, type "cmd" or "command prompt" into the search bar on the Start menu, and then hit Enter.

![Running Command Prompt from the Start Menu.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/11/run-command-prompt.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/c17xsnbinCQ?si=xHKslFgC3QbxY4qW&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Alternatively, you can use Windows PowerShell. Click the Start button, type "powershell" into the search bar in the Start menu, and hit Enter.

![Enter "PowerShell" in the Start Menu search.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/11/run-powershell.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/W5aJC8okA8s?si=L2rnYAp-gmGlLQSf&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 With either Command Prompt or Windows PowerShell opened, enter the following command:

        `ipconfig /flushdns`
    
 If the DNS cache was flushed, you should see the "Successfully flushed the DNS Resolver Cache" message. You can now close the window.

 If you're using PowerShell 5 (which is still default on Windows 10) your Window will be blue instead of black. 

![The DNS Cache has been flushed successfully in PowerShell.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/11/flush-dns-powershell.png) 

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
<li><a href="https://fox-hovers.techidaily.com/new-2024-approved-soaring-sights-dissecting-the-gopro-karma-drones-features/"><u>[New] 2024 Approved Soaring Sights Dissecting the GoPro Karma Drone's Features</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-finding-the-right-balance-essential-points-for-lens-shopping/"><u>[New] Finding the Right Balance Essential Points for Lens Shopping</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-future-proof-cameras-top-2024-choices/"><u>[New] Future-Proof Cameras Top 2024 Choices</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-in-depth-analysis-kinemaster-app-transform-your-gaming-world/"><u>[New] In-Depth Analysis KineMaster App - Transform Your Gaming World</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-in-depth-look-at-final-cut-pro-functions-and-features/"><u>[New] In-Depth Look at Final Cut Pro Functions and Features</u></a></li>
<li><a href="https://facebook-videos.techidaily.com/updated-uniting-platforms-efficiently-share-fb-videos-to-whatsapp-for-2024/"><u>[Updated] Uniting Platforms Efficiently Share FB Videos to WhatsApp for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-gigabytes-needed-for-a-full-days-movie-watching/"><u>2024 Approved Gigabytes Needed for a Full Day's Movie Watching</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-how-augmentation-changes-our-reality-view/"><u>2024 Approved How Augmentation Changes Our Reality View</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-in-depth-look-is-inshot-the-premier-editing-tool/"><u>2024 Approved In-Depth Look Is InShot the Premier Editing Tool?</u></a></li>
<li><a href="https://data-recovery.techidaily.com/confidently-comeback-lost-data-on-ios-devices/"><u>Confidently Comeback Lost Data on iOS Devices</u></a></li>
<li><a href="https://fix-guide.techidaily.com/edit-and-send-fake-location-on-telegram-for-your-zte-nubia-z60-ultra-in-3-ways-drfone-by-drfone-virtual-android/"><u>Edit and Send Fake Location on Telegram For your ZTE Nubia Z60 Ultra in 3 Ways | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/explore-the-depths-of-video-clarity-comprehensive-guide-to-vce-22-for-2024/"><u>Explore the Depths of Video Clarity - Comprehensive Guide to VCE 2.2 for 2024</u></a></li>
<li><a href="https://android-location-track.techidaily.com/in-2024-best-anti-tracker-software-for-oppo-reno-11-5g-drfone-by-drfone-virtual-android/"><u>In 2024, Best Anti Tracker Software For Oppo Reno 11 5G | Dr.fone</u></a></li>
<li><a href="https://youtube-webster.techidaily.com/24-decoding-ad-revenue-distribution-in-youtubes-economic-model/"><u>In 2024, Decoding Ad Revenue Distribution in YouTube's Economic Model</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-image-banking-securing-premium-stock-graphics/"><u>In 2024, Image Banking Securing Premium Stock Graphics</u></a></li>
<li><a href="https://facebook-videos.techidaily.com/in-2024-the-animation-advantage-boosting-profits-in-social-media-ads/"><u>In 2024, The Animation Advantage Boosting Profits in Social Media Ads</u></a></li>
<li><a href="https://youtube-data.techidaily.com/24-top-5-youtube-video-editor-alternatives/"><u>In 2024, Top 5 YouTube Video Editor Alternatives</u></a></li>
<li><a href="https://ai-topics.techidaily.com/new-in-2024-how-to-generate-speech-from-text-the-best-text-to-speech-converters/"><u>New In 2024, How To Generate Speech From Text | The Best Text-to-Speech Converters</u></a></li>
<li><a href="https://buynow-reviews.techidaily.com/the-most-advanced-netgear-routers-launched-consumers/"><u>The Most Advanced Netgear Routers Launched Consumers</u></a></li>
</ul></div>

