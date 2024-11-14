---
title: "Troubleshooting Guide: Why Won't My New SSD Appear on Windows? Discover Solutions"
date: 2024-11-09T16:06:30.697Z
updated: 2024-11-14T03:35:30.591Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://thmb.techidaily.com/8eb0a52f331cadec1455be55279efe68c9588c11451977d41c23dfeca435c0f3.jpg
---

## Troubleshooting Guide: Why Won't My New SSD Appear on Windows? Discover Solutions

### Quick Links

* [The Most Common Reason Your Disk Is Missing](https://fox-links.techidaily.com/new-2024-approved-essential-steps-to-prep-your-oculus-rift-zone/)
* [How to Bring Your Missing Drive Online](https://apple-account.techidaily.com/in-2024-your-account-has-been-disabled-in-the-app-store-and-itunes-from-iphone-13-by-drfone-ios/)

### Key Takeaways

* Hard drives you purchase aren't usually preformatted, so Windows waits for you to decide what to do with the drive.
* Open the Disk Management tool, identify your new (unformatted) drive, then right-click it and select "Initialize."
* After you initialize the drive, you must format it before you can store anything on it. Use NTFS if the drive will only be used in a Windows PC.

 You installed a new hard drive in your computer and, to your dismay, it's nowhere to be found. Don't panic, you just need to give Windows a little nudge to bring it online.

##  The Most Common Reason Your Disk Is Missing

 You grabbed a nice big hard disk on sale, you cracked open your computer case, plugged the drive into the motherboard and power supply with the appropriate cables (no? better double check that before you keep reading), and when you booted your computer back up the new hard drive was nowhere to be found.

 Or maybe you followed along with [our external hard drive tutorial](https://video-screen-grab.techidaily.com/new-diving-deep-into-minecraft-playback-secrets-from-the-pros/) and can't figure out why, even though you can hear the disk whirring away in the enclosure, you don't see the disk in Windows. What's the deal?

 Unlike the hard drive that ships with an off-the-shelf computer or external drive, extra hard drives you purchase aren't always shipped formatted and ready to use. Instead, they're in a totally blank state—the idea is that the end user will do what they wish with the drive, so there is no benefit to preformatting or otherwise changing the drive at the factory.

 As such, when you put the drive in your system, Windows simply waits for you to decide what to do with the drive instead of automatically formatting and adding it to the drive list. If you've never added a hard drive to your computer before, however, it can be pretty disconcerting when it appears like the drive is missing (or, worse, dead). Have no fear, though! It's easy to bring your hard drive out of hiding.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2111981/7443" target="_top" id="2111981">
  <img src="//a.impactradius-go.com/display-ad/7443-2111981" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2111981/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  How to Bring Your Missing Drive Online

 Assuming that the hard drive is installed properly, and is not, (by some horrible dumb luck) defective out of the gate, bringing it online is a very simple process. To do so, you first need to pull up the Windows Disk Management tool.

 Press Windows+R on your keyboard to launch the Run dialog box. Type **diskmgmt.msc** into the box and press Enter.

![img_57c452aa264cd](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c452aa264cd.png) 

 Before we proceed, we want to appropriately warn you: Do not play around in Disk Management. Although the task we're about to perform is very straightforward and simple to do, if you muck around with this tool you will have a very bad time. Double check every step. Make sure you're selecting the correct disk, or you can lose lots of data.

 Disk Management will likely detect that you have a new drive and prompt you to initialize it. You should pick GPT if this option appears, then click "OK." 

![Select 'GPT (GUID Partition Table),' then click 'OK.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/1-hdd-auto-detected.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2135351/19272" target="_top" id="2135351">
  <img src="//a.impactradius-go.com/display-ad/19272-2135351" border="0" alt="https://techidaily.com" width="125" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135351/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 If it doesn't show up, you just need to initialize it manually. In Disk Management, scroll down through the list of disks in the bottom pane. These disks will be labeled "Disk 1" through however many disks you have. Windows assigns a number to all hard disks, solid state disks, USB drives, and card readers, so don't be surprised if you have to scroll down a bit—in our case the new drive was "Disk 10" as seen below.

![img_57c45698e20bd](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45698e20bd.png) 

 There are four bits of information here that indicate we're looking at the right disk. First, the disk is marked as "unknown" and "Not initialized" on the left, which a brand-new disk introduced to the system would be flagged as. Second, the drive size matches the size of the drive we just installed (around 1 TB), and the drive is flagged as unallocated, which means none of the hard drive space has been formatted or assigned a partition.

 Right click on the name portion of the disk entry, where it says "Disk \[#\]", and select "Initialize Disk" from the right-click context menu.

![img_57c457c7c1208](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c457c7c1208.png) 

 In the first step of the initilization process, you'll be prompted to choose whether you want to use a Master Boot Record (MBR) or a GUID Partition Table (GPT) for the partition style of your disk. If you want to do some in depth reading before making a choice, you can [check out our explainer here](https://instagram-videos.techidaily.com/2024-approved-exclusive-guide-ranking-most-effective-ig-money-makers/). In short, unless you have a pressing reason to use MBR, use GPT instead—it's newer, more efficient, and offers more robust protection against corruptions of the boot record.

![img_57c45b8a5fff8](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45b8a5fff8.png) 

<!-- affiliate ads begin -->
<a href="https://unicoeye.pxf.io/c/5597632/2134239/18498" target="_top" id="2134239">
  <img src="//a.impactradius-go.com/display-ad/18498-2134239" border="0" alt="https://techidaily.com" width="721" height="90"/>
</a>
<img height="0" width="0" src="https://unicoeye.pxf.io/i/5597632/2134239/18498" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Click "OK" and you'll be returned to the main Disk Management window. There you'll find that your disk is now labeled "Basic" and "Online" on the left, but the contents are still "unallocated". Right click on the striped box presenting the unallocated drive space. Select "New Simple Volume".

![img_57c45c0ad925a](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45c0ad925a.png) 

<!-- affiliate ads begin -->
<a href="https://unicoeye.pxf.io/c/5597632/2134221/18498" target="_top" id="2134221">
  <img src="//a.impactradius-go.com/display-ad/18498-2134221" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://unicoeye.pxf.io/i/5597632/2134221/18498" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 This will launch the New Simple Volume Wizard to guide you through the process of setting up the disk. In the first step, select how much space you want to include in the volume. By default the number is the full amount of available disk space--unless you're planning on reserving space for additional partitions, there's no reason to change this. Click "Next".

![img_57c45c8fc3c3e](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45c8fc3c3e.png) 

 In the second step, assign a drive letter. The default is probably fine.

![img_57c45d02176de](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45d02176de.png) 

 Finally, format the volume. If you're using the volume for routine computing tasks (storing photos, video games, etc.) there's no real need to deviate from the default NTFS file system and settings. Curious about the differences between file systems and why you might use the different options? We've [got you covered](https://extra-approaches.techidaily.com/seamless-multi-screen-browsing-in-chrome-using-pip-for-2024/). Give your volume a name, click "Next", and wait for the format process to finish.

![img_57c45d3ae14d7](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45d3ae14d7.png) 

 When the process is complete, you'll see your new drive--allocated, formatted, and ready for action--in the Disk Management disk list.

![img_57c45e2278bff](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45e2278bff.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2080333/19272" target="_top" id="2080333">
  <img src="//a.impactradius-go.com/display-ad/19272-2080333" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2080333/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 You can now use the disk like any other on your system for media storage, games, and other purposes.

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
<li><a href="https://some-techniques.techidaily.com/new-excellent-easytime-timer-services/"><u>[New] Excellent EasyTime Timer Services</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-focused-frames-eliminating-jitterbugs/"><u>[New] Focused Frames Eliminating Jitterbugs</u></a></li>
<li><a href="https://screen-capture.techidaily.com/new-premium-online-audio-solutions-guide-for-2024/"><u>[New] Premium Online Audio Solutions Guide for 2024</u></a></li>
<li><a href="https://youtube-lab.techidaily.com/ed-2024-approved-channel-dynamo-craft-your-content-empire/"><u>[Updated] 2024 Approved Channel Dynamo Craft Your Content Empire</u></a></li>
<li><a href="https://snapchat-videos.techidaily.com/updated-2024-approved-conquer-chronological-chaos-snapchats-video-inversion/"><u>[Updated] 2024 Approved Conquer Chronological Chaos Snapchat's Video Inversion</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-expressive-faces-with-motion-blur-in-picsart/"><u>[Updated] Expressive Faces with Motion Blur in Picsart</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/complete-guide-for-recovering-photos-files-on-realme-note-50-by-fonelab-android-recover-photos/"><u>Complete guide for recovering photos files on Realme Note 50.</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/how-samsung-galaxy-s23-fe-mirror-screen-to-pc-drfone-by-drfone-android/"><u>How Samsung Galaxy S23 FE Mirror Screen to PC? | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/humorous-craftsmanship-access-without-expense-for-2024/"><u>Humorous Craftsmanship Access Without Expense for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-exploring-your-digital-trail-a-comprehensive-guide-to-previewing-off-facebook-activities/"><u>In 2024, Exploring Your Digital Trail - A Comprehensive Guide to Previewing Off-Facebook Activities</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-find-your-ideal-wedding-timer-on-android-and-ios-platforms-here/"><u>In 2024, Find Your Ideal Wedding Timer on Android & iOS Platforms Here</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-in-depth-modifying-ios-tones-for-max-impact/"><u>In 2024, In-Depth Modifying iOS Tones for Max Impact</u></a></li>
<li><a href="https://easy-unlock-android.techidaily.com/in-2024-lock-your-realme-narzo-n55-phone-in-style-the-top-5-gesture-lock-screen-apps-by-drfone-android/"><u>In 2024, Lock Your Realme Narzo N55 Phone in Style The Top 5 Gesture Lock Screen Apps</u></a></li>
<li><a href="https://hardware-help.techidaily.com/step-by-step-guide-to-upgrading-your-steelseries-arcteus-5-audio-experience-via-driver-download/"><u>Step-by-Step Guide to Upgrading Your SteelSeries Arcteus 5 Audio Experience via Driver Download</u></a></li>
<li><a href="https://extra-information.techidaily.com/swift-solutions-to-youtube-buffer-in-chrome-and-safari/"><u>Swift Solutions to YouTube Buffer in Chrome and Safari</u></a></li>
</ul></div>

