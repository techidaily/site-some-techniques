---
title: "Comprehensive Guide: Managing Access Rights Using Linux's Access Control Lists"
date: 2024-11-09T23:56:21.022Z
updated: 2024-11-14T00:45:31.893Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://thmb.techidaily.com/292b65daa58a3cb7189f78d0565b817f09110724b35903d3b3e9b8eb64f84eb9.jpg
---

## Comprehensive Guide: Managing Access Rights Using Linux's Access Control Lists

### Key Takeaways

* To view all ACL entries for a file, use the command 'getfacl filename' but replace 'filename' with the name of your file.
* To set a new ACL entry for a file, use the command 'setfacl -m u:username:rwx filename'
* To set a Default ACL entry on a directory, use the command 'setfacl -d -m u:username:rwx dirname'

 Are you in charge of a shared file server between multiple groups of people, who all need varying access? In this tutorial we'll go over the basics of ACLs and employ them in a fictional office scenario.

##  What Are ACLs?

 Access Control Lists (ACLs) supplement the [standard file system permissions model on Linux and Unix](https://os-tips.techidaily.com/how-to-reset-waze-location-memory-on-ios-devices-a-step-by-step-guide/). In a nutshell, they allow you to go beyond the "user/group/other" concept to create additional sets of permissions for files and directories. They also do neat things like automatically applying permissions to new files and directories. But first, let's cover some basic Linux file system permissions concepts in which ACLs work alongside.

###  Standard File System Permissions

 To understand file system permissions under Linux, first you need to know that Linux is a "multi-user operating system". This means there exist multiple [user accounts](https://fox-links.techidaily.com/updated-gif-magic-transformations-without-extra-files-downloaded-for-2024/) which essentially allow more than one person to log into the system, each having their own freedoms and restrictions.

 Some user accounts are "system" accounts; not ones that are used by a person, but rather by a piece of software, for instance. Processes run under these special accounts to allow and restrict them to various parts of the OS, just as a normal user account would.

 Now that we understand users, I can introduce you to "groups." Groups are pretty easy to understand—they're simply collections of existing users. To assign permission for a resource to lots of users at the same time, you can create a new group and grant specific users membership to that group. You then assign permission for the resource to the group, instead of each individual user. This makes administration easier and more streamlined.

 OK, let's talk about files and directories. These are the resources we care about granting and protecting access to.

 Most Linux file systems (EXT4, XFS and ZFS for example) allow you to apply 3 primary permissions to files and directories. These permissions are:

* **Read:** Allow a file to be read (or list contents inside a directory)
* **Write:** Allow a file to be written to or modified (or create files and subdirectories _inside_ a directory)
* **Execute:** Allow to run a program or script (or enter into a directory, for example with the [cd command](https://audio-shaping.techidaily.com/updated-decoding-vimeos-video-dimensions-a-complete-perspective-on-aspect-ratios-for-2024/))

 All files and directories on a file system have standard permission assigned to 3 distinct entities: the user who owns it, the group owner and all other users. Each entity may have a combination of read, write and execute (r/w/x) permissions assigned. You can [use the ls command](https://extra-tips.techidaily.com/in-2024-capturecraft-hd-top-10-freepaid-filters-list/) to look at all of this info:

ls -l mysupersecretfile.txt

![A terminal window showing standard file permissions of a sample file on Linux.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/2-1.png) 

1. \[U\]ser (owner) permissions
2. \[G\]roup permissions
3. All \[O\]ther users' permissions
4. Owning username
5. Owning group name

 By default, each newly created user is also assigned to a new primary group of the same name. In the example above, #4 is the username "user" and #5 is the group name "user". Keep that in mind when looking at output such as this as it may be confusing at first.

 The files and directories that users are allowed to modify depend on a couple of things, including whether the user "owns" it or if they otherwise have the appropriate permissions to via a group membership. Note that the [root user](https://digital-screen-recording.techidaily.com/updated-2024-approved-entrance-video-analysis-review/) can modify any file on the system, regardless of ownership.

 This approach to file system permissions works well for most at-home and standalone setups. Of course, when you're working with systems where multiple users are accessing the same file hierarchy, and you must give certain people access to some areas (and restrict them from others), you'll start to understand the standard "1 owner, 1 group" methodology falls a bit short.

###  How ACLs Enhance the Standard Permissions Model

 Access Control Lists add the ability to apply permission entries to multiple users and groups for files and directories. One example where ACLs are a good option is when you want to assign a certain user permission to a file that already has specific owner and group owner permissions assigned.

 ACLs for directories follow the standard permissions **r**/**w**/**x** model in that they give you the ability to (**r**)ead (list contents, but not enter) the directory, (**w**)rite (create) new files and directories _inside_ the directory, and e(**x**)ecute (enter) the directory.

 How about an example? Let's say you have a file, report.pdf, owned by a user, peter, with read+write permissions. You've additionally granted group ownership of this file to the accounting group. Now you've received a request to grant read access to the user named lumberg.

 Let's assume you're using the standard permissions model. Here are a few (futile) ideas for completing this request:

* You can't grant lumberg membership to the accounting group (that would give him access to all sorts of other files he shouldn't be looking at).
* You also don't want to, as a matter of proper administrative practice, create a whole new group with users from the accounting group plus lumberg, just for this file.
* You _especially_ don't want to open up permissions to all other users, for obvious security reasons.

ls -l report.pdf

![A terminal window showing file listing output on Debian.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/3-2.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2049363/7443" target="_top" id="2049363">
  <img src="//a.impactradius-go.com/display-ad/7443-2049363" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2049363/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 What to do? Well, you _could_ just take an early lunch break. However, let's instead employ ACLs!

<!-- affiliate ads begin -->
<span id="1265663">
					<video width="240" height="200" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1265663.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/4482-1265663">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1265663.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:150px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fmartinic.evyy.net%2Fc%2F5597632%2F1265663%2F4482'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1265663/4482" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Checking for ACL Support on Your System

 Most modern Linux distributions support ACLs out-of-the-box. Most common file systems support them, their default mount options include ACL support and default installations should include the proper packages.

 To verify on ext2/3/4 file systems, use tune2fs. For example, if you want to check /dev/sda1 (which contains an ext4 file system):

sudo tune2fs -l /dev/sda1 | grep "Default mount options"

![A terminal window showing output of tune2fs command, and acl default mount option circled.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/4-1.png) 

 For reference, here's a [list of different file system support for ACLs, grouped by platform, written by IBM](https://www.ibm.com/docs/en/storage-protect/8.1.21?topic=linux-file-system-acl-support).

##  The getfacl Command

 The getfacl command displays (gets) file access control lists for files and directories. If you run getfacl on our report file from above, you'll see:

getfacl report.pdf

![A terminal window showing getfacl command and its output on a file.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/6.png) 

 Right now the output shows the _minimum ACL_ of the file. The minimum ACL comprises the standard permissions for the owner, owning group and all other users.

 If there were an _extended ACL_ entry for another user, let's call them michael, we'd see this:

getfacl report.pdf

![A terminal window showing getfacl command and its output.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/8.png) 

<!-- affiliate ads begin -->
<span id="1977004">
					<video width="128" height="480" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1977004.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/22993-1977004">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1977004.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:80px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fhomestyler.sjv.io%2Fc%2F5597632%2F1977004%2F22993'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1977004/22993" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 In addition to the minimum ACLs, we now have an extended ACL entry for user michael (read+write permissions). If you list the file again with extended ACLs, you'll notice a plus (+) sign to the right of the "other users" permissions, indicating that extended ACL entries exist:

ls -l report.pdf

![A terminal window showing ls command output with ACL entry flag.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/9.png) 

##  The setfacl Command

 The setfacl command is what actually _sets_ ACLs for files and directories. It adds and removes user and group entries, modifies permissions and other tasks like setting default ACLs on directories and working with masks. We'll use it to complete the request above by granting the lumberg user read access to report.pdf.

 To add the new user ACL entry, you'll use setfacl with this syntax (which I'll break down below):

sudo setfacl -m u:lumberg:r report.pdf

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2037318/7443" target="_top" id="2037318">
  <img src="//a.impactradius-go.com/display-ad/7443-2037318" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2037318/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

## ![A terminal window showing the setfacl command modifying a file's ACL entry.](https://static0.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/7-1.png) 

* **\-m** means we're modifying an ACL entry for the file
* **u:** means it's a user we're adding, followed by a colon (:) separator (a **g:** adds a group and **o:** adds all other users' permissions)
* **lumberg:** is the username we're adding, followed by another colon separator
* **r** means we're adding read permissions (only) to the entry
* **report.pdf** is the name of the file we're adding the ACL entry to

 Now that this is set we can take a look, using getfacl, once again:

getfacl report.pdf

![A terminal window showing output of getfacl command on our sample file.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/10.png) 

 Do you spot our new entry?

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2135351/19272" target="_top" id="2135351">
  <img src="//a.impactradius-go.com/display-ad/19272-2135351" border="0" alt="https://techidaily.com" width="125" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135351/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Default ACLs

 Default ACLs only apply to directories (folders). When you set a default ACL on a directory, the entry you specify will automatically be applied to _every_ new file and directory within it, regardless of who creates them. It's sort of a catch-all, recursive approach which makes it pretty useful when you're planning your file system hierarchy.

 Let's make sure Lumberg will be able to read new files and enter new directories that are created under Accounting. We'll use the -d option for adding a _default ACL_:

sudo setfacl -d -m u:lumberg:rX Accounting

![A terminal window showing setfacl command to set permissions, then getfacl to show them.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/12.png) 

<!-- affiliate ads begin -->
<span id="1982485">
					<video width="576" height="240" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1982485.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/22993-1982485">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1982485.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:360px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fhomestyler.sjv.io%2Fc%2F5597632%2F1982485%2F22993'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1982485/22993" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 An upper-case **X** applies the execute permission only against new subdirectories; not files.

 Access control lists are great for when you want to take your file system permissions to the next level. You can get away with a lot with standard user/group/other permissions, but there will likely be a point in your journeys where using ACLs makes much more sense.

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
<li><a href="https://fox-cloud.techidaily.com/new-diving-into-drones-syma-x5c-review-beginners-dream-uav-for-2024/"><u>[New] Diving Into Drones? Syma X5C Review Beginner's Dream UAV for 2024</u></a></li>
<li><a href="https://fox-links.techidaily.com/updated-2024-approved-best-subtitle-converters-win-and-mac-edition-leading-8-sbt-to-srtr-tools/"><u>[Updated] 2024 Approved Best Subtitle Converters Win & Mac Edition, Leading 8 SBT to SRTR Tools</u></a></li>
<li><a href="https://article-files.techidaily.com/updated-ideal-6-networks-for-thriving-business-ventures/"><u>[Updated] Ideal 6 Networks for Thriving Business Ventures</u></a></li>
<li><a href="https://video-screen-grab.techidaily.com/updated-in-2024-a-detailed-review-of-camstudio-screencapture/"><u>[Updated] In 2024, A Detailed Review of CamStudio ScreenCapture</u></a></li>
<li><a href="https://some-techniques.techidaily.com/cookiebot-enhanced-personalization-for-optimized-user-experience/"><u>Cookiebot-Enhanced Personalization for Optimized User Experience</u></a></li>
<li><a href="https://some-techniques.techidaily.com/cookiebot-fueled-success-boost-your-websites-traffic-with-proven-automation-tools/"><u>Cookiebot-Fueled Success: Boost Your Website's Traffic with Proven Automation Tools</u></a></li>
<li><a href="https://some-techniques.techidaily.com/cookiebot-the-cutting-edge-solution-for-seamless-marketing-automation-and-analytics/"><u>Cookiebot: The Cutting-Edge Solution for Seamless Marketing Automation and Analytics</u></a></li>
<li><a href="https://some-techniques.techidaily.com/customized-marketing-automation-with-leading-ai-technology/"><u>Customized Marketing Automation with Leading AI Technology</u></a></li>
<li><a href="https://some-techniques.techidaily.com/effortless-conversion-of-pdfs-and-images-to-searchable-files-using-docscan-x-top-tier-mobile-ocr-technology/"><u>Effortless Conversion of PDFs & Images to Searchable Files Using DocScan X: Top-Tier Mobile OCR Technology</u></a></li>
<li><a href="https://review-topics.techidaily.com/how-to-upgrade-or-downgrade-iphone-14-pro-without-itunes-drfone-by-drfone-ios-system-repair-ios-system-repair/"><u>How To Upgrade or Downgrade iPhone 14 Pro Without iTunes? | Dr.fone</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/in-2024-catch-or-beat-sleeping-snorlax-on-pokemon-go-for-xiaomi-redmi-k70-pro-drfone-by-drfone-virtual-android/"><u>In 2024, Catch or Beat Sleeping Snorlax on Pokemon Go For Xiaomi Redmi K70 Pro | Dr.fone</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/in-2024-will-pokemon-go-ban-the-account-if-you-use-pgsharp-on-oppo-reno-8t-5g-drfone-by-drfone-virtual-android/"><u>In 2024, Will Pokémon Go Ban the Account if You Use PGSharp On Oppo Reno 8T 5G | Dr.fone</u></a></li>
<li><a href="https://win-howtos.techidaily.com/1723211676541-razer-keyboard-not-glowing-common-issues-and-fixes-discovered/"><u>Razer Keyboard Not Glowing: Common Issues and Fixes Discovered</u></a></li>
<li><a href="https://youtube-videos.techidaily.com/unveiling-the-seven-best-youtube-live-streaming-tools-for-iphoneandroid/"><u>Unveiling The Seven Best YouTube Live Streaming Tools for iPhone/Android</u></a></li>
</ul></div>

