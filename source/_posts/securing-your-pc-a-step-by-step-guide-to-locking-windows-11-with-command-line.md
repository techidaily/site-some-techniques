---
title: "Securing Your PC: A Step-by-Step Guide to Locking Windows 11 with Command Line"
date: 2024-09-05T05:27:33.254Z
updated: 2024-09-06T05:27:33.254Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://thmb.techidaily.com/07cfabd2fe9acb782e30cca8205dc0f557a2c3371dbf02532bc0633c00063d56.jpg
---

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1884021/19272" target="_top" id="1884021">
  <img src="//a.impactradius-go.com/display-ad/19272-1884021" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1884021/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Securing Your PC: A Step-by-Step Guide to Locking Windows 11 with Command Line

### Quick Links

* [Lock Your Windows 10 PC Using Command Prompt](https://vp-tips.techidaily.com/new-audiovisual-adaptability-in-free-fire-for-2024/)
* [Set the Lock Screen Timeout Setting Using Command Prompt](https://eaxpv-info.techidaily.com/new-finding-a-different-way-to-naming-your-channel-with-filmora-for-2024/)

<!-- affiliate ads begin -->
<a href="https://laganoo.pxf.io/c/5597632/1484909/16446" target="_top" id="1484909">
  <img src="//a.impactradius-go.com/display-ad/16446-1484909" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://laganoo.pxf.io/i/5597632/1484909/16446" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
### Key Takeaways

* To lock your Windows PC using Command Prompt, run "**Rundll32.exe user32.dll,LockWorkStation"** in the Command Prompt
* To set the lock screen timeout, run "**powercfg.exe /SETACVALUEINDEX SCHEME\_CURRENT SUB\_VIDEO VIDEOCONLOCK <time>"** in Command Prompt as Admin
* Activate the lock screen timeout setting by running "**powercfg.exe /SETACTIVE SCHEME\_CURRENT"** after you set the timeout.

 One of the first rules of cyber security is to always lock your PC before stepping away. While it may not be the quickest way to lock your Windows 10 PC, you can do it using the Command Prompt.

##  Lock Your Windows 10 PC Using Command Prompt

 First, [open the Command Prompt](https://android-frp.techidaily.com/in-2024-step-by-step-tutorial-how-to-bypass-oppo-a78-frp-by-drfone-android/) on your PC by opening the Start menu, typing “cmd” in the Windows Search bar, and then selecting “Command Prompt” from the search results.

![Click the Start button, search for 'cmd,' then open 'Command Prompt.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/1-launch-cmd.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1880944/19272" target="_top" id="1880944">
  <img src="//a.impactradius-go.com/display-ad/19272-1880944" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1880944/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 Command Prompt will now open. Here, run this command to lock your Windows 10 PC.

Rundll32.exe user32.dll,LockWorkStation

![Locking your PC with Command Prompt.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/2-lock-pc-command-prompt.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2137380/7443" target="_top" id="2137380">
  <img src="//a.impactradius-go.com/display-ad/7443-2137380" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2137380/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 Once executed, your PC will be locked. You'll have to sign back in with your PIN, password, or whatever sign-in method you usually use.

##  Set the Lock Screen Timeout Setting Using Command Prompt

 Once you’ve locked your PC, the lock screen will generally be displayed for a certain amount of time before it time outs. You can set the amount of time that needs to pass before timing out using the Command Prompt.

 To do this, you’ll need to [open Command Prompt as an admin](https://screen-mirror.techidaily.com/how-to-screen-mirroring-xiaomi-14-ultra-drfone-by-drfone-android/). Do so by typing “cmd” in the Windows Search bar and then right-clicking “Command Prompt” from the results. Next, select “Run As Administrator” from the menu that appears.

![Launching Command Prompt as admin.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/3-launch-cmd.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2037346/7443" target="_top" id="2037346">
  <img src="//a.impactradius-go.com/display-ad/7443-2037346" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2037346/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 With Command Prompt open, run this command.

powercfg.exe /SETACVALUEINDEX SCHEME_CURRENT SUB_VIDEO VIDEOCONLOCK <time>

 Replace `<time>` with your desired amount of time in seconds. That means if you want to time out the lock screen after two minutes, you’d enter this command:

powercfg.exe /SETACVALUEINDEX SCHEME_CURRENT SUB_VIDEO VIDEOCONLOCK 120

![Change the timeout to 120.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/4-changing-timeout-to-120.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2049383/7443" target="_top" id="2049383">
  <img src="//a.impactradius-go.com/display-ad/7443-2049383" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2049383/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 This command sets the lock screen timeout setting for your PC if it’s plugged in to a power source. To set the lock screen timeout setting for your PC if it’s running on battery, change`/SETACVALUEINDEX` to`/SETDCVALUEINDEX` and run the command as normal.

 Next, run this command:

powercfg.exe /SETACTIVE SCHEME_CURRENT

![Apply the setting to the currently active scheme.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/5-set-active.png) 

 Now your [lock screen](https://driver-download.techidaily.com/1722977751917-synaptics-drivers-download-and-update-for-windows-easily/) will timeout after the set amount of time. Give it a try!

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
<li><a href="https://youtube-stream.techidaily.com/new-spice-up-viewers-innovative-cooking-channel-naming-tips/"><u>[New] Spice Up Viewers  Innovative Cooking Channel Naming Tips</u></a></li>
<li><a href="https://some-techniques.techidaily.com/1724313515797-abbyy/"><u>「日本語対応インボーズ自動化 - ABBYYフレックスキャプチャで処理簡素化」</u></a></li>
<li><a href="https://fox-helps.techidaily.com/2024-approved-dialogue-dynamics-balancing-verisimilitude-and-style/"><u>2024 Approved  Dialogue Dynamics  Balancing Verisimilitude and Style</u></a></li>
<li><a href="https://youtube-help.techidaily.com/2024-approved-unseen-yet-seen-how-to-conceal-faces-and-objects-digitally/"><u>2024 Approved  Unseen Yet Seen  How to Conceal Faces and Objects Digitally</u></a></li>
<li><a href="https://some-techniques.techidaily.com/1724313546384-abbyy/"><u>税収管理革新：ABBYY、トッパン・フォームズが中野区及び京都電子計算との共同模型構築</u></a></li>
<li><a href="https://some-techniques.techidaily.com/abbyy-finereader-beim-deutschen-patent-und-markenamt-volltextsuche-fur-eine-effiziente-dokumentation/"><u>ABBYY FineReader Beim Deutschen Patent- Und Markenamt - Volltextsuche Für Eine Effiziente Dokumentation</u></a></li>
<li><a href="https://some-techniques.techidaily.com/abbyy-flexicapture-cloud-terms-and-conditions-us-based-api-services/"><u>ABBYY FlexiCapture Cloud Terms and Conditions - US-Based API Services</u></a></li>
<li><a href="https://some-techniques.techidaily.com/abbyy-mobile-ocr-software-revolutionizes-portable-loan-verification-fun-and-fast/"><u>ABBYY Mobile OCR Software Revolutionizes Portable Loan Verification - Fun and Fast</u></a></li>
<li><a href="https://some-techniques.techidaily.com/abbyy-study-reveals-key-factors-influencing-the-outcomes-of-smart-process-automation/"><u>ABBYY Study Reveals Key Factors Influencing the Outcomes of Smart Process Automation</u></a></li>
<li><a href="https://some-techniques.techidaily.com/abbyys-smart-intelligence-catalyzing-enterprise-digitization-and-streamlining-processes/"><u>ABBYY's Smart Intelligence: Catalyzing Enterprise Digitization and Streamlining Processes</u></a></li>
<li><a href="https://network-issues.techidaily.com/addressing-laptop-display-distortion-a-step-by-step-approach/"><u>Addressing Laptop Display Distortion: A Step-by-Step Approach</u></a></li>
<li><a href="https://some-techniques.techidaily.com/ancien-cadre-chez-hp-et-microsoft-robert-youngjohns-devient-le-nouveau-president-du-conseil-dadministration-dabbyy/"><u>Ancien Cadre Chez HP Et Microsoft, Robert Youngjohns Devient Le Nouveau Président Du Conseil D'Administration D'ABBYY</u></a></li>
<li><a href="https://some-techniques.techidaily.com/at-the-helm-of-client-satisfaction-meet-nina-walker-vp-of-customer-success-at-abbyy/"><u>At the Helm of Client Satisfaction - Meet Nina Walker, VP of Customer Success at ABBYY</u></a></li>
<li><a href="https://some-techniques.techidaily.com/cookiebot-empowering-websites-with-advanced-tracking-technology/"><u>Cookiebot: Empowering Websites with Advanced Tracking Technology</u></a></li>
<li><a href="https://some-techniques.techidaily.com/customized-interactions-with-cookiebot-technology-for-improved-conversions/"><u>Customized Interactions with Cookiebot Technology for Improved Conversions</u></a></li>
<li><a href="https://screen-capture.techidaily.com/essential-tips-for-screen-recording-on-lenovo-devices-for-2024/"><u>Essential Tips for Screen Recording on Lenovo Devices for 2024</u></a></li>
<li><a href="https://youtube-sure.techidaily.com/ring-the-depths-of-asmr-audio-magic/"><u>Exploring the Depths of ASMR Audio Magic</u></a></li>
<li><a href="https://some-techniques.techidaily.com/globale-partnerschaft-kodak-alaris-und-abbyy-treten-bei-der-weltweiten-verbraucherdatenerfassung-zusammen/"><u>Globale Partnerschaft: Kodak Alaris Und AbbyY Treten Bei Der Weltweiten Verbraucherdatenerfassung Zusammen</u></a></li>
<li><a href="https://some-techniques.techidaily.com/harness-advanced-traffic-analysis-with-our-cookiebot-technology-solutions/"><u>Harness Advanced Traffic Analysis with Our Cookiebot Technology Solutions</u></a></li>
<li><a href="https://some-techniques.techidaily.com/harnessing-cookiebots-power-optimize-your-site-for-superior-seo-results/"><u>Harnessing Cookiebot's Power: Optimize Your Site for Superior SEO Results</u></a></li>
<li><a href="https://extra-tips.techidaily.com/hero4-black-vs-hero4-silver/"><u>Hero4 Black Vs Hero4 Silver</u></a></li>
<li><a href="https://facebook-clips.techidaily.com/igniting-online-trends-crafting-viral-facebook-posts/"><u>Igniting Online Trends  Crafting Viral Facebook Posts</u></a></li>
<li><a href="https://apple-account.techidaily.com/in-2024-the-easy-way-to-remove-an-apple-id-from-your-macbook-for-your-apple-iphone-6-by-drfone-ios/"><u>In 2024, The Easy Way to Remove an Apple ID from Your MacBook For your Apple iPhone 6</u></a></li>
<li><a href="https://some-techniques.techidaily.com/leadership-spotlight-abbyy-hails-as-a-premier-contender-on-the-202e-idp-peak-matrix-endorsement-by-everest-group/"><u>Leadership Spotlight: ABBYY Hails as a Premier Contender on the 202E IDP PEAK Matrix - Endorsement by Everest Group</u></a></li>
<li><a href="https://some-techniques.techidaily.com/navigating-the-web-discovering-your-perfect-page/"><u>Navigating the Web - Discovering Your Perfect Page</u></a></li>
<li><a href="https://some-techniques.techidaily.com/optimize-conversions-with-cookiebot-technology-integrated-into-your-website/"><u>Optimize Conversions with Cookiebot Technology Integrated Into Your Website</u></a></li>
<li><a href="https://some-techniques.techidaily.com/optimize-website-performance-with-advanced-cookiebot-solutions/"><u>Optimize Website Performance with Advanced Cookiebot Solutions</u></a></li>
<li><a href="https://some-techniques.techidaily.com/optimized-web-analytics-and-conversion-through-innovative-cookiebot-solutions/"><u>Optimized Web Analytics and Conversion Through Innovative Cookiebot Solutions</u></a></li>
<li><a href="https://some-techniques.techidaily.com/optimized-with-automated-tracking-the-power-of-cookiebot-technology/"><u>Optimized with Automated Tracking: The Power of Cookiebot Technology</u></a></li>
<li><a href="https://some-techniques.techidaily.com/outperforming-the-finance-market-elevate-success-using-abbyy-strategies/"><u>Outperforming the Finance Market: Elevate Success Using ABBYY Strategies</u></a></li>
<li><a href="https://some-techniques.techidaily.com/personalized-navigation-with-cookiebot-technology/"><u>Personalized Navigation with Cookiebot Technology</u></a></li>
<li><a href="https://extra-tips.techidaily.com/revolutionary-wearable-camera-tech/"><u>Revolutionary Wearable Camera Tech</u></a></li>
<li><a href="https://some-techniques.techidaily.com/revolutionizing-corporate-strategy-the-impact-of-digital-intellect-through-abbyy-expertise/"><u>Revolutionizing Corporate Strategy: The Impact of Digital Intellect Through ABBYY Expertise</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/say-it-like-you-mean-it-androids-voicegpt-guide/"><u>Say It Like You Mean It: Android’s VoiceGPT Guide</u></a></li>
<li><a href="https://some-techniques.techidaily.com/smart-analytics-driven-by-cookiebot-technology/"><u>Smart Analytics Driven by Cookiebot Technology</u></a></li>
<li><a href="https://some-techniques.techidaily.com/transform-your-iphone-photos-into-searchable-pdfs-mastering-scan-ocr-and-file-conversion-in-finereader-app/"><u>Transform Your iPhone Photos Into Searchable PDFs: Mastering Scan, OCR, and File Conversion in FineReader App</u></a></li>
<li><a href="https://some-techniques.techidaily.com/unleashing-the-potential-of-smart-technology-turning-contract-analysis-into-strategic-business-advantages-with-abbyy/"><u>Unleashing the Potential of Smart Technology: Turning Contract Analysis Into Strategic Business Advantages with ABBYY</u></a></li>
<li><a href="https://some-techniques.techidaily.com/wie-deloitte-die-funktionalitat-ihres-ediscovery-suites-erweitert/"><u>Wie Deloitte Die Funktionalität Ihres eDiscovery Suites Erweitert</u></a></li>
</ul></div>
