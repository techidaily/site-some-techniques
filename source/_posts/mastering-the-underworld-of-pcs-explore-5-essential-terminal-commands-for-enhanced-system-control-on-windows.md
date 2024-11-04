---
title: "Mastering the Underworld of PCs: Explore 5 Essential Terminal Commands for Enhanced System Control on Windows"
date: 2024-11-01T07:03:00.617Z
updated: 2024-11-03T17:18:09.899Z
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
<a href="https://zebaoaffiliateprogram.pxf.io/c/5597632/2137974/21526" target="_top" id="2137974">
  <img src="//a.impactradius-go.com/display-ad/21526-2137974" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://zebaoaffiliateprogram.pxf.io/i/5597632/2137974/21526" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://aligracehair.sjv.io/c/5597632/1938721/19272" target="_top" id="1938721">
  <img src="//a.impactradius-go.com/display-ad/19272-1938721" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1938721/19272" style="position:absolute;visibility:hidden;" border="0" />
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

##  Use cmatrix to Create the Iconic Matrix Text Rain (WSL necessary)

 Let's step it up a notch with a command that truly embodies the hacker aesthetic—cmatrix. This command creates the falling green text effect popularized by The Matrix movies. Now this is a Linux command, and you’ll need to first install it on your system before you can use it. To do this, open the Ubuntu terminal—or whichever Linux terminal you've installed using WSL, and enter the following command:

sudo apt install cmatrix

 After installation, simply type:

cmatrix

Your browser does not support the video tag. 

 Press CTRL+C to quit when you're done basking in the glow of your Matrix-inspired terminal.

<!-- affiliate ads begin -->
<a href="https://laganoo.pxf.io/c/5597632/1657386/16446" target="_top" id="1657386">
  <img src="//a.impactradius-go.com/display-ad/16446-1657386" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://laganoo.pxf.io/i/5597632/1657386/16446" style="position:absolute;visibility:hidden;" border="0" />
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

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2105864/7443" target="_top" id="2105864">
  <img src="//a.impactradius-go.com/display-ad/7443-2105864" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2105864/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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
<li><a href="https://extra-information.techidaily.com/new-constructing-an-intriguing-trailer-blueprint/"><u>[New] Constructing an Intriguing Trailer Blueprint</u></a></li>
<li><a href="https://vp-tips.techidaily.com/new-in-2024-tailoring-battery-choices-for-exceptional-drone-performance/"><u>[New] In 2024, Tailoring Battery Choices for Exceptional Drone Performance</u></a></li>
<li><a href="https://youtube-sure.techidaily.com/ed-how-does-youtube-work-after-a-video-is-uploaded/"><u>[Updated] How Does YouTube Work After a Video Is Uploaded</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-humorhub-generate-hilarious-jokes-and-gifs-easily/"><u>[Updated] HumorHub Generate Hilarious Jokes and GIFs Easily</u></a></li>
<li><a href="https://fox-http.techidaily.com/updated-simplifying-the-process-of-creating-time-lapses-with-gopro/"><u>[Updated] Simplifying the Process of Creating Time Lapses with GoPro</u></a></li>
<li><a href="https://some-techniques.techidaily.com/exceptional-book-video-examples-for-2024/"><u>Exceptional Book Video Examples for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/fabulous-review-and-diverse-options-for-2024/"><u>Fabulous Review & Diverse Options for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/from-niche-to-mainstream-amassing-a-million-view-channel-for-2024/"><u>From Niche to Mainstream Amassing a Million-View Channel for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/high-end-8-cam-modifiers-for-crystal-clear-feeds-for-2024/"><u>High-End 8 Cam Modifiers for Crystal Clear Feeds for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/high-end-uavs-purchase-without-delay-for-2024/"><u>High-End UAVs Purchase Without Delay for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/how-to-get-started-building-time-lapse-expertise-with-gopro-software-for-2024/"><u>How to Get Started Building Time-Lapse Expertise with GoPro Software for 2024</u></a></li>
<li><a href="https://ios-unlock.techidaily.com/how-to-unlock-iphone-15-plus-with-a-mask-on-by-drfone-ios/"><u>How to Unlock iPhone 15 Plus with a Mask On</u></a></li>
<li><a href="https://android-transfer.techidaily.com/in-2024-4-ways-to-transfer-music-from-vivo-y02t-to-iphone-drfone-by-drfone-transfer-from-android-transfer-from-android/"><u>In 2024, 4 Ways to Transfer Music from Vivo Y02T to iPhone | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-exploring-iphoneutility-mirror-photo-mastery-tips/"><u>In 2024, Exploring iPhone'utility Mirror Photo Mastery Tips</u></a></li>
<li><a href="https://iphone-unlock.techidaily.com/in-2024-how-to-unlock-iphone-se-passcode-screen-drfone-by-drfone-ios/"><u>In 2024, How to Unlock iPhone SE Passcode Screen? | Dr.fone</u></a></li>
<li><a href="https://facebook-videos.techidaily.com/in-2024-interactive-guide-twitter-and-facebook-synergy/"><u>In 2024, Interactive Guide Twitter & Facebook Synergy</u></a></li>
<li><a href="https://smart-video-creator.techidaily.com/new-edit-like-a-pro-gopro-video-editing-for-mac-users-2023-update/"><u>New Edit Like a Pro GoPro Video Editing for Mac Users (2023 Update)</u></a></li>
</ul></div>

