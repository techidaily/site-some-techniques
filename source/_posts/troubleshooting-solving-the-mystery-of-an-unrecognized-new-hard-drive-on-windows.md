---
title: "Troubleshooting: Solving the Mystery of an Unrecognized New Hard Drive on Windows"
date: 2024-11-11T17:00:21.434Z
updated: 2024-11-12T22:09:26.491Z
tags:
  - deals
categories:
  - tech
thumbnail: https://thmb.techidaily.com/290fdfbe7988bc73a9658535e5e89697be7bda898900fabab3b9425630194609.jpg
---

## Troubleshooting: Solving the Mystery of an Unrecognized New Hard Drive on Windows

### Quick Links

* [The Most Common Reason Your Disk Is Missing](https://fox-links.techidaily.com/new-2024-approved-essential-steps-to-prep-your-oculus-rift-zone/)
* [How to Bring Your Missing Drive Online](https://apple-account.techidaily.com/in-2024-your-account-has-been-disabled-in-the-app-store-and-itunes-from-iphone-13-by-drfone-ios/)

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2037334/7443" target="_top" id="2037334">
  <img src="//a.impactradius-go.com/display-ad/7443-2037334" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2037334/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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
<a href="https://appsumo.8odi.net/c/5597632/2151870/7443" target="_top" id="2151870">
  <img src="//a.impactradius-go.com/display-ad/7443-2151870" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2151870/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  How to Bring Your Missing Drive Online

 Assuming that the hard drive is installed properly, and is not, (by some horrible dumb luck) defective out of the gate, bringing it online is a very simple process. To do so, you first need to pull up the Windows Disk Management tool.

 Press Windows+R on your keyboard to launch the Run dialog box. Type **diskmgmt.msc** into the box and press Enter.

![img_57c452aa264cd](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c452aa264cd.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2082520/7443" target="_top" id="2082520">
  <img src="//a.impactradius-go.com/display-ad/7443-2082520" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2082520/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Before we proceed, we want to appropriately warn you: Do not play around in Disk Management. Although the task we're about to perform is very straightforward and simple to do, if you muck around with this tool you will have a very bad time. Double check every step. Make sure you're selecting the correct disk, or you can lose lots of data.

 Disk Management will likely detect that you have a new drive and prompt you to initialize it. You should pick GPT if this option appears, then click "OK." 

![Select 'GPT (GUID Partition Table),' then click 'OK.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/1-hdd-auto-detected.png) 

 If it doesn't show up, you just need to initialize it manually. In Disk Management, scroll down through the list of disks in the bottom pane. These disks will be labeled "Disk 1" through however many disks you have. Windows assigns a number to all hard disks, solid state disks, USB drives, and card readers, so don't be surprised if you have to scroll down a bit—in our case the new drive was "Disk 10" as seen below.

![img_57c45698e20bd](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45698e20bd.png) 

 There are four bits of information here that indicate we're looking at the right disk. First, the disk is marked as "unknown" and "Not initialized" on the left, which a brand-new disk introduced to the system would be flagged as. Second, the drive size matches the size of the drive we just installed (around 1 TB), and the drive is flagged as unallocated, which means none of the hard drive space has been formatted or assigned a partition.

 Right click on the name portion of the disk entry, where it says "Disk \[#\]", and select "Initialize Disk" from the right-click context menu.

![img_57c457c7c1208](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c457c7c1208.png) 

 In the first step of the initilization process, you'll be prompted to choose whether you want to use a Master Boot Record (MBR) or a GUID Partition Table (GPT) for the partition style of your disk. If you want to do some in depth reading before making a choice, you can [check out our explainer here](https://instagram-videos.techidaily.com/2024-approved-exclusive-guide-ranking-most-effective-ig-money-makers/). In short, unless you have a pressing reason to use MBR, use GPT instead—it's newer, more efficient, and offers more robust protection against corruptions of the boot record.

![img_57c45b8a5fff8](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45b8a5fff8.png) 

<!-- affiliate ads begin -->
<a href="https://laganoo.pxf.io/c/5597632/1528688/16446" target="_top" id="1528688">
  <img src="//a.impactradius-go.com/display-ad/16446-1528688" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://laganoo.pxf.io/i/5597632/1528688/16446" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Click "OK" and you'll be returned to the main Disk Management window. There you'll find that your disk is now labeled "Basic" and "Online" on the left, but the contents are still "unallocated". Right click on the striped box presenting the unallocated drive space. Select "New Simple Volume".

![img_57c45c0ad925a](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45c0ad925a.png) 

 This will launch the New Simple Volume Wizard to guide you through the process of setting up the disk. In the first step, select how much space you want to include in the volume. By default the number is the full amount of available disk space--unless you're planning on reserving space for additional partitions, there's no reason to change this. Click "Next".

![img_57c45c8fc3c3e](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45c8fc3c3e.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2082532/7443" target="_top" id="2082532">
  <img src="//a.impactradius-go.com/display-ad/7443-2082532" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2082532/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 In the second step, assign a drive letter. The default is probably fine.

![img_57c45d02176de](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45d02176de.png) 

 Finally, format the volume. If you're using the volume for routine computing tasks (storing photos, video games, etc.) there's no real need to deviate from the default NTFS file system and settings. Curious about the differences between file systems and why you might use the different options? We've [got you covered](https://extra-approaches.techidaily.com/seamless-multi-screen-browsing-in-chrome-using-pip-for-2024/). Give your volume a name, click "Next", and wait for the format process to finish.

![img_57c45d3ae14d7](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45d3ae14d7.png) 

 When the process is complete, you'll see your new drive--allocated, formatted, and ready for action--in the Disk Management disk list.

![img_57c45e2278bff](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45e2278bff.png) 

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
<li><a href="https://some-techniques.techidaily.com/new-expert-advice-optimizing-vlc-for-maximum-efficiency-on-mac/"><u>[New] Expert Advice Optimizing VLC for Maximum Efficiency on Mac</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-fast-track-fps-the-ultimate-speedy-extension-guide/"><u>[New] Fast-Track FPS The Ultimate Speedy Extension Guide</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-flip-page-film-narrative-guide/"><u>[New] Flip Page Film Narrative Guide</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-hear-the-difference-change-your-playstation-sound/"><u>[New] Hear the Difference Change Your PlayStation Sound</u></a></li>
<li><a href="https://article-helps.techidaily.com/updated-2024-approved-seamless-transition-from-photography-to-video-with-pixiz/"><u>[Updated] 2024 Approved Seamless Transition From Photography to Video with Pixiz</u></a></li>
<li><a href="https://article-posts.techidaily.com/updated-unleash-the-potential-of-videos-with-these-top-10-ios-apps/"><u>[Updated] Unleash the Potential of Videos with These Top 10 iOS Apps</u></a></li>
<li><a href="https://fox-blue.techidaily.com/2024-approved-cutting-edge-tech-in-daily-life/"><u>2024 Approved Cutting-Edge Tech in Daily Life</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-fresh-conversation-starters-keeping-listeners-hooked/"><u>2024 Approved Fresh Conversation Starters Keeping Listeners Hooked</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-gaming-galore-top-10-virtual-reality-for-phones/"><u>2024 Approved Gaming Galore Top 10 Virtual Reality for Phones</u></a></li>
<li><a href="https://extra-support.techidaily.com/2024-approved-mastering-podcast-release-schedules/"><u>2024 Approved Mastering Podcast Release Schedules</u></a></li>
<li><a href="https://youtube-help.techidaily.com/2024-approved-perfect-thumbnail-size-for-click-through-rates/"><u>2024 Approved Perfect Thumbnail Size for Click-Through Rates</u></a></li>
<li><a href="https://win-answers.techidaily.com/achieving-victory-over-call-of-duty-error-6328-in-warzone-ultimate-fix-guide-for-gamers/"><u>Achieving Victory over Call of Duty Error 6328 in Warzone - Ultimate Fix Guide for Gamers</u></a></li>
<li><a href="https://screen-recording.techidaily.com/augmenting-your-stardew-experience-with-seven-top-mods-for-2024/"><u>Augmenting Your Stardew Experience with Seven Top Mods for 2024</u></a></li>
<li><a href="https://app-tips.techidaily.com/debunking-common-errors-in-understanding-how-to-earn-from-big-data-a-deep-dive-nextgen-business-trends/"><u>Debunking Common Errors in Understanding How to Earn From Big Data: A Deep Dive | NextGen Business Trends</u></a></li>
<li><a href="https://games-able.techidaily.com/guide-to-overcoming-steam-server-disconnection/"><u>Guide to Overcoming Steam Server Disconnection</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-explore-the-pinnacle-of-photography-frames/"><u>In 2024, Explore the Pinnacle of Photography Frames</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-fast-tracking-fb-content-efficiency-strategies-explored/"><u>In 2024, Fast-Tracking FB Content Efficiency Strategies Explored</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-flip-clips-android-reversal-technique/"><u>In 2024, Flip Clips Android Reversal Technique</u></a></li>
<li><a href="https://buynow-reviews.techidaily.com/unlocking-potential-with-ankers-superspeed-usb-hub-in-depth-analysis-and-review/"><u>Unlocking Potential with Anker's SuperSpeed USB Hub - In-Depth Analysis & Review</u></a></li>
</ul></div>

