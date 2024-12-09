---
title: "Experience macOS Sequoia on Your Device: A Step-by-Step Guide for a Secure Trial"
date: 2024-12-04T17:04:28.374Z
updated: 2024-12-09T19:05:43.465Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://thmb.techidaily.com/298329c51bf36530c944afd2311460eb93803d5bd2abed16461ddf6c80bb2da9.jpg
---

## Experience macOS Sequoia on Your Device: A Step-by-Step Guide for a Secure Trial

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/U_aNKnMTPjo?si=Og_mEt7NP3Fbsg2n" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

### Quick Links

* [Install macOS Sequoia on a Separate Partition](https://mondly-stories.techidaily.com/a-complete-collection-of-top-16-german-gratefulness-statements/)
* [What About Installing macOS 15 Beta in a Virtual Machine?](https://fox-info.techidaily.com/horizon-captured-which-camera-takes-the-lead-in-2024/)

 Wondering what the next version of macOS is like? Try it out for yourself without risking your Mac by either installing it on a separate partition or using a virtual machine. Here’s how you can try both methods.

##  Install macOS Sequoia on a Separate Partition

 If you have the disk space to spare and you’re comfortable [playing around in Disk Utility](https://android-location-track.techidaily.com/in-2024-how-to-intercept-text-messages-on-vivo-y100i-power-5g-drfone-by-drfone-virtual-android/), you can install a pre-release version of macOS on a separate partition. You can retain your stable macOS installation on one partition, then reboot your Mac to try out the beta version.

 Your data won’t be affected, and you won’t even need to “sacrifice” disk space since macOS can take any data it needs from the main drive.

 It’s never a bad idea to [create a Time Machine backup](https://fox-hovers.techidaily.com/updated-2024-approved-navigating-the-path-free-and-safe-vlc-installer-for-macos-users/) before you start playing around with macOS partitions, just in case. Back up your Mac now, before you begin, so that you can restore your data if something goes wrong.

###  Download the macOS Sequoia Installer

 The first thing you’ll need to do is download the installer for the beta version of macOS that you want to download. The easiest way to do this is to use Terminal, which allows you to specify which version of macOS to download and places it ready in your Applications folder.

 You should do this using the same Mac on which you’re installing the beta, since Apple will detect your Mac and show appropriate releases.

 First, head to System Settings > General > Software Update then under “Beta Updates” choose the version of macOS that you want to install. We recommend the public beta, since developer betas can be even more unstable.

![Enable macOS beta updates.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/08/screenshot-2024-08-16-at-09-18-17.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/_dOmuXhsV6Y?si=aT6vgPbDx4ajjvdr" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Now open Terminal and run the following command:

softwareupdate --list-full-installers

 Wait a moment and your Mac will fetch a list of relevant installers.

![Download macOS installers using Terminal.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/08/screenshot-2024-08-16-at-12-15-13.png) 

 In the screenshot above we can see that 15.0 is the latest version. Now grab that specific installer using the following command:

softwareupdate --fetch-full-installer --full-installer-version 15.0

 Remember to replace the version number with the relevant version. Now wait for the installer to download. It’s around 15GB, so it may take a while.

 If the "list-full-installers" command isn’t working after you enabled the Beta flag in System Settings, restart your Mac and try again. If it's still not working, turn off beta participation and make sure your Mac is updated to the latest stable version of macOS and then switch beta participation back on and try again.

###  Create a New Partition for macOS Sequoia

 Now open Disk Utility and with your internal startup volume selected (probably labeled “Macintosh HD”), click the plus “+” icon near Volume. Give your new volume a name you can recognize, make sure “APFS” is selected, and don’t worry about specifying a size.

![Creating a new volume in "Macintosh HD."](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/08/screenshot-2024-08-16-at-14-50-04.png) 

 Click “Add” and your volume will be created. You can now close Disk Utility, you’re ready to install the macOS beta.

![Creating a partition for macOS Sequoia installation.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/08/screenshot-2024-08-16-at-14-55-38.png) 

###  Install macOS Sequoia on Your New Volume

 By now, you should hopefully have a new item in your Applications folder called “Install macOS 15 beta” (if you don’t, check the progress in that Terminal window).

![Running the macOS Sequoia beta installer.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/08/screenshot-2024-08-16-at-14-51-57.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/2Iv3DjT2Fyw?si=pR_z8ZDDVGF2MvKJ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 All that’s left to do is run this file and start the installation. Click “Continue” and on the next screen you’ll be invited to select an installation location. Click “Show All Disks” and select the volume you created earlier.

![Installing macOS Sequoia on a separate volume.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/08/screenshot-2024-08-16-at-14-56-49.png) 

 It’s worth double-checking to make sure that your main partition isn’t selected here, or you’ll overwrite your existing stable version of macOS.

 Hit “Continue” and choose whether to copy account settings. Finally, hit “Install” and enter a password if prompted. The macOS beta will be installed on the relevant partition.

![Final step of installing the macOS beta.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/08/screenshot-2024-08-16-at-14-57-35.png) 

 When the installation is finished, your Mac will restart and you’ll be invited to set up the new version of macOS [as if you were using a brand-new Mac](https://tech-recovery.techidaily.com/how-can-you-legally-download-netflix-titles-for-offline-viewing-on-a-laptop/).

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/GFHH14XlFCk?si=2HcjQbDx5eG0ZQAt" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

###  Switching Between Stable and Beta macOS Versions

 To pick which version of macOS you want to boot into, turn off your Mac using the Apple > Shut Down option.

 On an Apple Silicon Mac (with an M1 chip or later) press and hold the Power button (Touch ID sensor) to start your Mac, then choose the relevant partition. On an Intel Mac, press and hold Option then press the Power button (Touch ID sensor) and select the relevant partition.

 You’ll need to do this each time you want to swap between beta and stable macOS versions.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/KaqfZcWg5sE?si=LPmSKk7AFp8VxDFD" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

###  Deleting the macOS Beta

 To delete the beta, head back to Disk Utility from your stable version of macOS (in this case, macOS 14) and highlight the "macOS Sequoia" partition you created. Click on the minus "–" button next to "Volumes" and confirm by clicking "Delete."

![Deleting a macOS 15 volume.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/08/screenshot-2024-08-16-at-15-00-57.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/NTQGoOOiJzs?si=zbZwflEfXgBY3qbs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  What About Installing macOS 15 Beta in a Virtual Machine?

 This is supposed to be the part of the guide where I tell you how installing macOS 15 in a virtual machine is the easiest, least risky option. That’s technically true, but getting any of the macOS 15 betas working in a virtual machine isn’t necessarily straightforward.

 It should be a simple case of downloading the relevant IPSW from [Apple’s Developer website](https://developer.apple.com/download/) (which is now free or using a [free IPSW downloader](https://github.com/blacktop/ipsw) to swipe the relevant IPSW file), creating a [virtual machine in free tools like UTM](https://some-approaches.techidaily.com/transformative-approaches-to-engaging-with-online-video-reviews-for-2024/) and Virtual Buddy or a [paid tool like Parallels Desktop](https://screen-mirror.techidaily.com/in-2024-how-to-cast-oneplus-11r-screen-to-pc-using-wifi-drfone-by-drfone-android/), and you’re off to the races.

 After trying for several hours on a fully updated macOS 14 host, I was unable to create a working virtual machine for macOS 15\. This included installing the Xcode 16 beta, extracting and installing mobile support installers from the app directory, and even installing device support packages from Apple Developer.

 In UTM and Virtual Buddy (both of which are based on QEMU), I got a generic “installation failed” message. Parallels Desktop managed to create a virtual machine that terminated during the installation.

![An unhelpful error message in UTM for Mac.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/08/screenshot-2024-08-16-at-15-00-09.png) 

 There’s plenty of evidence online of people managing to get these methods working, and others failing miserably (as I did). This highlights the nature of pre-release software, where a few changes on Apple’s side can seemingly break compatibility with even paid virtualization solutions.

 And beta software is fleeting. While it’s likely that the final release of macOS 15 will work just fine in software like UTM and Parallels (just as macOS 14 does), the betas might never work.

 By the time you read this, there could be another beta out that fixes these issues and works fine. If you’re willing to give it a shot, we’ve included instructions below that might help.

###  Install macOS 15 Sequoia With UTM

**Download the Latest macOS and Xcode Beta** 

 To use a virtual machine like UTM, you’ll need to restore an IPSW image. These are provided by Apple with each beta release, and you can download them from [Apple’s Developer website](https://developer.apple.com/download/) (which is now free). Alternatively, you can use a [free IPSW downloader](https://github.com/blacktop/ipsw) to download the relevant IPSW file.

 You’ll also need to install “Device Support for macOS 15 beta” from the Apple Developer website.

**Create a Virtual Machine and Install macOS** 

 Once you’ve grabbed the latest beta version of macOS, it’s time to boot up UTM. Get started by clicking “Create a New Virtual Machine” and then choose “Virtualize” in the window that pops up.

 From here, select “macOS 12+” after which you’ll need to locate the IPSW file you downloaded using the “Browse” button.

 Now it’s time to configure your machine. Apple recommends at least 8GB RAM, but you can get away with 4GB if you’re tight on resources (remember this will be shared with the host machine). Next, specify four CPU cores, and nominate 80GB of disk space.

 Finally, give your machine a name and click “Save.” With your machine selected, click the “Play” button to get started. UTM will ask you if you want to install macOS, click “OK” and wait.

 read more

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/qObsqoJB9LI?si=ppqxfXzP0UL4J6Tp" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

###  Install macOS 15 Sequoia With Parallels Desktop

**Download the Latest macOS Beta IPSW** 

 To install macOS with Parallels Desktop, you’ll an IPSW image. Grab the latest version from [Apple’s Developer website](https://developer.apple.com/download/) (which is now free) or use a [free IPSW downloader](https://github.com/blacktop/ipsw) to download the relevant IPSW file.

 You’ll also need to install “Device Support for macOS 15 beta” from the Apple Developer website.

**Create a Virtual Machine and Install macOS** 

 Installing macOS in Parallels Desktop is really easy. First, open the app and click the plus “+” icon in Control Center. Choose “Install Windows, Linux, macOS from an image file” then click “Continue.”

 Drag your .IPSW file into the window, or click “select a file…” to locate it on your drive followed by “Continue.”

 Finally, click “Create” and wait for the installation process to complete.

 read more

---

 If you’d rather just find out what’s coming to your Mac without installing anything first, check out [our full roundup of the changes coming in macOS 15](https://youtube-tips.techidaily.com/approved-youtube-editing-essentials-the-ultimate-guide-post-upload-refinements/).

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
<li><a href="https://fox-direct.techidaily.com/new-2024-approved-elite-mac-video-editing-programs-sierra-edition/"><u>[New] 2024 Approved Elite Mac Video Editing Programs Sierra Edition</u></a></li>
<li><a href="https://eaxpv-info.techidaily.com/new-2024-approved-harmonize-your-imovie-projects-with-youtubes-melodies/"><u>[New] 2024 Approved Harmonize Your iMovie Projects With YouTube's Melodies</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-exploring-top-rated-frame-rate-choices-for-cinema-slow-motion/"><u>[New] Exploring Top-Rated Frame Rate Choices for Cinema Slow-Motion</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-from-black-and-white-to-richness-embracing-hdrs-power/"><u>[New] From Black and White to Richness Embracing HDR's Power</u></a></li>
<li><a href="https://facebook-videos.techidaily.com/new-mastering-facebook-visuals-adding-text-boxes-and-dark-bar-overlays/"><u>[New] Mastering Facebook Visuals Adding Text Boxes & Dark Bar Overlays</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-future-forward-entertainment-unveiling-the-lg-bp550-update/"><u>2024 Approved Future-Forward Entertainment Unveiling the LG BP550 Update</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-guide-to-progressive-audio-diminishment-via-lumafusion/"><u>2024 Approved Guide to Progressive Audio Diminishment via Lumafusion</u></a></li>
<li><a href="https://win11.techidaily.com/a-new-dawn-of-taskbars-in-windows-11-proposing-six-crucial-changes-for-enhanced-ux/"><u>A New Dawn of Taskbars in Windows 11: Proposing Six Crucial Changes for Enhanced UX</u></a></li>
<li><a href="https://extra-information.techidaily.com/androids-top-podcast-apps-showdown-6-innovators-revealed/"><u>Android's Top Podcast Apps Showdown 6 Innovators Revealed</u></a></li>
<li><a href="https://some-techniques.techidaily.com/from-pixels-to-perfection-the-advantages-of-srgb-over-rgb-for-2024/"><u>From Pixels to Perfection The Advantages of Srgb over Rgb for 2024</u></a></li>
<li><a href="https://techidaily.com/how-to-factory-reset-huawei-p60-in-5-easy-ways-drfone-by-drfone-reset-android-reset-android/"><u>How to Factory Reset Huawei P60 in 5 Easy Ways | Dr.fone</u></a></li>
<li><a href="https://blog-min.techidaily.com/how-to-recover-deleted-pictures-from-vivo-y100a-by-fonelab-android-recover-pictures/"><u>How to recover deleted pictures from Vivo Y100A.</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-illuminating-insights-for-iphone-night-photos/"><u>In 2024, Illuminating Insights for iPhone Night Photos</u></a></li>
<li><a href="https://easy-unlock-android.techidaily.com/in-2024-top-12-prominent-oppo-a78-fingerprint-not-working-solutions-by-drfone-android/"><u>In 2024, Top 12 Prominent Oppo A78 Fingerprint Not Working Solutions</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/top-10-airplay-apps-in-samsung-galaxy-a05-for-streaming-drfone-by-drfone-android/"><u>Top 10 AirPlay Apps in Samsung Galaxy A05 for Streaming | Dr.fone</u></a></li>
</ul></div>

