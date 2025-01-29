---
title: Impress Your Pals as a Fake Linux Guru with Just 5 Hilarious Bash Tricks
date: 2025-01-27T22:10:33.757Z
updated: 2025-01-28T21:45:47.616Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/ubuntu.jpg
---

## Impress Your Pals as a Fake Linux Guru with Just 5 Hilarious Bash Tricks

While I am a Linux daily driver, and I do sprinkle the terminal with commands now and then, I'm by no means a hacker. That didn't stop me from looking the part, though, since it turns out several simple commands (and a whole app) exist to make you look like a star in a florid cyberthriller. Here they are and how to run them.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/0dOfcihxjiw?si=_fkp1S1Uw0N1dp6b" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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
<iframe width="560" height="315" src="https://www.youtube.com/embed/ASUEYpqSP5E?si=0KOZxrTVexTuUkRn" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/U6lCtLUeROA?si=se6OFuis9JpcTGJf" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/ZLb1ViO4WR8?si=g_aiHGNCd7eAvmDM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/U_aNKnMTPjo?si=Og_mEt7NP3Fbsg2n" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://some-techniques.techidaily.com/updated-from-obscurity-to-influence-5-strategies-to-dominate-reddit-advertising/"><u>[Updated] From Obscurity to Influence 5 Strategies to Dominate Reddit Advertising</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-gigglegraphs-designing-delightful-memes/"><u>[Updated] GiggleGraphs Designing Delightful Memes</u></a></li>
<li><a href="https://extra-skills.techidaily.com/updated-leveraging-brand-partnerships-for-youtube-content-creators/"><u>[Updated] Leveraging Brand Partnerships for YouTube Content Creators</u></a></li>
<li><a href="https://screen-recording.techidaily.com/updated-recapturing-moments-the-xiaomi-mi-11s-superior-screen-record/"><u>[Updated] Recapturing Moments The Xiaomi Mi 11'S Superior Screen Record</u></a></li>
<li><a href="https://facebook-video-footage.techidaily.com/updated-recipes-that-resonate-best-practices-for-eating-themed-titles/"><u>[Updated] Recipes That Resonate Best Practices for Eating-Themed Titles</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-gopro-shootout-max-360-vs-hero-11-performance-analysis/"><u>2024 Approved GoPro Shootout Max 360 vs Hero 11 Performance Analysis</u></a></li>
<li><a href="https://youtube-docs.techidaily.com/oad-free-mcb-logo-templates-for-2024/"><u>Download Free MCB Logo Templates for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/fine-tuning-soundtracks-with-garageband-expertise-for-2024/"><u>Fine-Tuning Soundtracks with GarageBand Expertise for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/fiscally-friendly-action-footage-gear-for-2024/"><u>Fiscally-Friendly Action Footage Gear for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/high-staking-habitats-critical-commentary-for-2024/"><u>HIGH-STAKING HABITATS Critical Commentary for 2024</u></a></li>
<li><a href="https://activate-lock.techidaily.com/how-to-unlock-icloud-activation-lock-and-icloud-account-on-apple-iphone-6s-by-drfone-ios/"><u>How to Unlock iCloud Activation Lock and iCloud Account On Apple iPhone 6s?</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-from-still-life-to-motion-picture-a-complete-guide-on-pixiz-videos/"><u>In 2024, From Still Life to Motion Picture A Complete Guide on Pixiz Videos</u></a></li>
<li><a href="https://program-issues.techidaily.com/pc-gaming-fixes-overcoming-outpost-infinity-siege-freezing-issues/"><u>PC Gaming Fixes: Overcoming Outpost: Infinity Siege Freezing Issues</u></a></li>
<li><a href="https://youtube-sure.techidaily.com/er-capturing-device-for-exceptional-youtube-productions/"><u>Premier Capturing Device for Exceptional YouTube Productions</u></a></li>
<li><a href="https://fox-info.techidaily.com/selective-complementary-items-for-outstanding-gopros-for-2024/"><u>Selective Complementary Items for Outstanding GoPros for 2024</u></a></li>
<li><a href="https://driver-error.techidaily.com/the-evolution-and-functionality-of-usb-composite-devices-a-comprehensive-guide/"><u>The Evolution and Functionality of USB Composite Devices: A Comprehensive Guide</u></a></li>
</ul></div>

