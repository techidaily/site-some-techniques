---
title: "Comprehensive Guide: Managing Access Rights Using Linux's Access Control Lists"
date: 2025-02-05T16:16:09.781Z
updated: 2025-02-09T18:58:54.409Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://thmb.techidaily.com/292b65daa58a3cb7189f78d0565b817f09110724b35903d3b3e9b8eb64f84eb9.jpg
---

## Comprehensive Guide: Managing Access Rights Using Linux's Access Control Lists

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/TJCye_oCTTw?si=6bVyBphcSgSFdyuq" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

### Key Takeaways

* To view all ACL entries for a file, use the command 'getfacl filename' but replace 'filename' with the name of your file.
* To set a new ACL entry for a file, use the command 'setfacl -m u:username:rwx filename'
* To set a Default ACL entry on a directory, use the command 'setfacl -d -m u:username:rwx dirname'

 Are you in charge of a shared file server between multiple groups of people, who all need varying access? In this tutorial we'll go over the basics of ACLs and employ them in a fictional office scenario.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/FLO5dwmJAVs?si=1OYH8rv8aPaMsCiU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  What Are ACLs?

 Access Control Lists (ACLs) supplement the [standard file system permissions model on Linux and Unix](https://os-tips.techidaily.com/how-to-reset-waze-location-memory-on-ios-devices-a-step-by-step-guide/). In a nutshell, they allow you to go beyond the "user/group/other" concept to create additional sets of permissions for files and directories. They also do neat things like automatically applying permissions to new files and directories. But first, let's cover some basic Linux file system permissions concepts in which ACLs work alongside.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/DCARjc5g5VI?si=9OfovbKBrpoJeXTY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/vFQCEZiYA08?si=xjIu5IAy77RlHWii" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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

 What to do? Well, you _could_ just take an early lunch break. However, let's instead employ ACLs!

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/nWu29cqFjZA?si=TNZyCbPq68PQ0JIb" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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

 In addition to the minimum ACLs, we now have an extended ACL entry for user michael (read+write permissions). If you list the file again with extended ACLs, you'll notice a plus (+) sign to the right of the "other users" permissions, indicating that extended ACL entries exist:

ls -l report.pdf

![A terminal window showing ls command output with ACL entry flag.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/9.png) 

##  The setfacl Command

 The setfacl command is what actually _sets_ ACLs for files and directories. It adds and removes user and group entries, modifies permissions and other tasks like setting default ACLs on directories and working with masks. We'll use it to complete the request above by granting the lumberg user read access to report.pdf.

 To add the new user ACL entry, you'll use setfacl with this syntax (which I'll break down below):

sudo setfacl -m u:lumberg:r report.pdf

## ![A terminal window showing the setfacl command modifying a file's ACL entry.](https://static0.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/7-1.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/poI1NQxHfjc?si=ZLG0wziYcTKIKwL5" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

* **\-m** means we're modifying an ACL entry for the file
* **u:** means it's a user we're adding, followed by a colon (:) separator (a **g:** adds a group and **o:** adds all other users' permissions)
* **lumberg:** is the username we're adding, followed by another colon separator
* **r** means we're adding read permissions (only) to the entry
* **report.pdf** is the name of the file we're adding the ACL entry to

 Now that this is set we can take a look, using getfacl, once again:

getfacl report.pdf

![A terminal window showing output of getfacl command on our sample file.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/10.png) 

 Do you spot our new entry?

##  Default ACLs

 Default ACLs only apply to directories (folders). When you set a default ACL on a directory, the entry you specify will automatically be applied to _every_ new file and directory within it, regardless of who creates them. It's sort of a catch-all, recursive approach which makes it pretty useful when you're planning your file system hierarchy.

 Let's make sure Lumberg will be able to read new files and enter new directories that are created under Accounting. We'll use the -d option for adding a _default ACL_:

sudo setfacl -d -m u:lumberg:rX Accounting

![A terminal window showing setfacl command to set permissions, then getfacl to show them.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/12.png) 

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
<li><a href="https://video-capture.techidaily.com/new-elevating-live-game-coverage-tips-and-tricks/"><u>[New] Elevating Live Game Coverage Tips and Tricks</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-exploring-the-dynamics-of-canon-timelapse-imagery/"><u>[New] Exploring the Dynamics of Canon Timelapse Imagery</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-eye-catchers-of-tomorrow-discovering-6-future-oriented-genres/"><u>[New] Eye Catchers of Tomorrow Discovering 6 Future-Oriented Genres</u></a></li>
<li><a href="https://fox-helps.techidaily.com/new-in-2024-capture-crop-and-color-correct-with-this-lists-top-5-android-apps/"><u>[New] In 2024, Capture, Crop, and Color-Correct with This List's Top 5 Android Apps</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-innovative-notetaking-for-mobile-photographers/"><u>[New] Innovative Notetaking for Mobile Photographers</u></a></li>
<li><a href="https://youtube-docs.techidaily.com/ed-crafting-success-in-youtubes-creator-hub/"><u>[Updated] Crafting Success in YouTube's Creator Hub</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-funflicks-full-evaluation-and-instructions-24/"><u>[Updated] FunFlicks Full Evaluation & Instructions '24</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-how-to-add-radial-blur-effect-to-photos-in-photoshop/"><u>[Updated] How to Add Radial Blur Effect to Photos in Photoshop</u></a></li>
<li><a href="https://some-techniques.techidaily.com/immerse-in-windows-11s-photo-quality-filter-options-and-music-playlists-for-2024/"><u>Immerse in Windows 11'S Photo Quality Filter Options and Music Playlists for 2024</u></a></li>
<li><a href="https://easy-unlock-android.techidaily.com/in-2024-forgot-pattern-lock-heres-how-you-can-unlock-oneplus-nord-n30-5g-pattern-lock-screen-by-drfone-android/"><u>In 2024, Forgot Pattern Lock? Heres How You Can Unlock OnePlus Nord N30 5G Pattern Lock Screen</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-hasty-steps-ios-photos-and-videos-on-windows/"><u>In 2024, Hasty Steps IOS Photos & Videos on Windows</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-ideal-illustration-tools-for-windows-no-cost-high-prices/"><u>In 2024, Ideal Illustration Tools for Windows No Cost, High Prices</u></a></li>
<li><a href="https://fox-blue.techidaily.com/in-2024-navigating-win11-like-a-pro-your-guidebook/"><u>In 2024, Navigating Win11 Like a Pro - Your Guidebook</u></a></li>
<li><a href="https://facebook-video-content.techidaily.com/iphoneandroid-integrating-playlists-into-your-fb-music/"><u>IPhone/Android Integrating Playlists Into Your FB Music</u></a></li>
<li><a href="https://novels-ebooks.techidaily.com/2550560-9781937006501-moments-of-mindfulness/"><u>Moments of Mindfulness | Free Book</u></a></li>
<li><a href="https://extra-resources.techidaily.com/speed-enhancement-tips-for-periscope-livestimation/"><u>Speed Enhancement Tips for Periscope Livestimation</u></a></li>
<li><a href="https://youtube-data.techidaily.com/1-economical-cameras-for-professional-vloggers-for-2024/"><u>Top 11 Economical Cameras for Professional Vloggers for 2024</u></a></li>
</ul></div>

