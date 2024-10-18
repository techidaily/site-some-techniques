---
title: "Expert Tips: How to Perform a DNS Flush on a Windows 10 Computer"
date: 2024-10-11T16:01:26.097Z
updated: 2024-10-17T19:27:01.636Z
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

<!-- affiliate ads begin -->
<a href="https://unicoeye.pxf.io/c/5597632/2134244/18498" target="_top" id="2134244">
  <img src="//a.impactradius-go.com/display-ad/18498-2134244" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://unicoeye.pxf.io/i/5597632/2134244/18498" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://appsumo.8odi.net/c/5597632/2137393/7443" target="_top" id="2137393">
  <img src="//a.impactradius-go.com/display-ad/7443-2137393" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2137393/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Flushing Your DNS Cache

 The DNS cache is not stored as a file on your PC, it is stored in system memory. System memory gets cleared every time your computer powers off, which is part of the reason [why restarting your computer fixes so many problems](https://android-pokemon-go.techidaily.com/in-2024-all-you-need-to-know-about-mega-greninja-for-motorola-moto-g13-drfone-by-drfone-virtual-android/). It also means the simplest way to flush your DNS cache is to restart your PC.

 If you want to manually flush your DNS cache on Windows 10, you can use Command Prompt or Windows PowerShell. Some commands must be "[Run as administrator](https://android-location.techidaily.com/in-2024-10-fake-gps-location-apps-on-android-of-your-samsung-galaxy-xcover-6-pro-tactical-edition-drfone-by-drfone-virtual/)," but it doesn't matter in this case.

 To launch Command Prompt, click the start button, type "cmd" or "command prompt" into the search bar on the Start menu, and then hit Enter.

![Running Command Prompt from the Start Menu.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/11/run-command-prompt.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2037474/7443" target="_top" id="2037474">
  <img src="//a.impactradius-go.com/display-ad/7443-2037474" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2037474/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Alternatively, you can use Windows PowerShell. Click the Start button, type "powershell" into the search bar in the Start menu, and hit Enter.

![Enter "PowerShell" in the Start Menu search.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/11/run-powershell.png) 

<!-- affiliate ads begin -->
<a href="https://aidotcom.pxf.io/c/5597632/2134501/19576" target="_top" id="2134501">
  <img src="//a.impactradius-go.com/display-ad/19576-2134501" border="0" alt="https://techidaily.com" width="640" height="90"/>
</a>
<img height="0" width="0" src="https://aidotcom.pxf.io/i/5597632/2134501/19576" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://some-techniques.techidaily.com/new-exploring-the-capabilities-of-yuneecs-typhoon-uav/"><u>[New] Exploring the Capabilities of Yuneec’s Typhoon UAV</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-incorporating-personal-flair-fonts-for-ae-projects/"><u>[New] Incorporating Personal Flair Fonts for AE Projects</u></a></li>
<li><a href="https://fox-links.techidaily.com/updated-2024-approved-loop-engineers-assembly/"><u>[Updated] 2024 Approved Loop Engineer's Assembly</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-facebook-video-freeze-up-solutions-for-secure-browser-users/"><u>2024 Approved Facebook Video Freeze-Up Solutions for Secure Browser Users</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-ignite-motivation-the-hottest-playlists-for-workouts/"><u>2024 Approved Ignite Motivation The Hottest Playlists for Workouts</u></a></li>
<li><a href="https://facebook-video-content.techidaily.com/2024-approved-instagrams-best-practices-for-video-posts/"><u>2024 Approved Instagram's Best Practices for Video Posts</u></a></li>
<li><a href="https://ios-unlock.techidaily.com/detailed-review-of-doctorsim-unlock-service-for-apple-iphone-12-by-drfone-ios/"><u>Detailed Review of doctorSIM Unlock Service For Apple iPhone 12</u></a></li>
<li><a href="https://some-techniques.techidaily.com/from-concept-to-reality-selecting-top-3d-animators-software-for-2024/"><u>From Concept to Reality Selecting Top 3D Animators' Software for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/generate-individual-meme-crafts-today-for-2024/"><u>Generate Individual Meme Crafts Today for 2024</u></a></li>
<li><a href="https://win-able.techidaily.com/how-to-fix-the-persistent-connection-failed-error-in-hitman-3/"><u>How to Fix the Persistent 'Connection Failed' Error in Hitman 3</u></a></li>
<li><a href="https://change-location.techidaily.com/how-to-use-life360-on-windows-pc-for-oppo-reno-10-proplus-5g-drfone-by-drfone-virtual-android/"><u>How to Use Life360 on Windows PC For Oppo Reno 10 Pro+ 5G? | Dr.fone</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/in-2024-examining-gopro-max-and-hero-11-pursuit-of-perfect-footage/"><u>In 2024, Examining GoPro Max & Hero 11 Pursuit of Perfect Footage</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-excellence-in-penmanship-8-screenplay-classics/"><u>In 2024, Excellence in Penmanship 8 Screenplay Classics</u></a></li>
<li><a href="https://unlock-android.techidaily.com/in-2024-how-to-remove-or-bypass-knox-enrollment-service-on-xiaomi-14-pro-by-drfone-android/"><u>In 2024, How To Remove or Bypass Knox Enrollment Service On Xiaomi 14 Pro</u></a></li>
<li><a href="https://fox-glue.techidaily.com/in-2024-pictureweaversierra-blending-apple-media-artfully/"><u>In 2024, PictureWeaverSierra Blending Apple Media Artfully</u></a></li>
</ul></div>

