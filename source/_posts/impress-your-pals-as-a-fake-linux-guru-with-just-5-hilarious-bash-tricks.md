---
title: Impress Your Pals as a Fake Linux Guru with Just 5 Hilarious Bash Tricks
date: 2024-10-16T21:17:30.372Z
updated: 2024-10-23T17:11:24.849Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/ubuntu.jpg
---

## Impress Your Pals as a Fake Linux Guru with Just 5 Hilarious Bash Tricks

While I am a Linux daily driver, and I do sprinkle the terminal with commands now and then, I'm by no means a hacker. That didn't stop me from looking the part, though, since it turns out several simple commands (and a whole app) exist to make you look like a star in a florid cyberthriller. Here they are and how to run them.

## 1  neofetch 

![neofetch command output on an Ubuntu operating system.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/2024-02-14_16h38_17.png) 

 Starting simple, neofetch is perfect for when you want to send your friends a screenshot of your sweet new Linux desktop with a terminal open to make it look like you know how to use it. You simply run the command and some stats about your system will be printed next to a big [ASCII art](https://en.wikipedia.org/wiki/ASCII%5Fart) version of your distro's logo. If you've ever checked out r/UnixPorn, you'll recognize it as one of the more popular outputs to have printed in an open terminal.

 You can install neofetch on Debian and Ubuntu-based systems with this command

sudo apt install neofetch

 On Fedora Linux, you want this command:

sudo dnf install neofetch

 If you "use Arch btw" and have Pacman installed, you can instead run this command:

sudo pacman -S neofetch

 Then simply enter the command **neofetch** in your terminal to see your unique printout. Remember that the colors used will depend on your terminal settings. If the defaults don't look good, learn [how to customize your Bash prompt](https://screen-mirror.techidaily.com/3-facts-you-need-to-know-about-screen-mirroring-honor-90-gt-drfone-by-drfone-android/).

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2037338/7443" target="_top" id="2037338">
  <img src="//a.impactradius-go.com/display-ad/7443-2037338" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2037338/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

## 2  cmatrix 

Your browser does not support the video tag. 

 I know you were waiting for it: the classic Matrix-style text waterfall animation in your terminal. Put this on with a simple command and you'll become Neo, or so your friends will think. It's also the perfect "screensaver" for a terminal you maybe keep open in another monitor for when you need it.

 You can install cmatrix with this command.

sudo apt install cmatrix

 Or, on Red Hat distributions, run this command:

sudo dnf install cmatrix

 On Arch-based systems, use pacman to install it:

sudo pacman -S cmatrix

 You run the basic version with this command:

cmatrix

 You've got several flags (short bits of text you add onto the command) that will let you customize the look or function, like -r to get rainbow colors or -s to make it act like a screensaver where any keystroke closes the program. Use the **cmatrix -h** command to see them all.

<!-- affiliate ads begin -->
<a href="https://ephamedtechinc.pxf.io/c/5597632/2139322/26400" target="_top" id="2139322">
  <img src="//a.impactradius-go.com/display-ad/26400-2139322" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://ephamedtechinc.pxf.io/i/5597632/2139322/26400" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

## 3  genact 

Your browser does not support the video tag. 

 I was caught off-guard the first time I used the genact command because it seemed to be installing additional assets before running, which I thought was ridiculous for a simple text animation. The joke was on me, though, because that's just what genact does: it creates the impression it's downloading files, [crypto mining](https://vimeo-videos.techidaily.com/updated-in-2024-mastering-video-allure-securing-top-spots-with-the-vimeo-experts/), and running other random tasks when in fact nothing is happening. It has several unique modes that it cycles through at random, so you can open multiple terminal windows and run genact in each to look like you're multitasking like a pro.

 The easiest way to install it is through the Snap store, with this command:

snap install genact

 If you're not a Snap user, you can also download genact directly from [the GitHub release page](https://github.com/svenstaro/genact/releases). There are several versions, so you have to choose [your architecture](https://fox-friendly.techidaily.com/in-2024-top-professional-camera-choices-complete-360-guide-2023/) and operating system. If you're not sure, your safest bet is the one ending in "x86\_64-unknown-linux-gnu". Open a terminal, navigate to the directory genact is stored, then run **chmod +x genact-1.4.2-x86\_64-unknown-linux-gnu** (adjusting for your file name) to give the file permission to execute. Run it by typing ./ (a period and forward slash) followed by genact's file name. So for me that command looked like:

./genact-1.4.2-x86_64-unknown-linux-gnu

 If none of that setup appeals to you, you'll be happy to learn you don't need a terminal (or even a Linux distribution); you can simply [open genact in your browser](https://svenstaro.github.io/genact/). Fullscreen your browser with the F11 key for full effect.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1918698/19272" target="_top" id="1918698">
  <img src="//a.impactradius-go.com/display-ad/19272-1918698" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1918698/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

## 4  hollywood 

Your browser does not support the video tag. 

 Increasing in complexity is hollywood, which generates multiple panes in your terminal that show everything from hashes to speed tests to a global map in ASCII. It's _big_, so you'll want to maximize your terminal window. It's colorful, too, and resets frequently, perfect for an eye-catching and, well, cinematic display. Its name comes from the fact it's meant to be visible "in the background of any excellent schlock technothriller," to quote the creator.

 On Debian systems, use this command to install it:

sudo apt install hollywood

 If you're a Fedora or Red Hat user, you'll want this command:

dnf install hollywood

 For Arch users, you can get it with a Pacman command:

sudo pacman -S hollywood

 Once it's installed, going hacker mode is as simple as typing **hollywood** into your terminal and hitting Enter.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1883998/19272" target="_top" id="1883998">
  <img src="//a.impactradius-go.com/display-ad/19272-1883998" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1883998/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

## 5  eDEX-UI 

Your browser does not support the video tag. 

 eDEX-UI doesn't actually run in your terminal, it is _itself_ a terminal emulator, which means you can run actual commands inside it, including any of the ones I've already shown you. Designed to fit perfectly in a movie about hacking or espionage, eDEX-UI also produces those beeping and whirring sounds that computers in movies do (and that we all know would be very annoying in real life). It even supports touchscreens, so you can type on that virtual keyboard with a tablet or touch monitor!

 There is some bad news: eDEX-UI is no longer maintained as a project at the time of writing. The good news is the original repository is still available and works, at least in my testing. So just go to [the eDEX-UI release page](https://github.com/GitSquared/edex-ui/releases), download the version for you (likely "eDEX-UI-Linux-x86\_64.AppImage" and run it. Don't forget that since it's [an AppImage](https://facebook-video-recording.techidaily.com/updated-in-2024-expert-picks-top-6-fb-lite-extractors/) you'll need to give it permission to execute. Right-click it and open the Properties window, then look for an executable setting. In my file browser, Dolphin, it's a checkbox in the Permissions tab labeled "Is Executable." Voila, you're hacking the planet.

---

 If you're ready to go beyond just _looking_ like a hacker, you can do a lot of cool and actually useful things in the Linux terminal. After learning [some basic commands](https://win11-tips.techidaily.com/precision-adjusting-windows-locksleep-timer/), you can start automating your daily tasks scripts, and getting started is easy with some [beginner script examples](https://common-error.techidaily.com/rebooting-woes-windows-10-troubleshooting/). You can even [use Spotify in your terminal](https://phone-solutions.techidaily.com/all-about-factory-reset-what-is-it-and-what-it-does-to-your-samsung-galaxy-s23plus-drfone-by-drfone-reset-android-reset-android/)

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
<li><a href="https://facebook-record-videos.techidaily.com/new-2024-approved-essential-free-resources-for-youtube-intros/"><u>[New] 2024 Approved Essential Free Resources for YouTube Intros</u></a></li>
<li><a href="https://facebook-video-share.techidaily.com/new-in-2024-breaking-into-the-world-of-youtube-stellar-intros-in-imovie/"><u>[New] In 2024, Breaking Into the World of YouTube Stellar Intros in iMovie</u></a></li>
<li><a href="https://youtube-tips.techidaily.com/ed-2024-approved-unleashing-brand-potential-with-free-youtube-marketing-templates/"><u>[Updated] 2024 Approved Unleashing Brand Potential with FREE YouTube Marketing Templates</u></a></li>
<li><a href="https://win11.techidaily.com/a-handy-manual-assessing-and-annulling-window-history-data/"><u>A Handy Manual: Assessing & Annulling Window History Data</u></a></li>
<li><a href="https://some-techniques.techidaily.com/ai-vacation-planner-showdown-perplexity-versus-chatgpt-my-experience/"><u>AI Vacation Planner Showdown: Perplexity Versus ChatGPT - My Experience</u></a></li>
<li><a href="https://youtube-videos.techidaily.com/best-practices-for-designing-an-engaging-youtube-teaser-for-2024/"><u>Best Practices for Designing an Engaging YouTube Teaser for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/boosted-ai-capabilities-with-intel-core-ultra-pcs-experience-optimal-integration-of-cutting-edge-including-stable-diffusion/"><u>Boosted AI Capabilities with Intel Core Ultra PCs – Experience Optimal Integration of Cutting-Edge Including Stable Diffusion</u></a></li>
<li><a href="https://some-techniques.techidaily.com/californias-bold-move-prohibiting-new-gasoline-vehicle-purchases-by-2035/"><u>California's Bold Move: Prohibiting New Gasoline Vehicle Purchases by 2035</u></a></li>
<li><a href="https://some-techniques.techidaily.com/chatgpt-vs-google-translate-which-provides-superior-translation-accuracy/"><u>ChatGPT Vs. Google Translate: Which Provides Superior Translation Accuracy?</u></a></li>
<li><a href="https://some-techniques.techidaily.com/comparing-ideograms-and-midjourney-a-comprehensive-showdown/"><u>Comparing Ideograms and Midjourney: A Comprehensive Showdown</u></a></li>
<li><a href="https://some-techniques.techidaily.com/comprehensive-assessment-of-the-chipolo-card-spot-innovative-tracking-device-mimicking-credit-card-design/"><u>Comprehensive Assessment of the Chipolo CARD Spot: Innovative Tracking Device Mimicking Credit Card Design</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-exploring-ricoh-theta-s-in-full-review/"><u>In 2024, Exploring Ricoh Theta S in Full Review</u></a></li>
<li><a href="https://snapchat-videos.techidaily.com/in-2024-revisiting-old-memories-how-to-upload-them-on-snapchat/"><u>In 2024, Revisiting Old Memories How to Upload Them on Snapchat</u></a></li>
<li><a href="https://some-approaches.techidaily.com/in-2024-the-ultimate-list-premier-cameras-for-diving-and-snorkeling-enthusiasts/"><u>In 2024, The Ultimate List Premier Cameras for Diving & Snorkeling Enthusiasts</u></a></li>
<li><a href="https://fox-within.techidaily.com/mastering-system-fixes-navigating-through-windows-11-and-10-built-in-support/"><u>Mastering System Fixes: Navigating Through Windows 11 & 10 Built-In Support</u></a></li>
<li><a href="https://graphic-issues.techidaily.com/nvidia-card-not-compatible-with-windows-11-fix/"><u>Nvidia Card Not Compatible with Windows 11 [Fix]</u></a></li>
</ul></div>

