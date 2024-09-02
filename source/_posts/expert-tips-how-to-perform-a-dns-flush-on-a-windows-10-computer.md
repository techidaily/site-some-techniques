---
title: "Expert Tips: How to Perform a DNS Flush on a Windows 10 Computer"
date: 2024-09-01T01:23:14.003Z
updated: 2024-09-02T01:23:14.003Z
tags:
  - deals
categories:
  - tech
thumbnail: https://thmb.techidaily.com/af6a241ce73781e980e91fb32b5f340b0c43ca449b76945212041b79725c225d.jpg
---

## Expert Tips: How to Perform a DNS Flush on a Windows 10 Computer

### Quick Links

* [What Does the DNS Cache Do?](https://screen-video-capture.techidaily.com/new-2024-approved-simplified-game-recording-setups-for-stardew-villagers/)
* [Flushing Your DNS Cache](https://facebook-video-share.techidaily.com/updated-swipe-right-on-creativity-youtubes-top-techniques-for-greenscreens/)

### Key Takeaways

* The DNS cache stores information that translates domain names into IP addresses, saving time when you connect to websites.
* Flushing your PC's DNS cache can help fix internet connection issues caused by corrupted, outdated, or poisoned cache.
* To flush your DNS Cache, run "ipconfig /flushdns" in Command Prompt or PowerShell, or just restart your PC.

 A problem with your PC's DNS cache can result in trouble connecting to the internet. If you've tried the usual tricks [like clearing your browser cache and cookies](https://howto.techidaily.com/top-10-fixes-for-phone-keep-disconnecting-from-wi-fi-on-huawei-nova-y71-drfone-by-drfone-fix-android-problems-fix-android-problems/), flushing Windows 10's DNS may fix your problem.

<!-- affiliate ads begin -->
<a href="https://shop.copernic.com/order/checkout.php?PRODS=41033101&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.2checkout.com/images/merchant/8d30aa96e72440759f74bd2306c1fa3d/Copernic-2023-Affiliate-728x90-Elite.png" border="0"></a>
<!-- affiliate ads end -->
##  What Does the DNS Cache Do? 

 A [Domain Network System (DNS) server](https://instagram-clips.techidaily.com/new-2024-approved-revealing-the-top-10-hidden-story-supporters/) is what translates familiar domain names like howtogeek.com into the IP addresses computers use to connect with each other. When a program tries to connect to a domain name like google.com or facebook.com, your computer queries a DNS server on the internet to get the corresponding numerical IP address. To save time, Windows 10 stores a copy of the information it gets from DNS servers locally on your PC. This is called the DNS cache.

 Your PC's DNS cache can save time, but if something goes wrong with it, it can cause connection errors. The DNS cache can become corrupted, where the information relating IP addresses to domain names is lost due to a glitch. The cache can also become outdated, meaning that either the domain name or the IP address of the site you're trying to reach has changed since the cache was last updated. The DNS cache can also be poisoned, where it is [given incorrect information by DNS servers](https://vimeo-videos.techidaily.com/new-in-2024-premium-downloader-suite-for-vimeo-content/). DNS cache poisoning can be accidental, but it can also be used maliciously to steal login credentials or other sensitive data.

 The DNS cache affects all internet traffic on your PC, so if you're having trouble with only one program or a single website, the problem probably isn't your DNS cache. If you can't reach a specific website, you can use a tool like [IsItDownRightNow](https://www.isitdownrightnow.com/) to check the website's status. If a single application isn't able to connect to the internet, try [checking your firewall settings](https://screen-mirror.techidaily.com/in-2024-how-to-cast-apple-iphone-7-to-chromecast-drfone-by-drfone-ios/).

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=11224199&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/e09fdffe648a30658a9657bbed7b2388/products/copy_boxshot_lyricvideo.png" border="0">Lyric Video Creator Professional Version</a>
<!-- affiliate ads end -->
##  Flushing Your DNS Cache

 The DNS cache is not stored as a file on your PC, it is stored in system memory. System memory gets cleared every time your computer powers off, which is part of the reason [why restarting your computer fixes so many problems](https://android-pokemon-go.techidaily.com/in-2024-all-you-need-to-know-about-mega-greninja-for-motorola-moto-g13-drfone-by-drfone-virtual-android/). It also means the simplest way to flush your DNS cache is to restart your PC.

 If you want to manually flush your DNS cache on Windows 10, you can use Command Prompt or Windows PowerShell. Some commands must be "[Run as administrator](https://android-location.techidaily.com/in-2024-10-fake-gps-location-apps-on-android-of-your-samsung-galaxy-xcover-6-pro-tactical-edition-drfone-by-drfone-virtual/)," but it doesn't matter in this case.

 To launch Command Prompt, click the start button, type "cmd" or "command prompt" into the search bar on the Start menu, and then hit Enter.

![Running Command Prompt from the Start Menu.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/11/run-command-prompt.png) 

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4726807&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/c14a8df1e1b4d5297e9cb30cb34d5a00/products/copy_copy_power-tools-48.png" border="0">Power Tools add-on for Google Sheets, Lifetime subscription</a>
<!-- affiliate ads end -->
 Alternatively, you can use Windows PowerShell. Click the Start button, type "powershell" into the search bar in the Start menu, and hit Enter.

![Enter "PowerShell" in the Start Menu search.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/11/run-powershell.png) 

<!-- affiliate ads begin -->
<a href="https://shop.pcdj.com/order/checkout.php?PRODS=4698824&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/47f4b6321e9fd8e8f7326a6adc1a7c1e/products/dex3pro-screenshot-homepage.png" border="0">PCDJ DEX 3 for Windows & MAC is the total entertainment DJ software solution, offering audio, video, and karaoke mixing ability. Automatic beat-sync, smart looping, 4 decks, DJ MIDI controller support, Karaoke Streaming and much more. 
DEX 3 meets the demands of today’s versatile DJ, without compromise! 
DEX 3 (Audio, Video and Karaoke Mixing Software for Windows/MAC | 3 Activations and Free Updates)</a>
<!-- affiliate ads end -->
 With either Command Prompt or Windows PowerShell opened, enter the following command:

        `ipconfig /flushdns`
    
 If the DNS cache was flushed, you should see the "Successfully flushed the DNS Resolver Cache" message. You can now close the window.

 If you're using PowerShell 5 (which is still default on Windows 10) your Window will be blue instead of black. 

![The DNS Cache has been flushed successfully in PowerShell.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/11/flush-dns-powershell.png) 

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4600114&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.epubor.com/images/drm-removal-feature2.png" border="0">Any DRM Removal for Mac： Remove DRM from Adobe, Kindle, Sony eReader, Kobo, etc, read your ebooks anywhere.</a>
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
<li><a href="https://some-techniques.techidaily.com/new-excellent-pictorial-archive-networks/"><u>[New] Excellent Pictorial Archive Networks</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-exemplary-episodes-for-auditory-drama/"><u>[New] Exemplary Episodes for Auditory Drama</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-exploring-the-gopro-hero5-sessions/"><u>[New] Exploring the GoPro Hero5 Sessions</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-fine-tuning-the-art-of-recording-in-audacity/"><u>[New] Fine-Tuning the Art of Recording in Audacity</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-fly-high-with-gopro-karma-an-insiders-review/"><u>[New] Fly High with GoPro Karma  An Insider's Review</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-from-streaming-to-savings-preserving-your-internet-tunes/"><u>[New] From Streaming to Savings  Preserving Your Internet Tunes</u></a></li>
<li><a href="https://facebook-video-recording.techidaily.com/new-in-2024-digital-delights-8-most-watched-movies/"><u>[New] In 2024, Digital Delights  8 Most Watched Movies</u></a></li>
<li><a href="https://eaxpv-info.techidaily.com/new-in-2024-how-to-loop-a-video-on-iphone/"><u>[New] In 2024, How to Loop A Video on iPhone?</u></a></li>
<li><a href="https://facebook-videos.techidaily.com/updated-2024-approved-3-copywriting-structure-for-facebook-ads/"><u>[Updated] 2024 Approved  3 Copywriting Structure for Facebook Ads</u></a></li>
<li><a href="https://youtube-web.techidaily.com/ed-2024-approved-mastering-common-issues-in-youtube-shorts/"><u>[Updated] 2024 Approved  Mastering Common Issues in YouTube Shorts</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-evaluating-live-stream-giants-twitch-and-youtube/"><u>[Updated] Evaluating Live Stream Giants  Twitch & YouTube</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-evaluating-video-performance-vlc-versus-mx/"><u>[Updated] Evaluating Video Performance  VLC Versus MX</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-exploring-peak-performance-best-oculus-rift-players/"><u>[Updated] Exploring Peak Performance  Best Oculus Rift Players</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/updated-googles-advanced-upload-techniques-for-podcasters/"><u>[Updated] Google's Advanced Upload Techniques for Podcasters</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-gopros-top-tier-face-off-hero5-b-and-sessions/"><u>[Updated] GoPro's Top Tier Face-Off  Hero5 B & Sessions</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-harness-ai-to-generate-prime-video-titles/"><u>[Updated] Harness AI to Generate Prime Video Titles</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-how-to-create-time-lapse-video-with-canon-camera/"><u>[Updated] How to Create Time-Lapse Video with Canon Camera</u></a></li>
<li><a href="https://instagram-video-files.techidaily.com/updated-in-2024-the-quintessential-guide-to-secret-story-viewing/"><u>[Updated] In 2024, The Quintessential Guide to Secret Story Viewing</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-innovative-approach-to-hdr-portraiture-excellence/"><u>[Updated] Innovative Approach to HDR Portraiture Excellence</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-innovative-prime-lenses-for-professionals-shooting-4k/"><u>[Updated] Innovative Prime Lenses for Professionals Shooting 4K</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-innovative-strategies-to-enhance-video-craftsmanship-on-windows-10/"><u>[Updated] Innovative Strategies to Enhance Video Craftsmanship on Windows 10</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/4-solution-to-get-rid-of-pokemon-fail-to-detect-location-on-nokia-c300-drfone-by-drfone-virtual-android/"><u>4 solution to get rid of pokemon fail to detect location On Nokia C300 | Dr.fone</u></a></li>
<li><a href="https://tech-revival.techidaily.com/ai-income-avenues-assessing-gpt-powered-job-prospects/"><u>AI Income Avenues: Assessing GPT-Powered Job Prospects</u></a></li>
<li><a href="https://data-safeguard.techidaily.com/cookiebot-driven-analytics-and-marketing-solutions/"><u>Cookiebot-Driven Analytics & Marketing Solutions</u></a></li>
<li><a href="https://common-error.techidaily.com/efficient-techniques-to-fix-corrupt-windows-os-files-in-the-latest-versions-10-and-11/"><u>Efficient Techniques to Fix Corrupt Windows OS Files in the Latest Versions (10 and 11)</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/failed-to-play-mov-movies-on-motorola-moto-g14-by-aiseesoft-video-converter-play-mov-on-android/"><u>Failed to play MOV movies on Motorola Moto G14</u></a></li>
<li><a href="https://some-techniques.techidaily.com/geniusedit-ai-precision-in-photo-mastery-for-2024/"><u>GeniusEdit AI  Precision in Photo Mastery for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/glimmering-glides-of-2022s-speed-skaters-for-2024/"><u>Glimmering Glides of 2022'S Speed Skaters for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/go-live-on-youtube-with-minimum-follower-criteria-met-for-2024/"><u>Go Live on Youtube with Minimum Follower Criteria Met for 2024</u></a></li>
<li><a href="https://android-transfer.techidaily.com/how-to-transfer-data-from-infinix-zero-30-5g-to-blackberry-drfone-by-drfone-transfer-from-android-transfer-from-android/"><u>How to Transfer Data from Infinix Zero 30 5G to BlackBerry | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-exclusive-access-download-your-own-tailored-tracks/"><u>In 2024, Exclusive Access  Download Your Own Tailored Tracks</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-exclusive-guide-365-days-of-no-cost-text-files/"><u>In 2024, Exclusive Guide  365 Days of No-Cost Text Files</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-frame-finesse-selecting-superior-video-cams-for-slow-motion/"><u>In 2024, Frame Finesse  Selecting Superior Video Cams for Slow Motion</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-free-and-open-top-7-laptop-dvd-player-software-options/"><u>In 2024, Free & Open  Top 7 Laptop DVD Player Software Options</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-free-3d-text-psd-goldmine-top-selections/"><u>In 2024, Free 3D Text PSD Goldmine - Top Selections</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-from-basic-to-advanced-your-guide-to-system-advancements/"><u>In 2024, From Basic to Advanced  Your Guide to System Advancements</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-grasping-the-full-potential-of-animoji-on-iphone-x/"><u>In 2024, Grasping the Full Potential of Animoji on iPhone X</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-high-quality-action-captured-by-the-ion-pro-3-camera/"><u>In 2024, High-Quality Action Captured by the ION Pro 3 Camera</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-honing-skills-for-hiring-best-filmmakers/"><u>In 2024, Honing Skills for Hiring Best Filmmakers</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-ice-skates-and-epochs-a-look-at-beijings-olympic-saga-2022/"><u>In 2024, Ice Skates & Epochs  A Look at Beijing's Olympic Saga, 2022</u></a></li>
<li><a href="https://some-techniques.techidaily.com/infusing-life-into-virtual-scenes-with-spark-ar-and-personalized-lookups-for-2024/"><u>Infusing Life Into Virtual Scenes with Spark AR and Personalized Lookups for 2024</u></a></li>
<li><a href="https://techidaily.com/use-device-manager-to-reinstall-your-drivers-in-windows-11107-by-drivereasy-guide/"><u>Use Device Manager to reinstall your drivers in Windows 11/10/7</u></a></li>
</ul></div>
