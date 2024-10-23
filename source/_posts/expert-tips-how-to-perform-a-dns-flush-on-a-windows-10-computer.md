---
title: "Expert Tips: How to Perform a DNS Flush on a Windows 10 Computer"
date: 2024-10-19T17:20:04.464Z
updated: 2024-10-23T20:43:58.053Z
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
<a href="https://appsumo.8odi.net/c/5597632/2068411/7443" target="_top" id="2068411">
  <img src="//a.impactradius-go.com/display-ad/7443-2068411" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2068411/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  What Does the DNS Cache Do? 

 A [Domain Network System (DNS) server](https://instagram-clips.techidaily.com/new-2024-approved-revealing-the-top-10-hidden-story-supporters/) is what translates familiar domain names like howtogeek.com into the IP addresses computers use to connect with each other. When a program tries to connect to a domain name like google.com or facebook.com, your computer queries a DNS server on the internet to get the corresponding numerical IP address. To save time, Windows 10 stores a copy of the information it gets from DNS servers locally on your PC. This is called the DNS cache.

 Your PC's DNS cache can save time, but if something goes wrong with it, it can cause connection errors. The DNS cache can become corrupted, where the information relating IP addresses to domain names is lost due to a glitch. The cache can also become outdated, meaning that either the domain name or the IP address of the site you're trying to reach has changed since the cache was last updated. The DNS cache can also be poisoned, where it is [given incorrect information by DNS servers](https://vimeo-videos.techidaily.com/new-in-2024-premium-downloader-suite-for-vimeo-content/). DNS cache poisoning can be accidental, but it can also be used maliciously to steal login credentials or other sensitive data.

 The DNS cache affects all internet traffic on your PC, so if you're having trouble with only one program or a single website, the problem probably isn't your DNS cache. If you can't reach a specific website, you can use a tool like [IsItDownRightNow](https://www.isitdownrightnow.com/) to check the website's status. If a single application isn't able to connect to the internet, try [checking your firewall settings](https://screen-mirror.techidaily.com/in-2024-how-to-cast-apple-iphone-7-to-chromecast-drfone-by-drfone-ios/).

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1885928/19272" target="_top" id="1885928">
  <img src="//a.impactradius-go.com/display-ad/19272-1885928" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1885928/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Flushing Your DNS Cache

 The DNS cache is not stored as a file on your PC, it is stored in system memory. System memory gets cleared every time your computer powers off, which is part of the reason [why restarting your computer fixes so many problems](https://android-pokemon-go.techidaily.com/in-2024-all-you-need-to-know-about-mega-greninja-for-motorola-moto-g13-drfone-by-drfone-virtual-android/). It also means the simplest way to flush your DNS cache is to restart your PC.

 If you want to manually flush your DNS cache on Windows 10, you can use Command Prompt or Windows PowerShell. Some commands must be "[Run as administrator](https://android-location.techidaily.com/in-2024-10-fake-gps-location-apps-on-android-of-your-samsung-galaxy-xcover-6-pro-tactical-edition-drfone-by-drfone-virtual/)," but it doesn't matter in this case.

 To launch Command Prompt, click the start button, type "cmd" or "command prompt" into the search bar on the Start menu, and then hit Enter.

![Running Command Prompt from the Start Menu.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/11/run-command-prompt.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2105869/7443" target="_top" id="2105869">
  <img src="//a.impactradius-go.com/display-ad/7443-2105869" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2105869/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Alternatively, you can use Windows PowerShell. Click the Start button, type "powershell" into the search bar in the Start menu, and hit Enter.

![Enter "PowerShell" in the Start Menu search.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/11/run-powershell.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2111968/7443" target="_top" id="2111968">
  <img src="//a.impactradius-go.com/display-ad/7443-2111968" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2111968/7443" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://extra-tips.techidaily.com/new-chucklecanvas-jokesinframes/"><u>[New] ChuckleCanvas JokesInFrames</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-funimate-playbook-strategies-for-success/"><u>[New] Funimate Playbook Strategies for Success</u></a></li>
<li><a href="https://facebook-clips.techidaily.com/new-transforming-hidden-content-fb-video-strategies/"><u>[New] Transforming Hidden Content FB Video Strategies</u></a></li>
<li><a href="https://fox-hovers.techidaily.com/updated-a-step-by-step-framework-for-dimming-sounds-in-lumafusion/"><u>[Updated] A Step-by-Step Framework for Dimming Sounds in Lumafusion</u></a></li>
<li><a href="https://youtube-web.techidaily.com/ed-comparing-streams-vimeo-versus-youtube-for-2024/"><u>[Updated] Comparing Streams Vimeo Versus YouTube for 2024</u></a></li>
<li><a href="https://video-capture.techidaily.com/updated-in-2024-obs-studio-showdown-with-bandicam-the-ultimate-test/"><u>[Updated] In 2024, OBS Studio Showdown with Bandicam The Ultimate Test</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-excellence-on-screen-the-top-15-in-stop-motion-cinema/"><u>2024 Approved Excellence on Screen The Top 15 in Stop Motion Cinema</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-industrys-airborenas-titans-10-lifters-reviewed/"><u>2024 Approved Industry's Airborenas Titans 10 Lifters Reviewed</u></a></li>
<li><a href="https://facebook.techidaily.com/deciphering-hidden-identities-on-digital-communication-platforms/"><u>Deciphering Hidden Identities on Digital Communication Platforms</u></a></li>
<li><a href="https://some-techniques.techidaily.com/harnessing-techniques-for-superior-pics-free-of-charge-for-2024/"><u>Harnessing Techniques for Superior Pics, Free of Charge for 2024</u></a></li>
<li><a href="https://blog-min.techidaily.com/how-to-fix-excel-2023-run-time-error-1004-by-stellar-guide/"><u>How to Fix Excel 2023 Run Time Error 1004</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-from-overflowed-drafters-to-ordered-files-learn-to-edit-hefty-tiktok-content/"><u>In 2024, From Overflowed Drafters to Ordered Files Learn to Edit Hefty TikTok Content</u></a></li>
</ul></div>

