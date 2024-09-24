---
title: "Securing Your PC: A Step-by-Step Guide to Locking Windows 11 with Command Line"
date: 2024-09-23T07:36:25.191Z
updated: 2024-09-23T17:35:29.292Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://thmb.techidaily.com/07cfabd2fe9acb782e30cca8205dc0f557a2c3371dbf02532bc0633c00063d56.jpg
---

## Securing Your PC: A Step-by-Step Guide to Locking Windows 11 with Command Line

### Quick Links

* [Lock Your Windows 10 PC Using Command Prompt](https://vp-tips.techidaily.com/new-audiovisual-adaptability-in-free-fire-for-2024/)
* [Set the Lock Screen Timeout Setting Using Command Prompt](https://eaxpv-info.techidaily.com/new-finding-a-different-way-to-naming-your-channel-with-filmora-for-2024/)

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1886015/19272" target="_top" id="1886015">
  <img src="//a.impactradius-go.com/display-ad/19272-1886015" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1886015/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

### Key Takeaways

* To lock your Windows PC using Command Prompt, run "**Rundll32.exe user32.dll,LockWorkStation"** in the Command Prompt
* To set the lock screen timeout, run "**powercfg.exe /SETACVALUEINDEX SCHEME\_CURRENT SUB\_VIDEO VIDEOCONLOCK <time>"** in Command Prompt as Admin
* Activate the lock screen timeout setting by running "**powercfg.exe /SETACTIVE SCHEME\_CURRENT"** after you set the timeout.

 One of the first rules of cyber security is to always lock your PC before stepping away. While it may not be the quickest way to lock your Windows 10 PC, you can do it using the Command Prompt.

##  Lock Your Windows 10 PC Using Command Prompt

 First, [open the Command Prompt](https://android-frp.techidaily.com/in-2024-step-by-step-tutorial-how-to-bypass-oppo-a78-frp-by-drfone-android/) on your PC by opening the Start menu, typing “cmd” in the Windows Search bar, and then selecting “Command Prompt” from the search results.

![Click the Start button, search for 'cmd,' then open 'Command Prompt.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/1-launch-cmd.png) 

 Command Prompt will now open. Here, run this command to lock your Windows 10 PC.

Rundll32.exe user32.dll,LockWorkStation

![Locking your PC with Command Prompt.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/2-lock-pc-command-prompt.png) 

 Once executed, your PC will be locked. You'll have to sign back in with your PIN, password, or whatever sign-in method you usually use.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1934138/19272" target="_top" id="1934138">
  <img src="//a.impactradius-go.com/display-ad/19272-1934138" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1934138/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Set the Lock Screen Timeout Setting Using Command Prompt

 Once you’ve locked your PC, the lock screen will generally be displayed for a certain amount of time before it time outs. You can set the amount of time that needs to pass before timing out using the Command Prompt.

 To do this, you’ll need to [open Command Prompt as an admin](https://screen-mirror.techidaily.com/how-to-screen-mirroring-xiaomi-14-ultra-drfone-by-drfone-android/). Do so by typing “cmd” in the Windows Search bar and then right-clicking “Command Prompt” from the results. Next, select “Run As Administrator” from the menu that appears.

![Launching Command Prompt as admin.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/3-launch-cmd.png) 

<!-- affiliate ads begin -->
<a href="https://bluettius.sjv.io/c/5597632/2139110/17108" target="_top" id="2139110">
  <img src="//a.impactradius-go.com/display-ad/17108-2139110" border="0" alt="https://techidaily.com" width="468" height="60"/>
</a>
<img height="0" width="0" src="https://bluettius.sjv.io/i/5597632/2139110/17108" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 With Command Prompt open, run this command.

powercfg.exe /SETACVALUEINDEX SCHEME_CURRENT SUB_VIDEO VIDEOCONLOCK <time>

 Replace `<time>` with your desired amount of time in seconds. That means if you want to time out the lock screen after two minutes, you’d enter this command:

powercfg.exe /SETACVALUEINDEX SCHEME_CURRENT SUB_VIDEO VIDEOCONLOCK 120

![Change the timeout to 120.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/4-changing-timeout-to-120.png) 

<!-- affiliate ads begin -->
<a href="https://laganoo.pxf.io/c/5597632/1528693/16446" target="_top" id="1528693">
  <img src="//a.impactradius-go.com/display-ad/16446-1528693" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://laganoo.pxf.io/i/5597632/1528693/16446" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://extra-approaches.techidaily.com/updated-nikons-bold-move-into-4k-with-the-innovative-j5-model/"><u>[Updated] Nikon's Bold Move Into 4K with The Innovative J5 Model</u></a></li>
<li><a href="https://tech-revival.techidaily.com/8-cutting-edge-replacements-for-the-gpt-mobile-experience/"><u>8 Cutting-Edge Replacements for the GPT Mobile Experience</u></a></li>
<li><a href="https://some-techniques.techidaily.com/conversione-gratuita-da-mp4-a-vob-online-con-moviemaker/"><u>Conversione Gratuita Da MP4 a VOB Online Con MovieMaker</u></a></li>
<li><a href="https://some-techniques.techidaily.com/conversione-gratuita-di-wma-in-m4r-su-internet-utilizzando-movavi-guida-alla-conversione-rapida-e-facile/"><u>Conversione Gratuita Di WMA in M4R Su Internet Utilizzando Movavi - Guida Alla Conversione Rapida E Facile</u></a></li>
<li><a href="https://some-techniques.techidaily.com/conversione-gratuita-online-da-mkv-a-ogg-con-movavi-guida-completa/"><u>Conversione Gratuita Online Da MKV a OGG Con Movavi - Guida Completa</u></a></li>
<li><a href="https://some-techniques.techidaily.com/convert-audio-file-from-aac-to-flac-for-free-on-the-web-with-fastvideoeditingcom/"><u>Convert Audio File From AAC to FLAC for Free on the Web with FastVideoEditing.com</u></a></li>
<li><a href="https://some-techniques.techidaily.com/convert-audio-files-seamlessly-mp3-to-mov-for-free-with-moveavi/"><u>Convert Audio Files Seamlessly - MP3 To Mov For FREE with MoveAVI</u></a></li>
<li><a href="https://some-techniques.techidaily.com/convertir-archivos-mov-a-m4a-sin-costo-alguno-conversion-en-linea-facil/"><u>Convertir Archivos MOV a M4A Sin Costo Alguno - Conversión en Línea Fácil</u></a></li>
<li><a href="https://some-techniques.techidaily.com/denkvangerig-conversie-van-dng-naar-tiff-onlinegestuurd-and-vrijgevreesgratis-movavi/"><u>Denkvangerig Conversie Van DNG Naar TIFF - Onlinegestuurd & Vrijgevreesgratis - Movavi</u></a></li>
<li><a href="https://some-techniques.techidaily.com/descubre-el-tratodo-sobre-la-conversion-de-archivos-video-wmv-usando-ram-en-linea-gratis-la-solucion-de-movavi/"><u>Descubre El Tratodo Sobre La Conversión De Archivos Vídeo WMV Usando RAM en Línea Gratis: La Solución De Movavi</u></a></li>
<li><a href="https://some-techniques.techidaily.com/dettagli-sui-file-wmv-e-come-sbloccarne-il-contenuto-sul-tuo-computer/"><u>Dettagli Sui File WMV E Come Sbloccarne Il Contenuto Sul Tuo Computer</u></a></li>
<li><a href="https://some-techniques.techidaily.com/discover-movavi-unlimited-all-features-of-the-movavi-program-in-one-package/"><u>Discover Movavi Unlimited – All Features of the Movavi Program in One Package!</u></a></li>
<li><a href="https://sound-issues.techidaily.com/effective-solutions-for-malfunctioning-speakers-on-your-windows-11-system/"><u>Effective Solutions for Malfunctioning Speakers on Your Windows 11 System</u></a></li>
<li><a href="https://games-able.techidaily.com/essential-upgrades-for-optimal-steam-deck-performance/"><u>Essential Upgrades for Optimal Steam Deck Performance</u></a></li>
<li><a href="https://driver-download.techidaily.com/how-to-update-your-windows-10-11-8-or-n-version-with-microsofts-most-recent-bluetooth-driver-software/"><u>How to Update Your Windows (10, 11, 8 or N-Version) With Microsoft's Most Recent Bluetooth Driver Software</u></a></li>
<li><a href="https://review-topics.techidaily.com/how-to-upgrade-iphone-xs-without-itunes-drfone-by-drfone-ios-system-repair-ios-system-repair/"><u>How to Upgrade iPhone XS without iTunes? | Dr.fone</u></a></li>
<li><a href="https://extra-hints.techidaily.com/in-2024-best-5k-monitors-you-can-get/"><u>In 2024, Best 5K Monitors You Can Get</u></a></li>
<li><a href="https://windows11.techidaily.com/mastering-windows-11-settings-for-effortless-administration/"><u>Mastering Windows 11 Settings for Effortless Administration</u></a></li>
<li><a href="https://extra-tips.techidaily.com/quantum-hdr-unveiled-industry-insights/"><u>Quantum HDR Unveiled Industry Insights</u></a></li>
<li><a href="https://win-dash.techidaily.com/toughness-is-the-energy-absorption-capacity-of-a-material-up-to-fracture-combining-strength-and-ductility/"><u>Toughness Is the Energy Absorption Capacity of a Material up to Fracture, Combining Strength and Ductility.</u></a></li>
</ul></div>

