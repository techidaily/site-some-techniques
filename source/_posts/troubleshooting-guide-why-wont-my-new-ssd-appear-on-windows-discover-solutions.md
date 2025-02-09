---
title: "Troubleshooting Guide: Why Won't My New SSD Appear on Windows? Discover Solutions"
date: 2025-02-08T18:41:38.700Z
updated: 2025-02-09T17:01:04.896Z
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/iLlpdv0cz_k?si=HwTdnMmeVJXm4GPV" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  How to Bring Your Missing Drive Online

 Assuming that the hard drive is installed properly, and is not, (by some horrible dumb luck) defective out of the gate, bringing it online is a very simple process. To do so, you first need to pull up the Windows Disk Management tool.

 Press Windows+R on your keyboard to launch the Run dialog box. Type **diskmgmt.msc** into the box and press Enter.

![img_57c452aa264cd](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c452aa264cd.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/LeKJBWb6Jhk?si=AnViizAPiIT1YCRA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Before we proceed, we want to appropriately warn you: Do not play around in Disk Management. Although the task we're about to perform is very straightforward and simple to do, if you muck around with this tool you will have a very bad time. Double check every step. Make sure you're selecting the correct disk, or you can lose lots of data.

 Disk Management will likely detect that you have a new drive and prompt you to initialize it. You should pick GPT if this option appears, then click "OK." 

![Select 'GPT (GUID Partition Table),' then click 'OK.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/1-hdd-auto-detected.png) 

 If it doesn't show up, you just need to initialize it manually. In Disk Management, scroll down through the list of disks in the bottom pane. These disks will be labeled "Disk 1" through however many disks you have. Windows assigns a number to all hard disks, solid state disks, USB drives, and card readers, so don't be surprised if you have to scroll down a bit—in our case the new drive was "Disk 10" as seen below.

![img_57c45698e20bd](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45698e20bd.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/Vca--yEhtdo?si=7ijqjyP-oi3LYze1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 There are four bits of information here that indicate we're looking at the right disk. First, the disk is marked as "unknown" and "Not initialized" on the left, which a brand-new disk introduced to the system would be flagged as. Second, the drive size matches the size of the drive we just installed (around 1 TB), and the drive is flagged as unallocated, which means none of the hard drive space has been formatted or assigned a partition.

 Right click on the name portion of the disk entry, where it says "Disk \[#\]", and select "Initialize Disk" from the right-click context menu.

![img_57c457c7c1208](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c457c7c1208.png) 

 In the first step of the initilization process, you'll be prompted to choose whether you want to use a Master Boot Record (MBR) or a GUID Partition Table (GPT) for the partition style of your disk. If you want to do some in depth reading before making a choice, you can [check out our explainer here](https://instagram-videos.techidaily.com/2024-approved-exclusive-guide-ranking-most-effective-ig-money-makers/). In short, unless you have a pressing reason to use MBR, use GPT instead—it's newer, more efficient, and offers more robust protection against corruptions of the boot record.

![img_57c45b8a5fff8](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45b8a5fff8.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/T-ssCD10v2M?si=WVWGNayUiCAkMZzZ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Click "OK" and you'll be returned to the main Disk Management window. There you'll find that your disk is now labeled "Basic" and "Online" on the left, but the contents are still "unallocated". Right click on the striped box presenting the unallocated drive space. Select "New Simple Volume".

![img_57c45c0ad925a](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45c0ad925a.png) 

 This will launch the New Simple Volume Wizard to guide you through the process of setting up the disk. In the first step, select how much space you want to include in the volume. By default the number is the full amount of available disk space--unless you're planning on reserving space for additional partitions, there's no reason to change this. Click "Next".

![img_57c45c8fc3c3e](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45c8fc3c3e.png) 

 In the second step, assign a drive letter. The default is probably fine.

![img_57c45d02176de](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45d02176de.png) 

 Finally, format the volume. If you're using the volume for routine computing tasks (storing photos, video games, etc.) there's no real need to deviate from the default NTFS file system and settings. Curious about the differences between file systems and why you might use the different options? We've [got you covered](https://extra-approaches.techidaily.com/seamless-multi-screen-browsing-in-chrome-using-pip-for-2024/). Give your volume a name, click "Next", and wait for the format process to finish.

![img_57c45d3ae14d7](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45d3ae14d7.png) 

 When the process is complete, you'll see your new drive--allocated, formatted, and ready for action--in the Disk Management disk list.

![img_57c45e2278bff](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45e2278bff.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/DEqoiNArwjQ?si=oaL_lgnI-RxY5Qy_" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://facebook-record-videos.techidaily.com/new-brief-overview-of-the-quickest-chroma-key-tricks-for-2024/"><u>[New] Brief Overview of the Quickest Chroma Key Tricks for 2024</u></a></li>
<li><a href="https://remote-screen-capture.techidaily.com/new-elevating-sims-4-chronicles-advanced-techniques-for-precise-game-recording/"><u>[New] Elevating Sims 4 Chronicles Advanced Techniques for Precise Game Recording</u></a></li>
<li><a href="https://screen-sharing-recording.techidaily.com/new-expert-tips-to-enhance-your-iphone-memo-making-skills/"><u>[New] Expert Tips to Enhance Your iPhone Memo-Making Skills</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/new-viral-success-the-most-loved-ae-themes-for-social-media/"><u>[New] Viral Success The Most Loved AE Themes for Social Media</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-exploring-ustream-and-its-counterparts/"><u>[Updated] Exploring Ustream & Its Counterparts</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-grasping-the-advantages-of-av1-in-video-coding/"><u>[Updated] Grasping the Advantages of AV1 in Video Coding</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-ideal-e-commerce-avenues-for-aesthetic-box-personalization/"><u>[Updated] Ideal E-Commerce Avenues for Aesthetic Box Personalization</u></a></li>
<li><a href="https://youtube-sure.techidaily.com/approved-growth-in-focus-building-a-foundation-of-youtube-backlinks/"><u>2024 Approved Growth in Focus Building a Foundation of YouTube Backlinks</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-how-to-extend-the-usage-of-your-gopro-battery/"><u>2024 Approved How to Extend the Usage of Your GoPro Battery</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-innovative-approaches-to-flawlessly-insert-chapters-into-your-youtube-content/"><u>2024 Approved Innovative Approaches to Flawlessly Insert Chapters Into Your YouTube Content</u></a></li>
<li><a href="https://fox-access.techidaily.com/2024-approved-unearthing-the-skies-hubsan-h501x4-quad-drone-analysis/"><u>2024 Approved Unearthing the Skies Hubsan H501X4 Quad Drone Analysis</u></a></li>
<li><a href="https://some-techniques.techidaily.com/explore-virtual-realms-with-top-gadgets-and-peripherals-for-2024/"><u>Explore Virtual Realms with Top Gadgets and Peripherals for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/five-fantastic-iphones-for-podcast-fans-for-2024/"><u>Five Fantastic iPhones for Podcast Fans for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/from-static-to-dynamic-making-text-pop-on-instagram-stories-for-2024/"><u>From Static to Dynamic Making Text Pop on Instagram Stories for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-examining-dji-phantom-3s-advanced-video-capture-tech/"><u>In 2024, Examining DJI Phantom 3’S Advanced Video Capture Tech</u></a></li>
<li><a href="https://some-approaches.techidaily.com/in-2024-the-ultimate-guide-to-controlling-playback-rate-on-snapchat/"><u>In 2024, The Ultimate Guide to Controlling Playback Rate on Snapchat</u></a></li>
<li><a href="https://games-able.techidaily.com/peak-into-vrs-expensive-ecosystem-exploring-four-factors/"><u>Peak Into VR's Expensive Ecosystem: Exploring Four Factors</u></a></li>
<li><a href="https://data-safeguard.techidaily.com/stellar-repair-for-photo/"><u>Stellar Repair for Photo</u></a></li>
<li><a href="https://techno-recovery.techidaily.com/unraveling-code-43-errors-strategies-for-successful-correction/"><u>Unraveling Code 43 Errors: Strategies for Successful Correction</u></a></li>
</ul></div>

