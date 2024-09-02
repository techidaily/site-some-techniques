---
title: "Troubleshooting: Solving the Mystery of an Unrecognized New Hard Drive on Windows"
date: 2024-09-01T01:24:28.999Z
updated: 2024-09-02T01:24:28.999Z
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
<a href="https://ukaidot.sjv.io/c/5597632/1793234/19578" target="_top" id="1793234"><img src="//a.impactradius-go.com/display-ad/19578-1793234" border="0" alt="" width="678" height="452"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1793234/19578" style="position:absolute;visibility:hidden;" border="0" />
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

 There are four bits of information here that indicate we're looking at the right disk. First, the disk is marked as "unknown" and "Not initialized" on the left, which a brand-new disk introduced to the system would be flagged as. Second, the drive size matches the size of the drive we just installed (around 1 TB), and the drive is flagged as unallocated, which means none of the hard drive space has been formatted or assigned a partition.

 Right click on the name portion of the disk entry, where it says "Disk \[#\]", and select "Initialize Disk" from the right-click context menu.

![img_57c457c7c1208](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c457c7c1208.png) 

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4599951&QTY=1&AFFILIATE=108875&CART=1"><iframe width="864" height="500" src="https://www.youtube.com/embed/jVnfr5HudQw" title="The Latest and Easiest Solution to Remove Kindle DRM on Windows (without Degrading)" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
Epubor Ultimate for Win：Helps you read books anywhere, including the best eBook Converter + eBook DRM Removal functions.</a>
<!-- affiliate ads end -->
 In the first step of the initilization process, you'll be prompted to choose whether you want to use a Master Boot Record (MBR) or a GUID Partition Table (GPT) for the partition style of your disk. If you want to do some in depth reading before making a choice, you can [check out our explainer here](https://instagram-videos.techidaily.com/2024-approved-exclusive-guide-ranking-most-effective-ig-money-makers/). In short, unless you have a pressing reason to use MBR, use GPT instead—it's newer, more efficient, and offers more robust protection against corruptions of the boot record.

![img_57c45b8a5fff8](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45b8a5fff8.png) 

 Click "OK" and you'll be returned to the main Disk Management window. There you'll find that your disk is now labeled "Basic" and "Online" on the left, but the contents are still "unallocated". Right click on the striped box presenting the unallocated drive space. Select "New Simple Volume".

![img_57c45c0ad925a](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45c0ad925a.png) 

<!-- affiliate ads begin -->
<a href="https://bluetties.sjv.io/c/5597632/2039292/17094" target="_top" id="2039292"><img src="//a.impactradius-go.com/display-ad/17094-2039292" border="0" alt="BLUETTI NEW LAUNCH AC240" width="954" height="1020"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2039292/17094" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 This will launch the New Simple Volume Wizard to guide you through the process of setting up the disk. In the first step, select how much space you want to include in the volume. By default the number is the full amount of available disk space--unless you're planning on reserving space for additional partitions, there's no reason to change this. Click "Next".

![img_57c45c8fc3c3e](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45c8fc3c3e.png) 

 In the second step, assign a drive letter. The default is probably fine.

![img_57c45d02176de](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45d02176de.png) 

<!-- affiliate ads begin -->
<a href="https://store.massmailsoftware.com/order/checkout.php?PRODS=2069351&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/dc87c13749315c7217cdc4ac692e704c/banera_for_partners-24_%282%29.jpg" border="0"></a>
<!-- affiliate ads end -->
 Finally, format the volume. If you're using the volume for routine computing tasks (storing photos, video games, etc.) there's no real need to deviate from the default NTFS file system and settings. Curious about the differences between file systems and why you might use the different options? We've [got you covered](https://extra-approaches.techidaily.com/seamless-multi-screen-browsing-in-chrome-using-pip-for-2024/). Give your volume a name, click "Next", and wait for the format process to finish.

![img_57c45d3ae14d7](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45d3ae14d7.png) 

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=174416&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.easygifanimator.net/images/gif-animator.png" border="0">Easy GIF Animator is a powerful animated GIF editor and the top tool for creating animated pictures, banners, buttons and GIF videos. You get extensive animation editing features, animation effects, unmatched image quality and optimization for the web. No other GIF animation software matches our features and ease of use, that's why Easy GIF Animator is so popular.</a>
<!-- affiliate ads end -->
 When the process is complete, you'll see your new drive--allocated, formatted, and ready for action--in the Disk Management disk list.

![img_57c45e2278bff](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2016/08/img_57c45e2278bff.png) 

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=37701530&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/6fe0c81e3f9438db11ebbfba6c5ce460/products/copy_cbLogo_with_text_blue.png" border="0">CalendarBudget - Monthly subscription membership to CalendarBudget via web browser or mobile app. Support included. </a>
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
<li><a href="https://digital-screen-recording.techidaily.com/new-2024-approved-playful-pedal-powered-pastimes/"><u>[New] 2024 Approved  Playful Pedal-Powered Pastimes</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/new-2024-approved-unlocking-success-with-instagrams-business-platform/"><u>[New] 2024 Approved  Unlocking Success with Instagram's Business Platform</u></a></li>
<li><a href="https://extra-tips.techidaily.com/new-a-step-by-step-guide-to-video-aspect-ratio-selection/"><u>[New] A Step-by-Step Guide to Video Aspect Ratio Selection</u></a></li>
<li><a href="https://extra-lessons.techidaily.com/new-asus-proart-pa-329q-the-pinnacle-in-high-definition-viewing/"><u>[New] Asus ProArt PA 329Q  The Pinnacle in High-Definition Viewing</u></a></li>
<li><a href="https://tiktok-videos.techidaily.com/new-becoming-a-clone-mastermind-perfecting-the-copycat-artistry-on-tiktok/"><u>[New] Becoming a Clone Mastermind  Perfecting the Copycat Artistry on TikTok</u></a></li>
<li><a href="https://facebook-video-files.techidaily.com/new-brief-glimpses-in-the-social-space-for-2024/"><u>[New] Brief Glimpses in the Social Space for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-explore-and-outshine-cheapest-cloud-plans-for-every-need-2024/"><u>[New] Explore & Outshine  Cheapest Cloud Plans for Every Need, 2024</u></a></li>
<li><a href="https://screen-video-capture.techidaily.com/new-explore-the-best-webcams-on-your-windows-10-pc-for-2024/"><u>[New] Explore the Best Webcams on Your Windows 10 PC for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-extended-review-easy-dynamic-range-explained/"><u>[New] Extended Review  Easy Dynamic Range Explained</u></a></li>
<li><a href="https://facebook-videos.techidaily.com/new-free-mp4-conversion-tutorial-from-facebooks-high-definition-videos/"><u>[New] Free MP4 Conversion Tutorial From Facebook's High-Definition Videos</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-full-scrutiny-uncovering-the-dji-inspire-1-features/"><u>[New] Full Scrutiny  Uncovering the DJI Inspire 1 Features</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-go-beyond-basics-with-these-advanced-whatsapp-features/"><u>[New] Go Beyond Basics with These Advanced WhatsApp Features</u></a></li>
<li><a href="https://article-helps.techidaily.com/new-toolwiz-unpacked-expert-review-of-a-photography-powerhouse/"><u>[New] Toolwiz Unpacked  Expert Review of a Photography Powerhouse</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-expert-techniques-for-clearing-picture-edges/"><u>[Updated] Expert Techniques for Clearing Picture Edges</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-exploring-hues-from-textbooks-to-canvas/"><u>[Updated] Exploring Hues  From Textbooks to Canvas</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-exploring-vivacut-the-full-2024-video-editing-review/"><u>[Updated] Exploring VivaCut  The Full 2024 Video Editing Review</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-find-your-favorite-with-these-top-5-iphone-podcast-services/"><u>[Updated] Find Your Favorite with These Top 5 iPhone Podcast Services</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-harnessing-onscreen-power-expert-tips-on-cropping-images/"><u>[Updated] Harnessing Onscreen Power  Expert Tips on Cropping Images</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-how-to-find-the-optimal-balance-equipment-for-drone-photography/"><u>[Updated] How To Find the Optimal Balance Equipment for Drone Photography</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-imovie-cropping-mystery-unveiled/"><u>[Updated] IMovie Cropping Mystery Unveiled</u></a></li>
<li><a href="https://tiktok-video-recordings.techidaily.com/updated-unlock-creative-potential-crafting-tiktok-videos-using-templates-for-2024/"><u>[Updated] Unlock Creative Potential  Crafting TikTok Videos Using Templates for 2024</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/2024-approved-discover-the-top-tools-to-record-and-share-classroom-content/"><u>2024 Approved  Discover the Top Tools to Record and Share Classroom Content</u></a></li>
<li><a href="https://article-files.techidaily.com/2024-approved-fixing-iphone-x-overcoming-face-id-malfunction/"><u>2024 Approved  Fixing iPhone X  Overcoming Face ID Malfunction</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/a-working-guide-for-pachirisu-pokemon-go-map-on-lava-yuva-2-drfone-by-drfone-virtual-android/"><u>A Working Guide For Pachirisu Pokemon Go Map On Lava Yuva 2 | Dr.fone</u></a></li>
<li><a href="https://windows11.techidaily.com/arm-powered-windows-computers-get-official-chrome-support/"><u>ARM-Powered Windows Computers Get Official Chrome Support</u></a></li>
<li><a href="https://fox-boxes.techidaily.com/delving-into-magix-photo-editors-features/"><u>Delving Into MAGIX Photo Editor's Features</u></a></li>
<li><a href="https://some-techniques.techidaily.com/illuminating-the-future-luminances-influence-on-hdr-for-2024/"><u>Illuminating the Future  Luminance’s Influence on HDR for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/immersive-worlds-shaping-future-cinematic-experiences-for-2024/"><u>Immersive Worlds  Shaping Future Cinematic Experiences for 2024</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/in-2024-crafting-impressive-instagram-story-bokeh-art/"><u>In 2024, Crafting Impressive Instagram Story Bokeh Art</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-expert-opinion-on-slomo-recording-softwares-latest-version/"><u>In 2024, Expert Opinion on SloMo Recording Software's Latest Version</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-fine-tuning-the-art-of-recording-in-audacity/"><u>In 2024, Fine-Tuning the Art of Recording in Audacity</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-guide-to-convert-youtube-twitter-videos-to-mp3-songs/"><u>In 2024, Guide to Convert YouTube Twitter Videos to MP3 Songs</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-hasty-and-hassle-free-images-on-windows-11/"><u>In 2024, Hasty & Hassle-Free Images on Windows 11</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-hidden-methods-for-dodging-digital-study-vids/"><u>In 2024, Hidden Methods for Dodging Digital Study Vids</u></a></li>
<li><a href="https://facebook-clips.techidaily.com/in-2024-how-does-the-law-apply-to-video-sharing-on-facebook/"><u>In 2024, How Does the Law Apply to Video Sharing on Facebook?</u></a></li>
<li><a href="https://android-transfer.techidaily.com/in-2024-how-to-transfer-contacts-from-realme-v30-to-outlook-drfone-by-drfone-transfer-from-android-transfer-from-android/"><u>In 2024, How to Transfer Contacts from Realme V30 to Outlook | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-ideal-ae-text-sets-for-professional-work/"><u>In 2024, Ideal AE Text Sets for Professional Work</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-depth-review-and-step-by-step-tutorials-for-powerdirector-for-2024/"><u>In-Depth Review & Step-by-Step Tutorials for PowerDirector for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/innovative-tools-in-live-encoding-technology-for-2024/"><u>Innovative Tools in Live Encoding Technology for 2024</u></a></li>
<li><a href="https://fake-location.techidaily.com/ispoofer-is-not-working-on-motorola-edgeplus-2023-fixed-drfone-by-drfone-virtual-android/"><u>iSpoofer is not working On Motorola Edge+ (2023)? Fixed | Dr.fone</u></a></li>
<li><a href="https://win11-tips.techidaily.com/refine-your-terminal-experience-make-it-default/"><u>Refine Your Terminal Experience: Make It Default</u></a></li>
<li><a href="https://techidaily.com/repair-damaged-unplayable-video-files-of-honor-magic5-ultimate-by-stellar-video-repair-mobile-video-repair/"><u>Repair damaged, unplayable video files of Honor Magic5 Ultimate</u></a></li>
</ul></div>
