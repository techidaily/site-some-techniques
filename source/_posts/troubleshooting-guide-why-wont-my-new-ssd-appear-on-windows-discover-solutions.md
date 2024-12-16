---
title: "Troubleshooting Guide: Why Won't My New SSD Appear on Windows? Discover Solutions"
date: 2024-12-14T19:48:57.182Z
updated: 2024-12-16T01:01:52.890Z
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

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/RAnyQ0uj9Yg?si=Es4_ulcdM_-LuDcq" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  The Most Common Reason Your Disk Is Missing

 You grabbed a nice big hard disk on sale, you cracked open your computer case, plugged the drive into the motherboard and power supply with the appropriate cables (no? better double check that before you keep reading), and when you booted your computer back up the new hard drive was nowhere to be found.

 Or maybe you followed along with [our external hard drive tutorial](https://video-screen-grab.techidaily.com/new-diving-deep-into-minecraft-playback-secrets-from-the-pros/) and can't figure out why, even though you can hear the disk whirring away in the enclosure, you don't see the disk in Windows. What's the deal?

 Unlike the hard drive that ships with an off-the-shelf computer or external drive, extra hard drives you purchase aren't always shipped formatted and ready to use. Instead, they're in a totally blank state—the idea is that the end user will do what they wish with the drive, so there is no benefit to preformatting or otherwise changing the drive at the factory.

 As such, when you put the drive in your system, Windows simply waits for you to decide what to do with the drive instead of automatically formatting and adding it to the drive list. If you've never added a hard drive to your computer before, however, it can be pretty disconcerting when it appears like the drive is missing (or, worse, dead). Have no fear, though! It's easy to bring your hard drive out of hiding.

##  How to Bring Your Missing Drive Online

 Assuming that the hard drive is installed properly, and is not, (by some horrible dumb luck) defective out of the gate, bringing it online is a very simple process. To do so, you first need to pull up the Windows Disk Management tool.

 Press Windows+R on your keyboard to launch the Run dialog box. Type **diskmgmt.msc** into the box and press Enter.

![img_57c452aa264cd](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c452aa264cd.png) 

 Before we proceed, we want to appropriately warn you: Do not play around in Disk Management. Although the task we're about to perform is very straightforward and simple to do, if you muck around with this tool you will have a very bad time. Double check every step. Make sure you're selecting the correct disk, or you can lose lots of data.

 Disk Management will likely detect that you have a new drive and prompt you to initialize it. You should pick GPT if this option appears, then click "OK." 

![Select 'GPT (GUID Partition Table),' then click 'OK.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/1-hdd-auto-detected.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/cC-HtDQVoG0?si=nQcoa7q8q2IL8U0m" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 If it doesn't show up, you just need to initialize it manually. In Disk Management, scroll down through the list of disks in the bottom pane. These disks will be labeled "Disk 1" through however many disks you have. Windows assigns a number to all hard disks, solid state disks, USB drives, and card readers, so don't be surprised if you have to scroll down a bit—in our case the new drive was "Disk 10" as seen below.

![img_57c45698e20bd](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45698e20bd.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/fm0XhU5H8R4?si=cFPk6XK3X3CQSI7Y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 There are four bits of information here that indicate we're looking at the right disk. First, the disk is marked as "unknown" and "Not initialized" on the left, which a brand-new disk introduced to the system would be flagged as. Second, the drive size matches the size of the drive we just installed (around 1 TB), and the drive is flagged as unallocated, which means none of the hard drive space has been formatted or assigned a partition.

 Right click on the name portion of the disk entry, where it says "Disk \[#\]", and select "Initialize Disk" from the right-click context menu.

![img_57c457c7c1208](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c457c7c1208.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/FLO5dwmJAVs?si=1OYH8rv8aPaMsCiU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 In the first step of the initilization process, you'll be prompted to choose whether you want to use a Master Boot Record (MBR) or a GUID Partition Table (GPT) for the partition style of your disk. If you want to do some in depth reading before making a choice, you can [check out our explainer here](https://instagram-videos.techidaily.com/2024-approved-exclusive-guide-ranking-most-effective-ig-money-makers/). In short, unless you have a pressing reason to use MBR, use GPT instead—it's newer, more efficient, and offers more robust protection against corruptions of the boot record.

![img_57c45b8a5fff8](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45b8a5fff8.png) 

 Click "OK" and you'll be returned to the main Disk Management window. There you'll find that your disk is now labeled "Basic" and "Online" on the left, but the contents are still "unallocated". Right click on the striped box presenting the unallocated drive space. Select "New Simple Volume".

![img_57c45c0ad925a](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45c0ad925a.png) 

 This will launch the New Simple Volume Wizard to guide you through the process of setting up the disk. In the first step, select how much space you want to include in the volume. By default the number is the full amount of available disk space--unless you're planning on reserving space for additional partitions, there's no reason to change this. Click "Next".

![img_57c45c8fc3c3e](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45c8fc3c3e.png) 

 In the second step, assign a drive letter. The default is probably fine.

![img_57c45d02176de](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45d02176de.png) 

 Finally, format the volume. If you're using the volume for routine computing tasks (storing photos, video games, etc.) there's no real need to deviate from the default NTFS file system and settings. Curious about the differences between file systems and why you might use the different options? We've [got you covered](https://extra-approaches.techidaily.com/seamless-multi-screen-browsing-in-chrome-using-pip-for-2024/). Give your volume a name, click "Next", and wait for the format process to finish.

![img_57c45d3ae14d7](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45d3ae14d7.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/Zgwn5kVI5V4?si=1j6j4OuSSndFieXU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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
<li><a href="https://some-techniques.techidaily.com/new-freeing-up-your-screen-time-which-video-player-prevails-vlc-or-mpc/"><u>[New] Freeing Up Your Screen Time Which Video Player Prevails, VLC or MPC?</u></a></li>
<li><a href="https://video-screen-grab.techidaily.com/new-plex-vs-streaming-titanique/"><u>[New] Plex vs Streaming Titanique</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-exploring-5-engaging-book-promo-videos/"><u>[Updated] Exploring 5 Engaging Book Promo Videos</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-innovative-text-techniques-in-videos/"><u>[Updated] Innovative Text Techniques in Videos</u></a></li>
<li><a href="https://twitter-clips.techidaily.com/2024-approved-demystifying-twitter-archives-for-users-and-analysts/"><u>2024 Approved Demystifying Twitter Archives for Users & Analysts</u></a></li>
<li><a href="https://youtube-zero.techidaily.com/approved-the-blueprint-for-successful-valorant-thumbnails-on-social-media-platforms/"><u>2024 Approved The Blueprint for Successful Valorant Thumbnails on Social Media Platforms</u></a></li>
<li><a href="https://vp-tips.techidaily.com/effortless-dvd-to-ios-device-transfers-with-macx-for-mac-users-convert-and-rip-dvds-compatible-with-xs-xr-x-and-8-models/"><u>Effortless DVD to iOS Device Transfers with MacX for Mac Users – Convert and Rip DVDs Compatible With XS, XR, X, and 8 Models</u></a></li>
<li><a href="https://windows11.techidaily.com/how-to-counteract-dxgi-errors-after-device-loss/"><u>How to Counteract DXGI Errors After Device Loss</u></a></li>
<li><a href="https://fox-boxes.techidaily.com/in-2024-coding-warfare-comparing-the-superiority-of-av1-and-vp9/"><u>In 2024, Coding Warfare Comparing the Superiority of AV1 and VP9</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-evolved-windows-editor-programs-for-films/"><u>In 2024, Evolved Windows Editor Programs for Films</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-exclusive-guide-to-legal-gaming-music-without-price-tag/"><u>In 2024, Exclusive Guide to Legal Gaming Music Without Price Tag</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-expert-roundup-videonix-editors-capabilities/"><u>In 2024, Expert Roundup Videonix Editor's Capabilities</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-from-footage-to-fortune-unveiling-the-secrets-of-sj-cam-s6/"><u>In 2024, From Footage to Fortune Unveiling the Secrets of SJ-CAM S6</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-from-sound-to-sight-choosing-between-audio-and-video-media/"><u>In 2024, From Sound to Sight Choosing Between Audio and Video Media</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-improving-zoom-video-fidelity-easy-steps/"><u>In 2024, Improving Zoom Video Fidelity Easy Steps</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/in-2024-pokemon-go-cooldown-chart-on-tecno-spark-go-2024-drfone-by-drfone-virtual-android/"><u>In 2024, Pokémon Go Cooldown Chart On Tecno Spark Go (2024) | Dr.fone</u></a></li>
<li><a href="https://extra-lessons.techidaily.com/integrated-video-workflows-on-ios/"><u>Integrated Video Workflows on iOS</u></a></li>
<li><a href="https://video-creation-software.techidaily.com/new-2024-approved-how-to-remove-filmora-watermark-after-exporting-read-this-article-to-find-out-the-details-of-removing-the-filmora-watermark-even-without-p/"><u>New 2024 Approved How to Remove Filmora Watermark After Exporting? Read This Article to Find Out the Details of Removing the Filmora Watermark Even without Paying</u></a></li>
<li><a href="https://win11.techidaily.com/windows-11-taskbar-chat-ability-whats-it-mean-for-users/"><u>Windows 11 Taskbar Chat Ability: What's It Mean for Users?</u></a></li>
</ul></div>

