---
title: "Expert Tips: How to Perform a DNS Flush on a Windows 10 Computer"
date: 2024-12-12T01:16:23.046Z
updated: 2024-12-16T00:51:54.352Z
tags:
  - deals
categories:
  - tech
thumbnail: https://thmb.techidaily.com/af6a241ce73781e980e91fb32b5f340b0c43ca449b76945212041b79725c225d.jpg
---

## Expert Tips: How to Perform a DNS Flush on a Windows 10 Computer

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/pGHmqD53gc8?si=ymgHIB6Aa7_MoUUf" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/6kzbT13ds3M?si=hBInu0Or-cX2ANJF" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  What Does the DNS Cache Do? 

 A [Domain Network System (DNS) server](https://instagram-clips.techidaily.com/new-2024-approved-revealing-the-top-10-hidden-story-supporters/) is what translates familiar domain names like howtogeek.com into the IP addresses computers use to connect with each other. When a program tries to connect to a domain name like google.com or facebook.com, your computer queries a DNS server on the internet to get the corresponding numerical IP address. To save time, Windows 10 stores a copy of the information it gets from DNS servers locally on your PC. This is called the DNS cache.

 Your PC's DNS cache can save time, but if something goes wrong with it, it can cause connection errors. The DNS cache can become corrupted, where the information relating IP addresses to domain names is lost due to a glitch. The cache can also become outdated, meaning that either the domain name or the IP address of the site you're trying to reach has changed since the cache was last updated. The DNS cache can also be poisoned, where it is [given incorrect information by DNS servers](https://vimeo-videos.techidaily.com/new-in-2024-premium-downloader-suite-for-vimeo-content/). DNS cache poisoning can be accidental, but it can also be used maliciously to steal login credentials or other sensitive data.

 The DNS cache affects all internet traffic on your PC, so if you're having trouble with only one program or a single website, the problem probably isn't your DNS cache. If you can't reach a specific website, you can use a tool like [IsItDownRightNow](https://www.isitdownrightnow.com/) to check the website's status. If a single application isn't able to connect to the internet, try [checking your firewall settings](https://screen-mirror.techidaily.com/in-2024-how-to-cast-apple-iphone-7-to-chromecast-drfone-by-drfone-ios/).

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/2NU63YqpVqw?si=uoJs0-nZYAkILqXx" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Flushing Your DNS Cache

 The DNS cache is not stored as a file on your PC, it is stored in system memory. System memory gets cleared every time your computer powers off, which is part of the reason [why restarting your computer fixes so many problems](https://android-pokemon-go.techidaily.com/in-2024-all-you-need-to-know-about-mega-greninja-for-motorola-moto-g13-drfone-by-drfone-virtual-android/). It also means the simplest way to flush your DNS cache is to restart your PC.

 If you want to manually flush your DNS cache on Windows 10, you can use Command Prompt or Windows PowerShell. Some commands must be "[Run as administrator](https://android-location.techidaily.com/in-2024-10-fake-gps-location-apps-on-android-of-your-samsung-galaxy-xcover-6-pro-tactical-edition-drfone-by-drfone-virtual/)," but it doesn't matter in this case.

 To launch Command Prompt, click the start button, type "cmd" or "command prompt" into the search bar on the Start menu, and then hit Enter.

![Running Command Prompt from the Start Menu.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/11/run-command-prompt.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/RJNYTGHVlLc?si=heERQcpMi77lqToE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Alternatively, you can use Windows PowerShell. Click the Start button, type "powershell" into the search bar in the Start menu, and hit Enter.

![Enter "PowerShell" in the Start Menu search.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/11/run-powershell.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/vPGg53vbOsk?si=CkSEN5HFPS7vDuAa" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://some-techniques.techidaily.com/new-expert-advice-on-acquiring-royalty-free-high-quality-graphics/"><u>[New] Expert Advice on Acquiring Royalty-Free, High-Quality Graphics</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-fresh-selection-of-engagement-prompts-for-audio-audiences/"><u>[New] Fresh Selection of Engagement Prompts for Audio Audiences</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-expert-techniques-for-stellar-titling/"><u>[Updated] Expert Techniques for Stellar Titling</u></a></li>
<li><a href="https://extra-hints.techidaily.com/updated-top-10-professional-360-degree-cameras/"><u>[Updated] Top 10 Professional 360 Degree Cameras</u></a></li>
<li><a href="https://fox-helps.techidaily.com/updated-unraveling-the-itunes-radio-download-process/"><u>[Updated] Unraveling the iTunes Radio Download Process</u></a></li>
<li><a href="https://fox-blue.techidaily.com/2024-approved-prime-picks-7-superior-apple-video-viewers/"><u>2024 Approved Prime Picks 7 Superior Apple Video Viewers</u></a></li>
<li><a href="https://extra-tips.techidaily.com/capture-memories-safely-explore-all-inclusive-free-and-charged-cloud-storage-solutions-for-2024/"><u>Capture Memories Safely Explore All-Inclusive Free and Charged Cloud Storage Solutions for 2024</u></a></li>
<li><a href="https://tech-renaissance.techidaily.com/charge-and-chill-with-the-ultimate-magsafe-multi-device-dock-for-apple-gadgets-zdnets-top-picks/"><u>Charge and Chill with the Ultimate MagSafe Multi-Device Dock for Apple Gadgets - ZDNet's Top Picks!</u></a></li>
<li><a href="https://win-able.techidaily.com/fixing-apex-legends-game-engine-troubles-solutions-included/"><u>Fixing Apex Legends Game Engine Troubles - Solutions Included</u></a></li>
<li><a href="https://vimeo-videos.techidaily.com/in-2024-boosting-your-videos-chance-on-vimeo-staff-list/"><u>In 2024, Boosting Your Video's Chance on Vimeo Staff List</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-exceptional-aspects-of-inexpensive-asmr-microphones/"><u>In 2024, Exceptional Aspects of Inexpensive ASMR Microphones</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-formula-field-report-game-reviews/"><u>In 2024, FORMULA FIELD REPORT Game Reviews</u></a></li>
<li><a href="https://fix-guide.techidaily.com/in-2024-how-to-pause-life360-location-sharing-for-xiaomi-civi-3-drfone-by-drfone-virtual-android/"><u>In 2024, How To Pause Life360 Location Sharing For Xiaomi Civi 3 | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-how-to-run-a-giveaway-facebook-post/"><u>In 2024, How to Run a Giveaway Facebook Post</u></a></li>
<li><a href="https://youtube-web.techidaily.com/ating-with-youtube-studio-editor-for-next-gen-videos/"><u>Innovating with YouTube Studio Editor for Next-Gen Videos</u></a></li>
</ul></div>

