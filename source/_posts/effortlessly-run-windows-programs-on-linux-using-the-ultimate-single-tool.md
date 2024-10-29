---
title: Effortlessly Run Windows Programs on Linux Using the Ultimate Single Tool
date: 2024-10-26T16:05:51.449Z
updated: 2024-10-29T17:41:58.443Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/04/on-the-left-the-linux-mascot-and-the-bottle-app-logo-on-the-right-the-windows-logo-2.jpg
---

## Effortlessly Run Windows Programs on Linux Using the Ultimate Single Tool

### Quick Links

* [What Is Bottles?](https://unlock-android.techidaily.com/5-solutions-for-itel-p55-unlock-without-password-by-drfone-android/)
* [How to Install Bottles](https://techidaily.com/how-to-update-apple-iphone-11-pro-without-losing-data-drfone-by-drfone-ios-system-repair-ios-system-repair/)
* [Don't Forget to Adjust Bottles Preferences](https://screen-sharing-recording.techidaily.com/updated-2024-approved-ios-snapshot-spectrum-your-quick-reference/)
* [The Different Types of Bottle](https://fix-guide.techidaily.com/solved-warning-camera-failed-on-samsung-galaxy-a05s-drfone-by-drfone-fix-android-problems-fix-android-problems/)
* [Creating Your First Bottle](https://snapchat-videos.techidaily.com/snapchat-screen-recording-mobile-tips-and-tricks-for-2024/)
* [Running Our Windows Application](https://screen-capture.techidaily.com/updated-2024-approved-revolutionary-software-evolving-the-way-we-record-games/)
* [Fantastic, But Not Perfect](https://extra-support.techidaily.com/updated-music-video-shoot-estimated-financial-outlay/)

 You may already know that, thanks to the Wine project, you can run Windows applications on Linux. Wine is great, but it can be difficult for a beginner. Meet Bottles, an application that makes Wine much more manageable, accessible, and secure.

##  What Is Bottles?

 That’s a good question, but let’s take a step back. What is Wine? [Wine](http://www.winehq.org/) is a Linux application that makes Windows programs think they’re running in Microsoft Windows. It translates the calls the program would make to Windows, into Linux-compatible calls. It processes those requests and sends the responses back to the Windows program as though it was Windows that was replying. That’s an incredible achievement from an impressive project that’s [been around for a long time](https://some-guidance.techidaily.com/updated-ultimate-list-best-no-cost-lut-downloads/).

[Bottles is a visual wrapper for Wine](https://usebottles.com/). It still uses Wine as the technology to run the Windows applications, but it gives you an intuitive graphical interface so you don’t need to wrestle with Wine’s flexible but sometimes overwhelming configuration. After all, if you go to a store and buy wine, you don’t carry it home in your cupped hands. They give you a convenient glass container for that very purpose.

 Windows is the most commonly targeted platform for viruses and other malware, so there are risks to running Windows applications. Wine gives Windows applications access to your home drive with the same permissions and authority as you. Any malware you pick up has the same permissions. Bottles helps by sandboxing each Windows application, effectively acting as a container to confine the activities of applications and malware alike.

##  How to Install Bottles

 The best way to install Bottles is via Flatpak. In fact, it’s the only way to install Bottles that provides the full sandboxing capability, and it’s the officially recommended way.

 Both Manjaro Linux and Fedora Linux have Flatpak installed by default. On Ubuntu [you’ll need to install it](https://extra-support.techidaily.com/in-2024-marvelous-monitors-top-10-macbooks-with-4k-resolution/). Once Flatpak is set up, installing Bottles is simple.

flatpak install flathub com.usebottles.bottles

![Installing the Bottles flatpak on Linux](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/1-9.png) 

 The scrolling output will pause for you to confirm you wish to perform the installation.

![The Bottles flatpak installation requesting confirmation](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/2-8.png) 

 Type “Y” and hit “Enter.”

 The installation takes a little while. When it is completed, you can launch Bottles with this command.

flatpak run com.usebottles.bottles

![Launching the Bottles flatpak](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/3-8.png) 

 You’ll see some output as Bottles configures itself.

![The output from Bottles the first time it is launched](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/4-5.png) 

 Soon, Bottles launches, displaying the Welcome to Bottles introduction screens.

![The Bottles welcome screen](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/5-3.png) 

<!-- affiliate ads begin -->
<a href="https://bluettifr.pxf.io/c/5597632/2145082/17095" target="_top" id="2145082">
  <img src="//a.impactradius-go.com/display-ad/17095-2145082" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://bluettifr.pxf.io/i/5597632/2145082/17095" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Click the arrow button to move through the screens. On the Almost Done page, click the blue "Continue" button.

![Bottles' "Almost Done" welcome screen](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/6-8.png) 

 Bottles performs some further setup and configuration, then tells you it’s ready.

![Bottles' final welcome screen](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/8-5.png) 

 Click the blue “Start using Bottles” button to start using Bottles.

![The Bottles application straight after installation, with no bottles created](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/9-4.png) 

 With no Bottles created, the Library view is empty.

 You can also launch Bottles by finding it in your application view. On GNOME, press the "Super" key and start to type "Bottles."

![The Bottles icon in the GNOME application search results](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/24.png) 

 When you see the Bottles icon, click it to launch the application.

<!-- affiliate ads begin -->
<a href="https://imp.i357552.net/c/5597632/977686/11832" target="_top" id="977686">
  <img src="//a.impactradius-go.com/display-ad/11832-977686" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://imp.i357552.net/i/5597632/977686/11832" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Don't Forget to Adjust Bottles Preferences

 Bottles has a lot of settings that you can use to fine tune how your bottles are created, and what resources such as run time dependencies and DLLs are available for the applications inside your bottles.

 As we'll see, the defaults provided by Bottles for the different bottle types are sufficient for most case. But there’s still one setting that you might want to change. That’s where your bottles are created and stored in your file system.

 The default location is “\~/.var/app/com.usebottles.bottles/data/bottles/bottles/” for the Flatpak version of Bottles. The “/bottles/bottles” at the end of the path might look like a typo, but it’s not.

 We saw no need to change this location, but if you’d prefer to have your bottles and their applications stored on a particular location such as a large hard drive or fast SSD, you can change this location easily.

 Click on the hamburger menu icon, and select “Preferences” from the menu.

![The Preferences option in the Bottles hamburger menu](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/10-4.png) 

<!-- affiliate ads begin -->
<span id="1424529">
					<video width="864" height="1536" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1424529.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/16446-1424529">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1424529.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:540px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Flaganoo.pxf.io%2Fc%2F5597632%2F1424529%2F16446'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1424529/16446" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 The "Preferences" dialog appears.

![The "Bottles Directory" option in the General tab of the Prefrences dialog](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/11-4.png) 

<!-- affiliate ads begin -->
<a href="https://unicoeye.pxf.io/c/5597632/2148774/18498" target="_top" id="2148774">
  <img src="//a.impactradius-go.com/display-ad/18498-2148774" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://unicoeye.pxf.io/i/5597632/2148774/18498" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 The bottom option on the “General” tab is “Bottles Directory.” Click the button at the end of that line to open a file browser dialog.

![The file dialog that allows you to browse to a location and set it as the location for the bottles you create](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/12-3.png) 

 Browse to the location you wish to use, then click the orange “Select” button.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2123740/7443" target="_top" id="2123740">
  <img src="//a.impactradius-go.com/display-ad/7443-2123740" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2123740/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  The Different Types of Bottle

 Bottles provides a template for bottles that are geared towards gaming, and another that is more suited to general applications. It also provides a custom bottle template allowing you to configure your bottle yourself. This can also be used to run 32-bit software.

 Most of the time, and certainly for newcomers to Bottles, using either the gaming or applications templates is the easiest route to success.

 We’re going to use the template for applications.

##  Creating Your First Bottle

 To create your bottle, select “Bottles” from the toolbar, then click on the blue “Create New Bottle” button.

![The empty Bottles page](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/13-2.png) 

 We’re going to [install Notepad++](https://instagram-video-files.techidaily.com/updated-2024-approved-top-10-best-apps-for-editing-igtv-vertical-videos/), a Windows-only editor. We named our bottle “Notepad++”, and selected the “Application” radio button.

![Selecting the Application bottle type](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/14-2.png) 

 Click the blue “Create” button to create your bottle.

![The output while Bottles creates a new bottle](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/15-1.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1902294/19272" target="_top" id="1902294">
  <img src="//a.impactradius-go.com/display-ad/19272-1902294" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1902294/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Bottles configures your bottle and Wine, then tells you the process is complete.

![The confirmation when a bottle has been created](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/16-1.png) 

 Click the blue “Close” button to close the dialog. You can see the details of your new bottle.

![The details of the new bottle, and the options that can be used to fine tune and use it](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/17.png) 

##  Running Our Windows Application

 The “Install Programs” option lets you install some commonly used applications, wrapped by members of the Bottles user community. The “Dependencies” option lets you install resources that your application might need, such as runtimes, DLLs, or Microsoft fonts,

 We’re going to use the blue “Run Executable” to run the Notepad++ installer. This was already downloaded to my “\~/Downloads” directory.

 Browse to the location of the downloaded installer. Click on the file to highlight it, then click the “Run” button.

![Browsing to, and selecting, the installation file](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/18.png) 

 We see the usual Notepad++ installation dialog.

![The Notepad++ installation dialog](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/19.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2151854/7443" target="_top" id="2151854">
  <img src="//a.impactradius-go.com/display-ad/7443-2151854" border="0" alt="https://techidaily.com" width="600" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2151854/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Work your way through the installation screens.

![The Notepad++ installation  dialog welcome screen](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/20.png) 

 Soon, you’ll see the final screen.

![The Notepad++ final installation screen, with the checkbox selected](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/21.png) 

 Leave the tick in the “Run Notepad++ v8.6.2” checkbox and click the “Finish” button. Notepad++ launches on your desktop.

![The Windows application, Notepad++ running on Linux](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/22.png) 

 Back in Bottles, you’ll see Notepad++ is listed as an installed program.

![Notepad++ listed as an installed application in our new bottle, with the run icon highlighted](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/23.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1938682/19272" target="_top" id="1938682">
  <img src="//a.impactradius-go.com/display-ad/19272-1938682" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1938682/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Clicking the arrow head icon launches Notepad++ for us, whenever we wish to use it.

##  Fantastic, But Not Perfect

 There are Linux equivalents to most Windows applications, but they sometimes do things differently or don’t replicate all the functionality of their Windows equivalent. This can flummox newcomers to Linux. Sometimes, especially with games, there simply are no Linux equivalents.

 Bottles makes running the original Windows applications right inside your Linux computer pretty easy in most cases. If your application doesn’t want to run, check out the [Bottles forum](https://forum.usebottles.com/). You won’t be the first to have had your problem, and there may well be a known remedy.

 As wonderful as it is, Wine isn’t perfect. And so Bottles isn’t perfect. But Bottles makes using Wine much more palatable.

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
<li><a href="https://youtube-lab.techidaily.com/024-approved-youtube-film-craft-mastering-thumbnail-creation-on-mobiles/"><u>[New] 2024 Approved YouTube Film Craft Mastering Thumbnail Creation on Mobiles</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-excellence-in-vocal-alteration-top-choices-above-all/"><u>[New] Excellence in Vocal Alteration Top Choices Above All</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/updated-2024-approved-chromebook-screenshots-made-easy-top-5-app-choices/"><u>[Updated] 2024 Approved Chromebook Screenshots Made Easy Top 5 App Choices</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-exclusive-list-10-budget-friendly-passport-photographers-online/"><u>[Updated] Exclusive List 10 Budget-Friendly Passport Photographers Online</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-high-fidelity-footage-face-off-hero5-black-vs-hero4-silver/"><u>[Updated] High Fidelity Footage Face-Off Hero5 Black vs Hero4 Silver</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/updated-in-2024-in-depth-tutorial-for-gameplay-recorders-on-win10/"><u>[Updated] In 2024, In-Depth Tutorial for Gameplay Recorders on Win10</u></a></li>
<li><a href="https://extra-resources.techidaily.com/beginners-guide-to-changing-speed-up-in-videos-on-snapchat/"><u>Beginner’s Guide to Changing Speed Up in Videos on Snapchat</u></a></li>
<li><a href="https://techno-recovery.techidaily.com/best-reading-apps-of-2024-picked-by-us-top-8-selections/"><u>Best Reading Apps of 2024 (Picked by Us) - Top 8 Selections</u></a></li>
<li><a href="https://some-techniques.techidaily.com/explore-these-non-periscope-video-platforms-for-iphones-and-androids-for-2024/"><u>Explore These Non-Periscope Video Platforms for iPhones & Androids for 2024</u></a></li>
<li><a href="https://facebook-clips.techidaily.com/facebooks-shift-to-short-videos-a-look-into-2023-trends/"><u>Facebook's Shift to Short Videos A Look Into 2023 Trends</u></a></li>
<li><a href="https://some-techniques.techidaily.com/haul-videography-101-preparation-and-editing-for-maximum-impact-for-2024/"><u>Haul Videography 101 Preparation & Editing for Maximum Impact for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-explore-the-best-in-class-pc-vr-headsets/"><u>In 2024, Explore the Best-In-Class PC VR Headsets</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-free-red-eye-correction-for-iphone-users-tips-and-tricks/"><u>In 2024, Free Red-Eye Correction for iPhone Users - Tips and Tricks</u></a></li>
<li><a href="https://android-location-track.techidaily.com/in-2024-solutions-to-spy-on-lava-yuva-3-with-and-without-jailbreak-drfone-by-drfone-virtual-android/"><u>In 2024, Solutions to Spy on Lava Yuva 3 with and without jailbreak | Dr.fone</u></a></li>
<li><a href="https://some-approaches.techidaily.com/the-10-most-admirable-photo-frame-apps-for-2024/"><u>The 10 Most Admirable Photo Frame Apps for 2024</u></a></li>
<li><a href="https://buynow-marvelous.techidaily.com/vyans-tracking-service-analysis-reliable-monitoring-tool-with-puzzling-membership-options/"><u>Vyans Tracking Service Analysis: Reliable Monitoring Tool with Puzzling Membership Options</u></a></li>
</ul></div>

