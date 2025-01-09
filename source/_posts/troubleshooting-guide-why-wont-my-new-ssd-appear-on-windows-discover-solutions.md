---
title: "Troubleshooting Guide: Why Won't My New SSD Appear on Windows? Discover Solutions"
date: 2025-01-03T18:38:22.821Z
updated: 2025-01-09T19:10:46.202Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://thmb.techidaily.com/8eb0a52f331cadec1455be55279efe68c9588c11451977d41c23dfeca435c0f3.jpg
---

## Troubleshooting Guide: Why Won't My New SSD Appear on Windows? Discover Solutions

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/GFHH14XlFCk?si=2HcjQbDx5eG0ZQAt" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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
<iframe width="560" height="315" src="https://www.youtube.com/embed/l4R7_qNIQvY?si=2zJOPfEcm6_3udzn" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  How to Bring Your Missing Drive Online

 Assuming that the hard drive is installed properly, and is not, (by some horrible dumb luck) defective out of the gate, bringing it online is a very simple process. To do so, you first need to pull up the Windows Disk Management tool.

 Press Windows+R on your keyboard to launch the Run dialog box. Type **diskmgmt.msc** into the box and press Enter.

![img_57c452aa264cd](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c452aa264cd.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/iOVkXoUxLf4?si=QfC18T2cb5OkiaXo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Before we proceed, we want to appropriately warn you: Do not play around in Disk Management. Although the task we're about to perform is very straightforward and simple to do, if you muck around with this tool you will have a very bad time. Double check every step. Make sure you're selecting the correct disk, or you can lose lots of data.

 Disk Management will likely detect that you have a new drive and prompt you to initialize it. You should pick GPT if this option appears, then click "OK." 

![Select 'GPT (GUID Partition Table),' then click 'OK.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/1-hdd-auto-detected.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/e4Nt2xXXtmE?si=CtKwFry4b0AJXnaN" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 If it doesn't show up, you just need to initialize it manually. In Disk Management, scroll down through the list of disks in the bottom pane. These disks will be labeled "Disk 1" through however many disks you have. Windows assigns a number to all hard disks, solid state disks, USB drives, and card readers, so don't be surprised if you have to scroll down a bit—in our case the new drive was "Disk 10" as seen below.

![img_57c45698e20bd](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45698e20bd.png) 

 There are four bits of information here that indicate we're looking at the right disk. First, the disk is marked as "unknown" and "Not initialized" on the left, which a brand-new disk introduced to the system would be flagged as. Second, the drive size matches the size of the drive we just installed (around 1 TB), and the drive is flagged as unallocated, which means none of the hard drive space has been formatted or assigned a partition.

 Right click on the name portion of the disk entry, where it says "Disk \[#\]", and select "Initialize Disk" from the right-click context menu.

![img_57c457c7c1208](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c457c7c1208.png) 

 In the first step of the initilization process, you'll be prompted to choose whether you want to use a Master Boot Record (MBR) or a GUID Partition Table (GPT) for the partition style of your disk. If you want to do some in depth reading before making a choice, you can [check out our explainer here](https://instagram-videos.techidaily.com/2024-approved-exclusive-guide-ranking-most-effective-ig-money-makers/). In short, unless you have a pressing reason to use MBR, use GPT instead—it's newer, more efficient, and offers more robust protection against corruptions of the boot record.

![img_57c45b8a5fff8](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45b8a5fff8.png) 

 Click "OK" and you'll be returned to the main Disk Management window. There you'll find that your disk is now labeled "Basic" and "Online" on the left, but the contents are still "unallocated". Right click on the striped box presenting the unallocated drive space. Select "New Simple Volume".

![img_57c45c0ad925a](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45c0ad925a.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/HSFNIAYChbA?si=4TIlsUrYmY5vP2il" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 This will launch the New Simple Volume Wizard to guide you through the process of setting up the disk. In the first step, select how much space you want to include in the volume. By default the number is the full amount of available disk space--unless you're planning on reserving space for additional partitions, there's no reason to change this. Click "Next".

![img_57c45c8fc3c3e](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45c8fc3c3e.png) 

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
<li><a href="https://some-techniques.techidaily.com/new-fading-out-the-louder-end-techniques-using-lumafusion/"><u>[New] Fading Out the Louder End Techniques Using Lumafusion</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-finding-sound-in-silence-3-cost-free-methods-to-music-enrich-your-videos/"><u>[New] Finding Sound in Silence 3 Cost-Free Methods to Music-Enrich Your Videos</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-friendly-frontier-metaverse-multiplayer-wonders/"><u>[New] Friendly Frontier Metaverse Multiplayer Wonders</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-hasten-your-windows-doc-analysis-process/"><u>[New] Hasten Your Windows Doc Analysis Process</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-innovating-with-technology-advanced-gopro-4k-editing-techniques/"><u>[New] Innovating with Technology Advanced GoPro 4K Editing Techniques</u></a></li>
<li><a href="https://screen-activity-recording.techidaily.com/new-obs-full-screen-fix-announced/"><u>[New] Obs Full-Screen Fix Announced</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-expert-tips-for-radial-blur-techniques-in-photoshop/"><u>[Updated] Expert Tips for Radial Blur Techniques in Photoshop</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-exploring-top-9-iphone-applications-for-adding-photo-water-marks/"><u>[Updated] Exploring Top 9 iPhone Applications for Adding Photo Water Marks</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/updated-in-2024-discovering-the-potential-apple-devices-on-your-youtube-channel/"><u>[Updated] In 2024, Discovering the Potential Apple Devices on Your YouTube Channel</u></a></li>
<li><a href="https://digital-screen-recording.techidaily.com/updated-turbo-testing-our-compreenas-five-best-racing-games/"><u>[Updated] Turbo Testing Our Compreenas Five Best Racing Games</u></a></li>
<li><a href="https://extra-resources.techidaily.com/a-comprehensive-guide-to-affordable-video-enhancement-websites-for-2024/"><u>A Comprehensive Guide to Affordable Video Enhancement Websites for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/expertise-in-iphones-macro-photography-secrets-revealed-for-2024/"><u>Expertise in iPhone's Macro Photography Secrets Revealed for 2024</u></a></li>
<li><a href="https://techidaily.com/how-to-factory-reset-xiaomi-redmi-13c-5g-without-losing-data-drfone-by-drfone-reset-android-reset-android/"><u>How to Factory Reset Xiaomi Redmi 13C 5G without Losing Data | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-explore-10-prime-online-stores-for-curious-gift-boxes/"><u>In 2024, Explore 10 Prime Online Stores for Curious Gift Boxes</u></a></li>
<li><a href="https://unlock-android.techidaily.com/in-2024-how-to-change-tecno-pop-8-lock-screen-password-by-drfone-android/"><u>In 2024, How To Change Tecno Pop 8 Lock Screen Password?</u></a></li>
<li><a href="https://ai-video-tools.techidaily.com/new-free-4k-video-converter-roundup-the-best-for-2024/"><u>New Free 4K Video Converter Roundup The Best for 2024</u></a></li>
<li><a href="https://some-guidance.techidaily.com/reach-out-to-our-creative-tech-experts-get-started-with-digiarty-today/"><u>Reach Out To Our Creative Tech Experts - Get Started with Digiarty Today!</u></a></li>
<li><a href="https://tech-haven.techidaily.com/streamlining-excel-processes-using-chatgpt-ai/"><u>Streamlining Excel Processes Using ChatGPT AI</u></a></li>
<li><a href="https://win11-tips.techidaily.com/supercharge-window-management-with-ingenious-hotkey-steps/"><u>Supercharge Window Management with Ingenious Hotkey Steps</u></a></li>
</ul></div>

