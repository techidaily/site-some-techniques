---
title: "Expert Tips: How to Perform a DNS Flush on a Windows 10 Computer"
date: 2025-01-19T20:21:23.716Z
updated: 2025-01-21T17:38:03.889Z
tags:
  - deals
categories:
  - tech
thumbnail: https://thmb.techidaily.com/af6a241ce73781e980e91fb32b5f340b0c43ca449b76945212041b79725c225d.jpg
---

## Expert Tips: How to Perform a DNS Flush on a Windows 10 Computer

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/Nl0Z0eth1u4?si=0eecOBNfc--51AJO" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

### Quick Links

* [What Does the DNS Cache Do?](https://screen-video-capture.techidaily.com/new-2024-approved-simplified-game-recording-setups-for-stardew-villagers/)
* [Flushing Your DNS Cache](https://facebook-video-share.techidaily.com/updated-swipe-right-on-creativity-youtubes-top-techniques-for-greenscreens/)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/BR4gsW-J7as?si=9a56UDKZKhREZnwz" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/XIUatTFH0Zw?si=ZCtoBtIy18y2F5Vc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Flushing Your DNS Cache

 The DNS cache is not stored as a file on your PC, it is stored in system memory. System memory gets cleared every time your computer powers off, which is part of the reason [why restarting your computer fixes so many problems](https://android-pokemon-go.techidaily.com/in-2024-all-you-need-to-know-about-mega-greninja-for-motorola-moto-g13-drfone-by-drfone-virtual-android/). It also means the simplest way to flush your DNS cache is to restart your PC.

 If you want to manually flush your DNS cache on Windows 10, you can use Command Prompt or Windows PowerShell. Some commands must be "[Run as administrator](https://android-location.techidaily.com/in-2024-10-fake-gps-location-apps-on-android-of-your-samsung-galaxy-xcover-6-pro-tactical-edition-drfone-by-drfone-virtual/)," but it doesn't matter in this case.

 To launch Command Prompt, click the start button, type "cmd" or "command prompt" into the search bar on the Start menu, and then hit Enter.

![Running Command Prompt from the Start Menu.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/11/run-command-prompt.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/S3Th6oa_isA?si=TTQ013BB9beUM4x6" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Alternatively, you can use Windows PowerShell. Click the Start button, type "powershell" into the search bar in the Start menu, and hit Enter.

![Enter "PowerShell" in the Start Menu search.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/11/run-powershell.png) 

 With either Command Prompt or Windows PowerShell opened, enter the following command:

        `ipconfig /flushdns`
    
 If the DNS cache was flushed, you should see the "Successfully flushed the DNS Resolver Cache" message. You can now close the window.

 If you're using PowerShell 5 (which is still default on Windows 10) your Window will be blue instead of black. 

![The DNS Cache has been flushed successfully in PowerShell.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/11/flush-dns-powershell.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/kZVDkvMZvP4?si=xAugrCf-Ud6EMMpm" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://fox-cloud.techidaily.com/new-2024-approved-navigating-the-complex-world-of-lipos-for-drones/"><u>[New] 2024 Approved Navigating the Complex World of LiPos for Drones</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-excellence-in-capturing-slow-motions/"><u>[New] Excellence in Capturing Slow Motions</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-expert-tips-for-3d-text-designing-in-ai/"><u>[New] Expert Tips for 3D Text Designing in AI</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-harnessing-the-power-of-fisheye-photography/"><u>[New] Harnessing the Power of Fisheye Photography</u></a></li>
<li><a href="https://facebook-clips.techidaily.com/updated-discreet-peek-into-fb-narratives/"><u>[Updated] Discreet Peek Into FB Narratives</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-how-to-craft-and-modify-iphone-motion-videos-reducing-pace-effectively/"><u>[Updated] How to Craft & Modify iPhone Motion Videos Reducing Pace Effectively</u></a></li>
<li><a href="https://youtube-tips.techidaily.com/ed-optimize-your-video-written-by-your-name/"><u>[Updated] Optimize Your Video' Written By [Your Name]</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-happy-enrollment-and-logout-flowchart/"><u>2024 Approved Happy Enrollment & Logout Flowchart</u></a></li>
<li><a href="https://blog-min.techidaily.com/5-ways-to-move-contacts-from-infinix-zero-30-5g-to-iphone-131415-drfone-by-drfone-transfer-from-android-transfer-from-android/"><u>5 Ways to Move Contacts From Infinix Zero 30 5G to iPhone (13/14/15) | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/expertise-in-image-colors-pro-techniques-revealed-for-2024/"><u>Expertise in Image Colors Pro Techniques Revealed for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/full-analysis-of-t5-eyes-exceptional-action-recording-for-2024/"><u>Full Analysis of T5 Eye's Exceptional Action Recording for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/how-to-evade-tips-on-avoiding-edgenuity-video-lessons-with-finesse-for-2024/"><u>How to Evade Tips on Avoiding Edgenuity Video Lessons with Finesse for 2024</u></a></li>
<li><a href="https://apple-account.techidaily.com/how-to-fix-locked-apple-id-on-iphone-12-pro-by-drfone-ios/"><u>How to Fix Locked Apple ID on iPhone 12 Pro</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-exploring-the-marvel-of-apples-m1-max-attachments/"><u>In 2024, Exploring the Marvel of Apple’s M1 Max Attachments</u></a></li>
<li><a href="https://fox-boxes.techidaily.com/inside-the-top-10-virtual-reality-smartphone-gaming/"><u>Inside the Top 10 Virtual Reality Smartphone Gaming</u></a></li>
<li><a href="https://win-alternatives.techidaily.com/1728499976810-jvc-everio/"><u>JVC Everioビデオ機器から消失した動画を取り戻す簡単方法 – 完全復元のキーポイント</u></a></li>
<li><a href="https://facebook.techidaily.com/podcast-and-live-room-spotlight-on-facebooks-latest-hub/"><u>Podcast & Live Room Spotlight on Facebook's Latest Hub</u></a></li>
<li><a href="https://solve-popular.techidaily.com/step-by-step-guide-to-upgrading-windows-nstallation-from-hdd-to-ssd-with-drive-cloning/"><u>Step-by-Step Guide to Upgrading Windows Nstallation From HDD to SSD with Drive Cloning</u></a></li>
<li><a href="https://youtube-sure.techidaily.com/er-the-globes-secrets-with-these-youtubers/"><u>Uncover the Globe's Secrets with These Youtubers</u></a></li>
</ul></div>

