---
title: Master the Art of Using Pipx for Easy Python App Deployment
date: 2024-10-27T21:39:47.782Z
updated: 2024-11-04T05:27:14.697Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/08/52848278425_0515827579_o.jpg
---

## Master the Art of Using Pipx for Easy Python App Deployment

### Key Takeaways

* Installing Python apps can be challenging due to potential conflicts with system packages, but pipx makes it easy by creating virtual environments and managing dependencies for you.
* Pipx is a user-friendly alternative to pip that installs apps system-wide without requiring sudo privileges, and it helps you add, upgrade, or remove Python apps effortlessly.
* With pipx, you can install Python CLI apps, run them just like standard Linux commands, and even uninstall them easily. It's a convenient tool for managing and expanding your app library.

 There are a ton of useful Python CLI apps out there, but installation isn't always as easy as it seems. Let's take a look at how pipx can make it easy to install and manage them.

##  Why Python Apps Are Tricky

 Installing Python apps can get hairy pretty quickly. [Python](https://youtube-data.techidaily.com/024-approved-conveniently-connect-with-others-via-your-playlist/) is a versatile language, and often the first people learn. Browsing [GitHub](https://github.com/) or [PyPI](https://pypi.org/)—the Python Package Index—you can find tons of useful apps alongside programming libraries. Since it's become so ubiquitous, there are a lot of folks contributing code, along with a mixture of instructions to install them.

 Most installation instructions tell you to install using pip, the package manager for python. Comparable to [apt](https://fake-location.techidaily.com/prank-your-friends-easy-ways-to-fake-and-share-google-maps-location-on-tecno-camon-20-premier-5g-drfone-by-drfone-virtual-android/) and yum for Linux, it uses PyPI as its repository and allows you to install libraries for your code as well as complete applications written in Python. However, installing software via the instance of pip that's on your system can cause conflicts with the packages already owned and managed by your regular package manager. Most Linux distributions these days utilize and depend on python and associated packages in order to run operating system functions, and other core software often relies on specific versions of certain libraries.

 I strongly discourage installing software at a system level with **sudo pip install** because this can cause conflicts with your system's package manager and result in broken functionality, or in the worst case situation, a non-booting system. I'm not alone in this, either, as [RealPython](https://realpython.com/python-virtual-environments-a-primer/#why-do-you-need-virtual-environments) and the [virtualenv documentation](https://virtualenv.pypa.io/en/latest/) recommend this, and even the [official Python docs](https://docs.python.org/3/tutorial/venv.html) call out the issue.

 Another option is to install at a user level with **pip install --user**, but not every package works flawlessly that way. Dependencies are still installed system-wide for that user, which can still cause problems as well.

 The Python community recommends using something called a virtual environment—often referred to as venvs—to create isolated folders that include all the required parts of a project to work, but using them when you're not familiar with the process can be very frustrating, especially if you're trying to script things. These are just some of the challenges users might face getting Python apps working on their system.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2105869/7443" target="_top" id="2105869">
  <img src="//a.impactradius-go.com/display-ad/7443-2105869" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2105869/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  pipx to the Rescue

 To solve our problems, we can use an application called pipx. This is a user-friendly alternative to pip that's aimed at end-users instead of programmers. It creates the virtual environments for you, installs the dependencies, and makes the programs available system-wide—all without requiring sudo privileges on your system as well. It also manages your installed python apps for you, making it easy to add, upgrade, or remove them as you see fit.

 Since pipx isn't intended for programmers, it doesn't support some of the critical features you'd want while developing, like installing editable packages for testing. This is strictly for users!

 To install pipx, the most straightforward way is to use your system's package manager. First, let's make sure the required packages are installed. If you're on a Debian-based distribution like Ubuntu, you can use apt.

sudo apt update && sudo apt install python3-venv python3-pip

![installing python3-venv and python3-pip](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/pipx01_update_install_deps-1.png) 

<!-- affiliate ads begin -->
<a href="https://bluetties.sjv.io/c/5597632/2141687/17094" target="_top" id="2141687">
  <img src="//a.impactradius-go.com/display-ad/17094-2141687" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://bluetties.sjv.io/i/5597632/2141687/17094" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 This will install the core packages for virtual environments and the pip package manager. Many Linux distributions will have these preinstalled, but not all. Crucially, versions of Debian and Ubuntu don't guarantee those packages will be preinstalled, so if you're on those distros you should run the above commands. If you're on a different distribution, use your relevant package manager, whether that's yum, pacman, or even brew.

 Next, we can install the pipx package itself.

![terminal window showing 'sudo apt install pipx' command](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/pipx03_install_pipx.png) 

sudo apt install pipx

 Lastly, we want to make sure that pipx is hooked into our path, so that installed apps will launch the same way all others do. We just need to run this pipx command:

pipx ensurepath

 Notice that there is no sudo for this command! Everything will work in user-space, which is exactly what we want in order to avoid messing with our operating system's Python installation.

![terminal window with a message telling the user that pipx's path has been set but a restart may be required](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/pipx06_ensurepath2.png) 

 On some distros, like Ubuntu, you may get a message that tells you that you may need to re-login for the path change to take effect. On Rhino Linux, things worked immediately, but on Ubuntu I had to log out and in again.

 And that's it, pipx is ready to go! Let's take a look at how to use it with some Python apps.

##  Installing Python CLI Apps

 Let's install a fun app called cowsay using pipx.

pipx install cowsay

![terminal window that shows the output of the cowsay command, a cow saying 'Welcome to How-To Geek!'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/pipx07_cowsay_command.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2012429/19272" target="_top" id="2012429">
  <img src="//a.impactradius-go.com/display-ad/19272-2012429" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2012429/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 You can use the Python app just as if it was a standard Linux command or app we installed. Under the hood, it's running in its own virtual environment, and any dependencies are separated and kept away from our core operating system.

 If you need to run an app just once, and you don't want to worry about installing and uninstalling, pipx has a run mode that handles that for you as well.

pipx run speedtest-cli

![terminal output of the speedtest command showing the bandwidth of the internet connection](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/pipx08_run.png) 

 You can also provide arguments for the app, so you can run specific commands. There are some caveats to the formatting, so be sure to check out the [official pipx documentation](https://pipx.pypa.io/stable/docs/#pipx-run).

 You can use pipx to see which installed Python apps you installed.

pipx list

![terminal window with the output of the pipx list command which shows only cowsay is installed](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/pipx09_list.png) 

 You can see that **speedtest-cli** is not installed, but **cowsay** is still present on our system.

 You can also uninstall the cowsay app easily.

pipx uninstall cowsay

![terminal window showing the pipx uninstall command output, which says it successfully uninstalled the cowsay app](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/pipx07a_uninstall_cowsay.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2075462/7443" target="_top" id="2075462">
  <img src="//a.impactradius-go.com/display-ad/7443-2075462" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2075462/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Where pipx really helps is in managing more complex applications. As an example, you can easily write [simple bash scripts](https://common-error.techidaily.com/rebooting-woes-windows-10-troubleshooting/) to launch and maintain the calibre-web app to host your own ebook library because you can treat it as just another command. Without pipx, the service files you need to write would be much trickier for someone who doesn't know Python and its deployment practices.

##  Expand Your App Library With pipx

 Now that you have pipx installed, there's a wealth of new programs available to you! If you find projects on GitHub or PyPI that you want to utilize, pipx can make it simple to install and use them in just a minute or two.

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
<li><a href="https://some-techniques.techidaily.com/new-exclusive-12-video-hourly-livestream-service/"><u>[New] Exclusive 12 Video Hourly Livestream Service</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-harnessing-the-power-of-slow-motion-pro-tips-for-gopro-hero-10-users/"><u>[New] Harnessing the Power of Slow Motion Pro Tips for GoPro Hero 10 Users</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-innovative-approaches-to-flawlessly-insert-chapters-into-your-youtube-content/"><u>[New] Innovative Approaches to Flawlessly Insert Chapters Into Your YouTube Content</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-innovative-investigation-vll-on-app-standards/"><u>[New] Innovative Investigation VLL on App Standards</u></a></li>
<li><a href="https://extra-skills.techidaily.com/new-leading-unboxing-series-s-must-watch-yt-channels/"><u>[New] Leading Unboxing Series 'S Must-Watch YT Channels</u></a></li>
<li><a href="https://facebook-video-content.techidaily.com/updated-facesavedownloader-suite-mobile-pc/"><u>[Updated] FaceSaveDownloader Suite (Mobile, PC)</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/updated-focus-frameworks-key-tools-to-brighten-videos/"><u>[Updated] Focus Frameworks Key Tools to Brighten Videos</u></a></li>
<li><a href="https://on-screen-recording.techidaily.com/updated-high-definition-capturing-for-switch-gamers-for-2024/"><u>[Updated] High Definition Capturing for Switch Gamers for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-hilarious-guide-crafting-memes-with-ease/"><u>[Updated] Hilarious Guide Crafting Memes with Ease</u></a></li>
<li><a href="https://video-screen-grab.techidaily.com/updated-in-2024-capture-and-share-your-win10-gaming-life/"><u>[Updated] In 2024, Capture and Share Your Win10 Gaming Life</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-infinite-professional-slideshow-resource-for-businesses/"><u>2024 Approved Infinite Professional Slideshow Resource for Businesses</u></a></li>
<li><a href="https://vp-tips.techidaily.com/elevate-your-savings-with-the-latest-apple-card-high-interest-banking-feature/"><u>Elevate Your Savings with the Latest Apple Card High-Interest Banking Feature</u></a></li>
<li><a href="https://some-techniques.techidaily.com/experience-the-future-of-mobile-gaming-iphone-vr-leaderboard-for-2024/"><u>Experience the Future of Mobile Gaming IPhone VR Leaderboard for 2024</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/in-2024-12-proven-ways-to-increase-youtube-views/"><u>In 2024, 12 Proven Ways to Increase YouTube Views</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-highlight-effects-assessment-essential-or-excessive/"><u>In 2024, Highlight Effects Assessment Essential or Excessive?</u></a></li>
<li><a href="https://win-howtos.techidaily.com/troubleshooting-persistent-disappearance-of-cursor-on-windows-10-devices/"><u>Troubleshooting: Persistent Disappearance of Cursor on Windows 10 Devices</u></a></li>
<li><a href="https://some-approaches.techidaily.com/ultimate-guide-to-hassle-free-mp4-video-transformation-into-a-full-sized-dvd/"><u>Ultimate Guide to Hassle-Free MP4 Video Transformation Into a Full-Sized DVD</u></a></li>
</ul></div>

