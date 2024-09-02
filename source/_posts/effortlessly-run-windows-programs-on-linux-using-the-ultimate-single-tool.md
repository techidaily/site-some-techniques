---
title: Effortlessly Run Windows Programs on Linux Using the Ultimate Single Tool
date: 2024-08-27 12:25:45
updated: 2024-08-29 10:25:18
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

##  Don't Forget to Adjust Bottles Preferences

 Bottles has a lot of settings that you can use to fine tune how your bottles are created, and what resources such as run time dependencies and DLLs are available for the applications inside your bottles.

 As we'll see, the defaults provided by Bottles for the different bottle types are sufficient for most case. But there’s still one setting that you might want to change. That’s where your bottles are created and stored in your file system.

 The default location is “\~/.var/app/com.usebottles.bottles/data/bottles/bottles/” for the Flatpak version of Bottles. The “/bottles/bottles” at the end of the path might look like a typo, but it’s not.

 We saw no need to change this location, but if you’d prefer to have your bottles and their applications stored on a particular location such as a large hard drive or fast SSD, you can change this location easily.

 Click on the hamburger menu icon, and select “Preferences” from the menu.

![The Preferences option in the Bottles hamburger menu](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/10-4.png) 

 The "Preferences" dialog appears.

![The "Bottles Directory" option in the General tab of the Prefrences dialog](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/11-4.png) 

 The bottom option on the “General” tab is “Bottles Directory.” Click the button at the end of that line to open a file browser dialog.

![The file dialog that allows you to browse to a location and set it as the location for the bottles you create](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/12-3.png) 

 Browse to the location you wish to use, then click the orange “Select” button.

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

 Work your way through the installation screens.

![The Notepad++ installation  dialog welcome screen](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/20.png) 

 Soon, you’ll see the final screen.

![The Notepad++ final installation screen, with the checkbox selected](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/21.png) 

 Leave the tick in the “Run Notepad++ v8.6.2” checkbox and click the “Finish” button. Notepad++ launches on your desktop.

![The Windows application, Notepad++ running on Linux](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/22.png) 

 Back in Bottles, you’ll see Notepad++ is listed as an installed program.

![Notepad++ listed as an installed application in our new bottle, with the run icon highlighted](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/23.png) 

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
