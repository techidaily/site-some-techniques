---
title: "Mastering File Permissions in Linux: A Guide to SUID, SGID, and Sticky Bit Settings"
date: 2024-12-21T19:18:49.723Z
updated: 2024-12-24T21:56:43.146Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://thmb.techidaily.com/122b9bb2737079496d6a2d69ef766a3b3b8a091bd4f5906c27990e96a64caabf.jpg
---

## Mastering File Permissions in Linux: A Guide to SUID, SGID, and Sticky Bit Settings

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/gOyLy8DeizY?si=GkAmK0hChZw6_2tW" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

### Quick Links

* [They're Already in Use](https://bypass-frp.techidaily.com/how-to-bypass-frp-from-honor-by-drfone-android/)
* [Elevating Your Status](https://win-answers.techidaily.com/master-the-art-of-smooth-gameplay-strategies-for-tackling-fps-drops-on-a-computer-system/)
* [You're Elevating the Program's Status](https://youtube-video-recordings.techidaily.com/new-avoid-mainstream-underrated-movies-of-the-year/)
* [Linux Commands That Use SUID](https://fox-access.techidaily.com/in-2024-discover-11-secrets-of-windows-11/)
* [Setting the SUID Bit](https://facebook-videos.techidaily.com/new-in-2024-adeptly-attaining-youtube-like-features-download-fb-vids/)
* [The SGID Bit](https://youtube-stream.techidaily.com/mastering-freefire-the-30-best-tag-strategies-to-increase-views-for-2024/)
* [The Sticky Bit](https://bypass-frp.techidaily.com/in-2024-top-5-honor-x9b-bypass-frp-tools-for-pc-that-actually-work-by-drfone-android/)
* [Reminders](https://on-screen-recording.techidaily.com/in-2024-achieving-seamless-group-discussions-in-google-chat/)

 SUID, SGID, and Sticky Bits are powerful special permissions you can set for executables and directories on Linux. We'll share the benefits—and potential pitfalls—of using them.

##  They're Already in Use

 Building security into a multiuser operating system presents several quandaries. Take the (seemingly) basic concept of passwords, for example. They all have to be stored so each time someone logs in, the system can compare the password he types to the stored copy. Obviously, as passwords are the keys to the kingdom, they must be safeguarded.

 On Linux, stored passwords are protected in two ways: they're encrypted, and only someone with `root` privileges can access the file that contains the passwords. That might sound fine, but it presents a quandary: If only people with `root` privileges can access stored passwords, how do those who don't have that access change their passwords?

##  Elevating Your Status

 Usually, Linux commands and programs run with the same set of permissions as the person who launches the program. When `root` runs the passwd command [to change a password](http://man7.org/linux/man-pages/man1/passwd.1.html), it runs with `root`’s permissions. That means the passwd command can freely access the stored passwords in the /etc/shadow file.

 What would be ideal is a scheme in which anyone on the system could launch the passwd program, but have the passwd program retain `root`’s elevated privileges. This would empower anyone to change her own password.

 The above scenario is precisely what the Set User ID bit (`SUID`) does. It runs programs and commands with the permissions of the file owner, rather than the permissions of the person who launches the program.

##  You're Elevating the Program's Status

 There is another quandary, though. The person has to be prevented from meddling with anyone else's password. Linux incorporates the `SUID` scheme which allows it to run applications with a set of temporarily borrowed permissions—but that's only half of the security story.

 The control mechanism that prevents someone from working with another person's password is contained within the passwd program, not the operating system and the SUID scheme.

 Programs that run with elevated privileges can pose security risks if they're not created with a "security by design" mindset. That means security is the first thing you consider, and then you build on that. Don’t write your program, and then try to give it a coat of security afterward.

 The biggest advantage of open source software is [you can look at the source code yourself](https://github.com/shadow-maint/shadow/blob/master/src/passwd.c) or refer to trusted peer-reviews of it. In the source code for the `passwd` program, there are checks, so you can see whether the person running the program is `root`. Different capabilities are allowed if someone is `root` (or someone using `sudo`).

[This](https://github.com/shadow-maint/shadow/blob/master/src/passwd.c#L0759) is the code that detects whether someone is `root`.

![Source code snippet from passwd.c](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/02/0a.png) 

 The following is an example in which that's taken into account. Because `root` can change any password, the program doesn't have to bother with the checks it usually performs to see which passwords the person has permission change. So, for `root`, it [skips those checks and exits the checking function](https://github.com/shadow-maint/shadow/blob/master/src/passwd.c#L0397).

![Source code snippet from passwd.c](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/02/0b.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/Jng92DT1n_Y?si=EdMRoNAFi0Q6mP7G" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 With the core Linux commands and utilities, you can be confident they've got security baked into them and that the code has been reviewed many times. Of course, there's always the threat of as-yet-unknown exploits. However, patches or updates are quick to appear to counter any newly identified vulnerabilities.

 It's third-party software—especially any that isn't open-source—you need to be extremely careful about using `SUID` with. We're not saying don't do it, but, if you do, you want to make sure it won't expose your system to risk. You don't want to elevate the privileges of a program that isn't going to correctly self-govern itself and the person running it.

##  Linux Commands That Use SUID

 The following are a few of the Linux commands that use the SUID bit to give the command elevated privileges when run by a regular user:

ls -l /bin/su

ls -l /bin/ping

ls -l /bin/mount

ls -l /bin/umount

ls -l /usr/bin/passwd

![List of Linux commands that have their SUID bit set, in a terminal window](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/02/1-5.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/-Bov2KfWQ_Y?si=MnVczisgeJ-sGW2r" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Note the filenames are highlighted in red, which indicates the SUID bit is set.

 The permissions on a file or directory are usually represented by three groups of three characters: rwx. These stand for read, write and execute. If the letters are present, that permission has been granted. If a hyphen (`-`) instead of a letter is present, though, that permission hasn't been given.

 There are three groups of these permissions (from left to right): those for the owner of the file, for members of the file's group, and for others. When the `SUID` bit is set on a file, an "s" represents the owner's execute permission.

 If the `SUID` bit is set on a file that doesn't have executable capabilities, an uppercase "S" denotes this.

 We'll take a look at an example. Regular user dave types the **passwd** command:

passwd

![passwd command in a terminal window](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/02/2-4.png) 

 The `passwd` command prompts `dave` for his new password. We can use the `ps` command [to see the details of running processes](http://man7.org/linux/man-pages/man1/ps.1.html).

 We'll use `ps` with `grep` [in a different terminal window](http://man7.org/linux/man-pages/man1/grep.1.html) and look for the `passwd` process. We'll also use the -e (every process) and -f (full-format) options with `ps`.

 We type the following command:

ps -e -f | grep passwd

![ps -e -f | grep passwd in a terminal window](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/02/3-7.png) 

 Two lines are reported, the second of which is the `grep` process looking for commands with the string "passwd" in them. It's the first line that interests us, though, because that's the one for the `passwd` process `dave` launched.

 We can see the `passwd` process runs the same as it would if `root` had launched it.

##  Setting the SUID Bit

 It's easy to change the `SUID` bit with `[chmod](https://extra-guidance.techidaily.com/new-perfect-synchronization-enhancing-audio-visual-with-subtitles-in-wmp/)`. The `u+s` symbolic mode sets the `SUID` bit and the `u-s` symbolic mode clears the `SUID` bit.

 To illustrate some of the concepts of the SUID bit, we created a small program called `htg`. It's in the root directory of the `dave` user, and it doesn't have the `SUID` bit set. When it's executed, it displays the real and effective user IDs ([UID](https://en.wikipedia.org/wiki/User%5Fidentifier)).

 The real [UID](https://en.wikipedia.org/wiki/User%5Fidentifier) belongs to the person who launched the program. The effective ID is the account the program is behaving as though it had been launched by.

 We type the following:

ls -lh htg

./htg

![ls -lh htg in a terminal window](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/02/4-3.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/iLlpdv0cz_k?si=HwTdnMmeVJXm4GPV" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 When we run the local copy of the program, we see the real and effective IDs are both set to `dave`. So, it's behaving just as a normal program should.

 Let's copy it to the `/usr/local/bin` directory so others can use it.

 We type the following, using `chmod` to set the `SUID` bit, and then check that it's been set:

sudo cp htg /usr/local/bin

sudo chmod u+s /usr/local/bin/htg

ls -hl /usr/local/bin/htg

![sudo cp htg /usr/local/bin in a terminal window](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/02/5-2.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/odDOPrPjRYY?si=7QHzdUkTPNkHJiVj" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 So, the program is copied, and the SUID bit is set. We'll run it again, but this time we'll run the copy in the `/usr/local/bin` folder:

htg

![The htg program running in a terminal window](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/02/6-3.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/5EKBEujWCw4?si=PwVvvervi8OrYaEA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Even though `dave` launched the program, the effective ID is set to the `root` user. So, if `mary` launches the program, the same thing happens, as shown below:

htg

![htg launched by user mary in a terminal window](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/02/9-2.png) 

 The real ID is `mary`, and the effective ID is `root`. The program runs with the permissions of the root user.

##  The SGID Bit

 The Set Group ID (`SGID`) bit is very similar to the `SUID` bit. When the `SGID` bit is set on an executable file, the effective group is set to the group of the file. The process runs with the permissions of the members of the file's group, rather than the permissions of the person who launched it.

 We tweaked our `htg` program so it shows the effective group, too. We'll change the group of the `htg` program to be user `mary`'s default group, `mary`. We'll also use the `u-s` and `g+s` symbolic modes with `[chown](https://tech-recovery.techidaily.com/cant-remove-printer-on-windows-solved/)` to remove the `SUID` bit and set the `SGID`.

 To do so, we type the following:

sudo chown root:mary /usr/local/bin/htg

sudo chmod u-s,g+s /usr/local/bin/htg

ls -lh /usr/local/bin/htg

![sudo chown root:mary /usr/local/bin/htg in a terminal window](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/02/10-2.png) 

 You can see the `SGID` bit denoted by the "s" in the group permissions. Also, note the group is set to `mary` and the file name is now highlighted in yellow.

 Before we run the program, let's establish which groups `dave` and `mary` belong to. We'll use the `id` command with the -G (groups) option, [to print all group IDs](http://man7.org/linux/man-pages/man1/id.1.html). Then, we'll run the `htg` program as `dave`.

 We type the following commands:

id -G dave

id -G mary

htg

![id -G dave in a terminal window](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/02/15-2.png) 

 The ID of the default group for `mary` is 1001, and the effective group of the `htg` program is 1001\. So, although it was launched by `dave`, it's running with the permissions of the members in the `mary` group. It's the same as if `dave` had joined the `mary` group.

 Let's apply the `SGID` bit to a directory. First, we'll create a directory called "work," and then change its group to "geek." We'll then set the `SGID` bit on the directory.

 When we use `ls` to check the settings of the directory, we'll also use the `-d` (directory) option so we see the details of the directory, not its contents.

 We type the following commands:

sudo mkdir work

sudo chown dave:geek work

sudo chmod g+s work

ls -lh -d work

![sudo mkdir work in a terminal window](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/02/12-3.png) 

 The `SGID` bit and "geek" group are set. These will affect any items created within the `work` directory.

 We type the following to enter the `work` directory, create a directory called "demo," and check its properties:

cd work

mkdir demo

ls -lh -d demo

![cd work in a terminal window](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/02/13-1.png) 

 The `SGID` bit and "geek" group are automatically applied to the "demo" directory.

 Let's type the following to create a file with the [touch command](http://man7.org/linux/man-pages/man1/touch.1.html) and check its properties:

touch useful.sh

ls -lh useful.sh

![touch useful.sh in a terminal window](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/02/14-3.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/jf0JvOqiAXc?si=kHEHQGC_PhBv4xij" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 The group of the new file is automatically set to "geek."

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/15Ju8Cb4UZ8?si=5wdiQXdz1BOxIkDH" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

##  The Sticky Bit

 The sticky bit gets its name from its historical purpose. When set on an executable, it flagged to the operating system that the text portions of the executable should be held in [swap](https://youtube-web.techidaily.com/ed-scale-up-channel-followers-faster-and-cheaper-for-2024/), making their re-use faster. On Linux, the sticky bit only affects a directory—setting it on a file wouldn't make sense.

 When you set the sticky bit on a directory, people can only delete files that belong to them within that directory. They can't delete files that belong to someone else, no matter which combination of file permissions are set on the files.

 This allows you to create a directory that everyone—and the processes they launch—can use as shared file storage. The files are protected because, again, no one can delete anyone else's files.

 Let's create a directory called "shared." We'll use the `o+t` symbolic mode with `chmod` to set the sticky bit on that directory. We'll then look at the permissions on that directory, as well as the `/tmp` and `/var/tmp` directories.

 We type the following commands:

mkdir shared

sudo chmod o+t shared

ls -lh -d shared

ls -lh -d /tmp

ls -lh -d /var/tmp

![mkdir shared in a terminal window](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/02/16-3.png) 

 If the sticky bit is set, the executable bit of the "other" set of file permissions is set to "t." The file name is also highlighted in blue.

 The `/tmp` and `/var/tmp` folders are two examples of directories that have all the file permissions set for the owner, group, and others (that's why they're highlighted in green). They're used as shared locations for temporary files.

 With those permissions, anyone should, theoretically, be able to do anything. However, the sticky bit overrides them, and no one can delete a file that doesn't belong to him.

##  Reminders

 The following is a quick checklist of what we covered above for future reference:

* `SUID` only works on files.
* You can apply `SGID` to directories and files.
* You can only apply the sticky bit to directories.
* If the "`s`", "`g`", or "`t`" indicators appear in uppercase, the executable bit (`x`) hasn't been set.

 Keep those points in mind and you're well on your way.

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
<li><a href="https://tiktok-videos.techidaily.com/new-2024-approved-quick-and-reliable-tiktok-to-mp4-file-transfer-software/"><u>[New] 2024 Approved Quick and Reliable TikTok to MP4 File Transfer Software</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-exploring-the-huawei-p10s-user-interface-and-usability/"><u>[New] Exploring the Huawei P10's User Interface & Usability</u></a></li>
<li><a href="https://article-tips.techidaily.com/updated-mastering-android-streaming-virtual-reality-content-for-2024/"><u>[Updated] Mastering Android Streaming Virtual Reality Content for 2024</u></a></li>
<li><a href="https://fox-cloud.techidaily.com/updated-stable-vr-experience-8-ways-to-prevent-nausea-for-2024/"><u>[Updated] Stable VR Experience 8 Ways to Prevent Nausea for 2024</u></a></li>
<li><a href="https://youtube-lab.techidaily.com/approved-discover-the-art-of-youtube-playlist-shuffling/"><u>2024 Approved Discover the Art of YouTube Playlist Shuffling</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-iconic-discussions-in-history-top-10-on-reddit/"><u>2024 Approved Iconic Discussions in History - Top 10 on Reddit</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-immersive-commerce-environments-design/"><u>2024 Approved Immersive Commerce Environments Design</u></a></li>
<li><a href="https://extra-resources.techidaily.com/deciphering-how-burst-improves-video-continuity/"><u>Deciphering How Burst Improves Video Continuity</u></a></li>
<li><a href="https://fox-access.techidaily.com/explore-visionary-typography-the-ultimate-list-of-9-websites-offering-intricate-3d-letters-for-2024/"><u>Explore Visionary Typography The Ultimate List of 9 Websites Offering Intricate 3D Letters for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/grandest-directors-reveals-for-2024/"><u>Grandest Directors' Reveals for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/illuminate-iphone-clips-simple-solutions-to-lighten-video-for-2024/"><u>Illuminate iPhone Clips Simple Solutions to Lighten Video for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-gear-vr-compatibility-the-definitive-mobile-device-list-2023-edition/"><u>In 2024, Gear VR Compatibility The Definitive Mobile Device List - 2023 Edition</u></a></li>
<li><a href="https://some-skills.techidaily.com/in-2024-the-ultimate-zeo-startup-showcase/"><u>In 2024, The Ultimate Zeo-Startup Showcase</u></a></li>
<li><a href="https://win-hacks.techidaily.com/missing-page-error-file-not-retrieved-code-404/"><u>Missing Page Error – File Not Retrieved (Code #404)</u></a></li>
<li><a href="https://ai-video-tools.techidaily.com/updated-get-started-with-linux-on-your-chromebook-a-comprehensive-installation-guide-for-2024/"><u>Updated Get Started with Linux on Your Chromebook A Comprehensive Installation Guide for 2024</u></a></li>
</ul></div>

