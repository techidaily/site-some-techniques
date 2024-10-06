---
title: Impress Your Pals as a Fake Linux Guru with Just 5 Hilarious Bash Tricks
date: 2024-10-04T05:30:01.290Z
updated: 2024-10-05T18:48:57.124Z
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
<a href="https://ephamedtechinc.pxf.io/c/5597632/2137228/26400" target="_top" id="2137228">
  <img src="//a.impactradius-go.com/display-ad/26400-2137228" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://ephamedtechinc.pxf.io/i/5597632/2137228/26400" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://aligracehair.sjv.io/c/5597632/2012429/19272" target="_top" id="2012429">
  <img src="//a.impactradius-go.com/display-ad/19272-2012429" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2012429/19272" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://appsumo.8odi.net/c/5597632/2068425/7443" target="_top" id="2068425">
  <img src="//a.impactradius-go.com/display-ad/7443-2068425" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2068425/7443" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://aligracehair.sjv.io/c/5597632/1868586/19272" target="_top" id="1868586">
  <img src="//a.impactradius-go.com/display-ad/19272-1868586" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1868586/19272" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://youtube-zero.techidaily.com/024-approved-channel-up-your-earning-potential-with-youtube-shorts-strategy/"><u>[New] 2024 Approved Channel Up Your Earning Potential with YouTube Shorts Strategy</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-exclusive-insiders-take-on-best-3d-blu-ray-players/"><u>[New] Exclusive Insider's Take on Best 3D Blu-Ray Players</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-free-photo-editing-unleashed-android-and-iphones-top-tools-ranked/"><u>[New] Free Photo Editing Unleashed – Android & iPhone's Top Tools Ranked</u></a></li>
<li><a href="https://youtube-webster.techidaily.com/ow-much-could-you-make-on-youtube-snippets-for-2024/"><u>[New] How Much Could You Make on YouTube Snippets for 2024</u></a></li>
<li><a href="https://facebook-video-content.techidaily.com/2024-approved-amp-up-the-sound-beat-downloads-on-fb/"><u>2024 Approved Amp Up the Sound Beat Downloads on FB</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-ideal-fix-for-immersive-experiences/"><u>2024 Approved Ideal Fix for Immersive Experiences</u></a></li>
<li><a href="https://extra-skills.techidaily.com/2024-approved-quick-voice-mods-for-pubg-top-easy-techniques/"><u>2024 Approved Quick Voice Mods for PUBG Top Easy Techniques</u></a></li>
<li><a href="https://some-techniques.techidaily.com/how-to-harness-high-quality-artwork-at-no-cost-for-2024/"><u>How to Harness High-Quality Artwork at No Cost for 2024</u></a></li>
<li><a href="https://blog-min.techidaily.com/how-to-rescue-lost-contacts-from-huawei-p60-by-fonelab-android-recover-contacts/"><u>How to Rescue Lost Contacts from Huawei P60?</u></a></li>
<li><a href="https://tech-recovery.techidaily.com/how-to-seamlessly-bridge-airpods-and-your-macbook-air-a-step-by-nstep-guide/"><u>How to Seamlessly Bridge AirPods and Your MacBook Air: A Step-by-nStep Guide</u></a></li>
<li><a href="https://article-files.techidaily.com/in-2024-implementing-dynamic-filters-transform-your-videos-digitally/"><u>In 2024, Implementing Dynamic Filters Transform Your Videos Digitally</u></a></li>
<li><a href="https://win-solutions.techidaily.com/resolving-critical-development-bugs-in-call-of-duty-modern-warfare-and-warzone/"><u>Resolving Critical Development Bugs in Call of Duty Modern Warfare and Warzone</u></a></li>
<li><a href="https://extra-support.techidaily.com/top-7-must-have-metaverse-devices-you-need-to-prepare-for-2024/"><u>Top 7 Must-Have Metaverse Devices You Need to Prepare for 2024</u></a></li>
</ul></div>

