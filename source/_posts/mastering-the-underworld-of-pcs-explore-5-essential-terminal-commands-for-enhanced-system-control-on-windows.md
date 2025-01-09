---
title: "Mastering the Underworld of PCs: Explore 5 Essential Terminal Commands for Enhanced System Control on Windows"
date: 2025-01-07T20:17:03.933Z
updated: 2025-01-09T18:12:05.029Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://thmb.techidaily.com/1ed4f091728645649c840ae907d2be87aba494a53f4cf1942b1dcf1c240fc190.jpg
---

## Mastering the Underworld of PCs: Explore 5 Essential Terminal Commands for Enhanced System Control on Windows

### Key Takeaways

* Enable WSL and set terminal color to Matrix green for a hacker aesthetic.
* Install necessary commands and Linux distros via WSL for full functionality.
* Use commands like dir /s, ping -t, cmatrix, genact, and hollywood to simulate the hacker aesthetics.

 Ever wanted to feel like a Hollywood hacker without the associated risks? Here's how to transform your boring Windows terminal into a "hacker" space with five harmless commands.

##  Prerequisite: Enable WSL and Set Terminal Color to Matrix Green

 Some of the commands we will showcase are Linux native commands and don't run on Windows. But that’s nothing to worry about because you can easily run Linux commands on the Windows terminal by [enabling Windows Subsystem for Linux (WSL)](http://www.howtogeek.com/devops/what-is-windows-subsystem-for-linux-wsl-and-how-do-you-use-it/). Here’s a quick guide to enabling WSL:

1. Open the Start menu.
2. Search for **Turn Windows Features On or Off.**
3. Scroll down and check the box next to “Windows Subsystem for Linux.”
4. Click OK and restart your PC when prompted.
5. After restart, open the Microsoft Store and search for Ubuntu 24.04, or your preferred Linux distro.
6. Click Install and wait for it to download.
7. Once installed, open the Start Menu and search for **Ubuntu**.
8. Open Ubuntu and the Ubuntu Terminal window will appear.
9. Create a username and password.
10. And that’s it! You can now enter Linux Commands into this Ubuntu Terminal running on your Windows PC.

 With WSL enabled, we are ready to set the stage. Nothing says "hacker" quite like the iconic green-on-black text from _The Matrix_. Luckily, you can easily change the color of your Windows terminal to achieve this look. Just open Command Prompt and type:

color a

 or

color 2

![Windows command prompt color change to green](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/windows-command-prompt-color-change-to-green.png) 

 The "color" command only works in Windows Command Prompt (cmd) and not in PowerShell.

 Both of these commands will turn your text to a bright green color, instantly giving your terminal that classic hacker aesthetic. If you want to go back to the default colors, simply enter:

color

 Now that we've got the look down, let's move on to some commands that'll make you feel like a hacker.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/hHPljBHrvkA?si=HwdfDM9rlbABSIrx" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Use dir /s Command to Create a Lot of Scrolling Text

 The first command we'll look at is:

dir /s

 This command lists all files and directories in the current directory and all its subdirectories. When run from a high-level directory like the C Drive, it can produce an impressive amount of scrolling text that looks like you're diving deep into the system's file structure.

 Here's what the command does:

* dir: Lists files and directories
* /s: Includes all sub-directories

 To use it, simply open Command Prompt and type **dir /s** and watch as your screen fills with rapidly scrolling text, displaying every file and folder on your system.

Your browser does not support the video tag. 

 This command is not just for show and can be incredibly useful when you need to [find a specific file](https://facebook-video-content.techidaily.com/seamless-share-youtube-videos-set-up-autoplay-on-fb-for-2024/) or get an overview of your directory structure.

 Alternatively, to make it look even more impressive, this command:

dir /s | more

 It'll pause the output after each screenful of information—making it look like you're carefully analyzing each line of data.

![Windows cmd output of dir command with more](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/windows-cmd-output-of-dir-command-with-more.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/YpnYKIrpgZQ?si=94zicAHp1CH-0oso" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/iPCr_bxZjMQ?si=ubOsoq5umPEXL9xL" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Use the ping-t Command to Ping a Website Continuously

 Next up is the ping command with the -t option:

ping -t example.com

 The ping command is used to test the reachability of a host on an Internet Protocol (IP) network. Adding the -t option allows it to continue pinging the specified address until you stop it manually (by pressing Ctrl+C). Here's what it does:

* ping: Sends a network request to a specific IP address or domain
* \-t: Continues pinging until stopped
* example.com: The website you want to ping. e.g. google.com

Your browser does not support the video tag. 

 This command will continuously display the server’s response time, giving you real-time network performance data. It's not only visually appealing with its constant stream of data, but also practically useful for monitoring network connectivity.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/XVsiIO7hWOc?si=UvWnqxaI_yHwEr74" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Use cmatrix to Create the Iconic Matrix Text Rain (WSL necessary)

 Let's step it up a notch with a command that truly embodies the hacker aesthetic—cmatrix. This command creates the falling green text effect popularized by The Matrix movies. Now this is a Linux command, and you’ll need to first install it on your system before you can use it. To do this, open the Ubuntu terminal—or whichever Linux terminal you've installed using WSL, and enter the following command:

sudo apt install cmatrix

 After installation, simply type:

cmatrix

Your browser does not support the video tag. 

 Press CTRL+C to quit when you're done basking in the glow of your Matrix-inspired terminal.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/pRR3Oq03EuE?si=ZTy8-WH0AesA9zRh" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  Use genact to Simulate Running Random Tasks (WSL necessary)

 This is another fun Linux command that generates fake but realistic-looking activity in your terminal—perfect for when you want to look busy or just enjoy some tech-themed eye candy. Same as before, you’ll first need to install genact on your system. To do this, make sure you have Rust installed in your WSL environment by entering the following command in your WSL-backed Ubuntu terminal:

sudo snap install genact

 Once installed, you can run it simply by typing:

genact

Your browser does not support the video tag. 

 Genact will start displaying various fake activities, such as compiling code, running tests, or downloading files. It's completely harmless but looks impressively technical. Some of the modules you might see include:

* Cargo: Simulates building a Rust project
* Bootlog: Fakes downloading a file
* Cryptomining: Pretends to mine cryptocurrency
* Composer: Mimics compiling a Linux kernel

 The command for running the modules is like this:

genact -m _module-name_

    
 So, if you are trying to simulate cryptomining, this is the command you'll use:

genact -m cryptomining

Your browser does not support the video tag. 

##  Use hollywood to Feel Like a Hacker From The Movies (WSL necessary)

 For our final command, let’s pull out all the stops and go full overboard with “hollywood”. This is another Linux command that creates a split-screen terminal that looks like something straight out of a Hollywood movie—the stereotypical mainstream hacker visuals.

 You can run the command on your WSL powered Ubuntu terminal by entering:

hollywood

Your browser does not support the video tag. 

 As you can see, the terminal will split into multiple terminals, each running different commands and displaying various outputs. You'll see things like network scans, server logs, code compilations, system monitoring, and much more. It's a feast for the eyes and will definitely make anyone looking over your shoulder think you're engaged in some serious hacking. To exit hollywood, simply press Ctrl+C, and you'll be back to the base terminal.

 Now, in case, the command doesn't run, it means you'll need to first install it on your system. To do this, enter the following commands _one-by-one_ into the terminal.

        `sudo apt-add-repository ppa:hollywood/ppa  
sudo apt-get update  
sudo apt-get install byobu hollywood`
    
---

 So, as you can see, these five terminal commands can transform your Windows terminal into a hacker's playground. This can be a fun way to satisfy your inner cyberpunk or just impress (or scare) your friends.

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
<li><a href="https://some-techniques.techidaily.com/new-exciting-joint-ventures-in-the-virtual-metaverse/"><u>[New] Exciting Joint Ventures in the Virtual Metaverse</u></a></li>
<li><a href="https://digital-screen-recording.techidaily.com/new-real-time-game-recording-powered-by-obs-for-2024/"><u>[New] Real-Time Game Recording Powered by OBS for 2024</u></a></li>
<li><a href="https://facebook-video-share.techidaily.com/new-the-ultimate-playbook-to-create-compelling-youtube-educational-videos/"><u>[New] The Ultimate Playbook to Create Compelling YouTube Educational Videos</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/new-unlocking-the-potential-of-instagrams-filters-a-modern-guide-2e23-for-2024/"><u>[New] Unlocking the Potential of Instagram's Filters - A Modern Guide (2E23) for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-how-to-create-metaverse-avatar-easily-an-ultimate-guide/"><u>[Updated] How to Create Metaverse Avatar Easily An Ultimate Guide</u></a></li>
<li><a href="https://fox-access.techidaily.com/updated-in-2024-photoshop-stabilizers-role-crucial-for-creatives/"><u>[Updated] In 2024, Photoshop Stabilizer's Role - Crucial for Creatives?</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/updated-startup-strategy-guide-affordable-channels-to-monetize/"><u>[Updated] Startup Strategy Guide Affordable Channels to Monetize</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-expert-picks-for-superior-steadicams-in-aerial-cinema/"><u>2024 Approved Expert Picks for Superior Steadicams in Aerial Cinema</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-from-life-written-in-stillness-to-moving-pictures/"><u>2024 Approved From Life' Written in Stillness to Moving Pictures</u></a></li>
<li><a href="https://some-techniques.techidaily.com/fresh-take-on-sony-s6500-hd-dvd-and-bd-player-for-2024/"><u>Fresh Take on Sony S6500 HD DVD & BD Player for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/ideal-titles-superior-blu-ray-players-for-free-and-paid-users-for-2024/"><u>Ideal Titles Superior Blu-Ray Players for Free and Paid Users for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-exploring-magix-vpxs-innovative-editing-capabilities/"><u>In 2024, Exploring Magix VPX's Innovative Editing Capabilities</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-gag-generator-for-the-web/"><u>In 2024, Gag Generator for the Web</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/in-2024-how-to-cast-realme-11x-5g-screen-to-pc-using-wifi-drfone-by-drfone-android/"><u>In 2024, How to Cast Realme 11X 5G Screen to PC Using WiFi | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-how-to-curate-christian-chimes-for-devotion/"><u>In 2024, How to Curate Christian Chimes for Devotion</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/in-2024-wondering-the-best-alternative-to-hola-on-vivo-x-fold-2-here-is-the-answer-drfone-by-drfone-virtual-android/"><u>In 2024, Wondering the Best Alternative to Hola On Vivo X Fold 2? Here Is the Answer | Dr.fone</u></a></li>
<li><a href="https://win-exceptional.techidaily.com/ripara-iphone-bloccato-durante-la-migrazione-dei-dati-guida-completa-per-risolvere-i-problemi-di-trasferimento-su-iphone-13141516/"><u>Ripara iPhone Bloccato Durante La Migrazione Dei Dati: Guida Completa per Risolvere I Problemi Di Trasferimento Su iPhone 13/14/15/16</u></a></li>
<li><a href="https://tech-renaissance.techidaily.com/top-non-apple-non-tile-brands-discovering-exceptional-alternatives-to-the-famous-wallet-airtags-on-zdnet/"><u>Top Non-Apple, Non-Tile Brands: Discovering Exceptional Alternatives to the Famous Wallet AirTags on ZDNet</u></a></li>
<li><a href="https://howto.techidaily.com/what-to-do-if-google-play-services-keeps-stopping-on-xiaomi-civi-3-disney-100th-anniversary-edition-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>What to Do if Google Play Services Keeps Stopping on Xiaomi Civi 3 Disney 100th Anniversary Edition | Dr.fone</u></a></li>
</ul></div>

