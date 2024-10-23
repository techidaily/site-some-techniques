---
title: "Troubleshooting: Solving the Mystery of an Unrecognized New Hard Drive on Windows"
date: 2024-10-16T19:43:44.115Z
updated: 2024-10-23T18:11:54.473Z
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
<a href="https://aligracehair.sjv.io/c/5597632/2135396/19272" target="_top" id="2135396">
  <img src="//a.impactradius-go.com/display-ad/19272-2135396" border="0" alt="https://techidaily.com" width="160" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135396/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  How to Bring Your Missing Drive Online

 Assuming that the hard drive is installed properly, and is not, (by some horrible dumb luck) defective out of the gate, bringing it online is a very simple process. To do so, you first need to pull up the Windows Disk Management tool.

 Press Windows+R on your keyboard to launch the Run dialog box. Type **diskmgmt.msc** into the box and press Enter.

![img_57c452aa264cd](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c452aa264cd.png) 

 Before we proceed, we want to appropriately warn you: Do not play around in Disk Management. Although the task we're about to perform is very straightforward and simple to do, if you muck around with this tool you will have a very bad time. Double check every step. Make sure you're selecting the correct disk, or you can lose lots of data.

 Disk Management will likely detect that you have a new drive and prompt you to initialize it. You should pick GPT if this option appears, then click "OK." 

![Select 'GPT (GUID Partition Table),' then click 'OK.'](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/02/1-hdd-auto-detected.png) 

 If it doesn't show up, you just need to initialize it manually. In Disk Management, scroll down through the list of disks in the bottom pane. These disks will be labeled "Disk 1" through however many disks you have. Windows assigns a number to all hard disks, solid state disks, USB drives, and card readers, so don't be surprised if you have to scroll down a bit—in our case the new drive was "Disk 10" as seen below.

![img_57c45698e20bd](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45698e20bd.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2094428/7443" target="_top" id="2094428">
  <img src="//a.impactradius-go.com/display-ad/7443-2094428" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2094428/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 There are four bits of information here that indicate we're looking at the right disk. First, the disk is marked as "unknown" and "Not initialized" on the left, which a brand-new disk introduced to the system would be flagged as. Second, the drive size matches the size of the drive we just installed (around 1 TB), and the drive is flagged as unallocated, which means none of the hard drive space has been formatted or assigned a partition.

 Right click on the name portion of the disk entry, where it says "Disk \[#\]", and select "Initialize Disk" from the right-click context menu.

![img_57c457c7c1208](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c457c7c1208.png) 

 In the first step of the initilization process, you'll be prompted to choose whether you want to use a Master Boot Record (MBR) or a GUID Partition Table (GPT) for the partition style of your disk. If you want to do some in depth reading before making a choice, you can [check out our explainer here](https://instagram-videos.techidaily.com/2024-approved-exclusive-guide-ranking-most-effective-ig-money-makers/). In short, unless you have a pressing reason to use MBR, use GPT instead—it's newer, more efficient, and offers more robust protection against corruptions of the boot record.

![img_57c45b8a5fff8](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45b8a5fff8.png) 

<!-- affiliate ads begin -->
<span id="1498635">
					<video width="320" height="320" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1498635.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/17326-1498635">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1498635.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:200px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fancheer.sjv.io%2Fc%2F5597632%2F1498635%2F17326'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1498635/17326" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Click "OK" and you'll be returned to the main Disk Management window. There you'll find that your disk is now labeled "Basic" and "Online" on the left, but the contents are still "unallocated". Right click on the striped box presenting the unallocated drive space. Select "New Simple Volume".

![img_57c45c0ad925a](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45c0ad925a.png) 

 This will launch the New Simple Volume Wizard to guide you through the process of setting up the disk. In the first step, select how much space you want to include in the volume. By default the number is the full amount of available disk space--unless you're planning on reserving space for additional partitions, there's no reason to change this. Click "Next".

![img_57c45c8fc3c3e](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45c8fc3c3e.png) 

 In the second step, assign a drive letter. The default is probably fine.

![img_57c45d02176de](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45d02176de.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2115921/19272" target="_top" id="2115921">
  <img src="//a.impactradius-go.com/display-ad/19272-2115921" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2115921/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Finally, format the volume. If you're using the volume for routine computing tasks (storing photos, video games, etc.) there's no real need to deviate from the default NTFS file system and settings. Curious about the differences between file systems and why you might use the different options? We've [got you covered](https://extra-approaches.techidaily.com/seamless-multi-screen-browsing-in-chrome-using-pip-for-2024/). Give your volume a name, click "Next", and wait for the format process to finish.

![img_57c45d3ae14d7](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45d3ae14d7.png) 

 When the process is complete, you'll see your new drive--allocated, formatted, and ready for action--in the Disk Management disk list.

![img_57c45e2278bff](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45e2278bff.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1896510/19272" target="_top" id="1896510">
  <img src="//a.impactradius-go.com/display-ad/19272-1896510" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1896510/19272" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://on-screen-recording.techidaily.com/updated-building-an-mc-village-housing-essentials/"><u>[Updated] Building an MC Village Housing Essentials</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-from-ineffectiveness-to-influence-with-smm-mastery/"><u>[Updated] From Ineffectiveness to Influence with SMM Mastery</u></a></li>
<li><a href="https://facebook-video-share.techidaily.com/updated-unveiling-the-secrets-of-youtube-music-curation/"><u>[Updated] Unveiling the Secrets of YouTube Music Curation</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-evening-stories-visualized-evaluations/"><u>2024 Approved Evening Stories Visualized Evaluations</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-from-meetings-to-media-how-zoom-powers-fb-live-content/"><u>2024 Approved From Meetings to Media How Zoom Powers FB Live Content</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-harness-the-power-of-wins11-new-gaming-titles/"><u>2024 Approved Harness the Power of Wins11 New Gaming Titles</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/2024-approved-the-5-superior-ps2-android-gaming-simulators-reviewed/"><u>2024 Approved The 5 Superior PS2 Android Gaming Simulators Reviewed</u></a></li>
<li><a href="https://extra-tips.techidaily.com/exploring-the-extents-of-vr-technology/"><u>Exploring the Extents of VR Technology</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/first-step-to-aerial-adventure-best-beginner-drones-for-2024/"><u>First Step to Aerial Adventure Best Beginner Drones for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/frugal-flight-assemblies-budget-friendly-drones-ranking-for-2024/"><u>Frugal Flight Assemblies Budget-Friendly Drones Ranking for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/heartstrings-harmony-best-music-to-accompany-your-engagement-for-2024/"><u>Heartstrings Harmony Best Music to Accompany Your Engagement for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-finding-the-most-skilled-film-capturers/"><u>In 2024, Finding the Most Skilled Film Capturers</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-humor-and-heartbreak-the-vhs-story-of-goofy-movie/"><u>In 2024, Humor and Heartbreak The VHS Story of Goofy Movie</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-innovations-in-crafting-engaging-vlogging-scripts/"><u>In 2024, Innovations in Crafting Engaging Vlogging Scripts</u></a></li>
<li><a href="https://youtube-stream.techidaily.com/lawful-ways-to-attain-a-million-followers-on-youtube-for-2024/"><u>Lawful Ways to Attain a Million Followers on YouTube for 2024</u></a></li>
<li><a href="https://extra-approaches.techidaily.com/periscope-streaming-made-simple-for-2024/"><u>Periscope Streaming Made Simple for 2024</u></a></li>
<li><a href="https://win-howtos.techidaily.com/troubleshooting-fixing-platform-not-supported-error-on-intel-serial-io-driver-installation/"><u>Troubleshooting: Fixing 'Platform Not Supported' Error on Intel Serial IO Driver Installation</u></a></li>
<li><a href="https://audio-editing.techidaily.com/updated-2024-approved-cadence-in-coding-envisioning-the-leading-luminaries-amongst-ai-music-architects/"><u>Updated 2024 Approved Cadence in Coding Envisioning the Leading Luminaries Amongst AI Music Architects</u></a></li>
<li><a href="https://youtube-clips.techidaily.com/youtubes-essential-learning-resources-for-upcoming-directors/"><u>YouTube's Essential Learning Resources for Upcoming Directors</u></a></li>
</ul></div>

