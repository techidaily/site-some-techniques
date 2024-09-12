---
title: "Mastering File Permissions in Linux: A Guide to SUID, SGID, and Sticky Bit Settings"
date: 2024-09-11T20:16:26.935Z
updated: 2024-09-12T20:16:26.935Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://thmb.techidaily.com/122b9bb2737079496d6a2d69ef766a3b3b8a091bd4f5906c27990e96a64caabf.jpg
---

## Mastering File Permissions in Linux: A Guide to SUID, SGID, and Sticky Bit Settings

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

<!-- affiliate ads begin -->
<span id="1977006">
					<video width="128" height="480" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1977006.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/22993-1977006">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1977006.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:80px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fhomestyler.sjv.io%2Fc%2F5597632%2F1977006%2F22993'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1977006/22993" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Elevating Your Status

 Usually, Linux commands and programs run with the same set of permissions as the person who launches the program. When `root` runs the passwd command [to change a password](http://man7.org/linux/man-pages/man1/passwd.1.html), it runs with `root`’s permissions. That means the passwd command can freely access the stored passwords in the /etc/shadow file.

 What would be ideal is a scheme in which anyone on the system could launch the passwd program, but have the passwd program retain `root`’s elevated privileges. This would empower anyone to change her own password.

 The above scenario is precisely what the Set User ID bit (`SUID`) does. It runs programs and commands with the permissions of the file owner, rather than the permissions of the person who launches the program.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2115910/19272" target="_top" id="2115910">
  <img src="//a.impactradius-go.com/display-ad/19272-2115910" border="0" alt="https://techidaily.com" width="120" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2115910/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  You're Elevating the Program's Status

 There is another quandary, though. The person has to be prevented from meddling with anyone else's password. Linux incorporates the `SUID` scheme which allows it to run applications with a set of temporarily borrowed permissions—but that's only half of the security story.

 The control mechanism that prevents someone from working with another person's password is contained within the passwd program, not the operating system and the SUID scheme.

 Programs that run with elevated privileges can pose security risks if they're not created with a "security by design" mindset. That means security is the first thing you consider, and then you build on that. Don’t write your program, and then try to give it a coat of security afterward.

 The biggest advantage of open source software is [you can look at the source code yourself](https://github.com/shadow-maint/shadow/blob/master/src/passwd.c) or refer to trusted peer-reviews of it. In the source code for the `passwd` program, there are checks, so you can see whether the person running the program is `root`. Different capabilities are allowed if someone is `root` (or someone using `sudo`).

[This](https://github.com/shadow-maint/shadow/blob/master/src/passwd.c#L0759) is the code that detects whether someone is `root`.

![Source code snippet from passwd.c](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/02/0a.png) 

 The following is an example in which that's taken into account. Because `root` can change any password, the program doesn't have to bother with the checks it usually performs to see which passwords the person has permission change. So, for `root`, it [skips those checks and exits the checking function](https://github.com/shadow-maint/shadow/blob/master/src/passwd.c#L0397).

![Source code snippet from passwd.c](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/02/0b.png) 

 With the core Linux commands and utilities, you can be confident they've got security baked into them and that the code has been reviewed many times. Of course, there's always the threat of as-yet-unknown exploits. However, patches or updates are quick to appear to counter any newly identified vulnerabilities.

 It's third-party software—especially any that isn't open-source—you need to be extremely careful about using `SUID` with. We're not saying don't do it, but, if you do, you want to make sure it won't expose your system to risk. You don't want to elevate the privileges of a program that isn't going to correctly self-govern itself and the person running it.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2115938/19272" target="_top" id="2115938">
  <img src="//a.impactradius-go.com/display-ad/19272-2115938" border="0" alt="https://techidaily.com" width="120" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2115938/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Linux Commands That Use SUID

 The following are a few of the Linux commands that use the SUID bit to give the command elevated privileges when run by a regular user:

ls -l /bin/su

ls -l /bin/ping

ls -l /bin/mount

ls -l /bin/umount

ls -l /usr/bin/passwd

![List of Linux commands that have their SUID bit set, in a terminal window](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/02/1-5.png) 

 Note the filenames are highlighted in red, which indicates the SUID bit is set.

 The permissions on a file or directory are usually represented by three groups of three characters: rwx. These stand for read, write and execute. If the letters are present, that permission has been granted. If a hyphen (`-`) instead of a letter is present, though, that permission hasn't been given.

 There are three groups of these permissions (from left to right): those for the owner of the file, for members of the file's group, and for others. When the `SUID` bit is set on a file, an "s" represents the owner's execute permission.

 If the `SUID` bit is set on a file that doesn't have executable capabilities, an uppercase "S" denotes this.

 We'll take a look at an example. Regular user dave types the **passwd** command:

passwd

![passwd command in a terminal window](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/02/2-4.png) 

<!-- affiliate ads begin -->
<a href="https://review-au.sjv.io/c/5597632/2098701/14409" target="_top" id="2098701">
  <img src="//a.impactradius-go.com/display-ad/14409-2098701" border="0" alt="https://techidaily.com" width="120" height="90"/>
</a>
<img height="0" width="0" src="https://review-au.sjv.io/i/5597632/2098701/14409" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 The `passwd` command prompts `dave` for his new password. We can use the `ps` command [to see the details of running processes](http://man7.org/linux/man-pages/man1/ps.1.html).

 We'll use `ps` with `grep` [in a different terminal window](http://man7.org/linux/man-pages/man1/grep.1.html) and look for the `passwd` process. We'll also use the -e (every process) and -f (full-format) options with `ps`.

 We type the following command:

ps -e -f | grep passwd

![ps -e -f | grep passwd in a terminal window](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/02/3-7.png) 

<!-- affiliate ads begin -->
<a href="https://review-au.sjv.io/c/5597632/2098704/14409" target="_top" id="2098704">
  <img src="//a.impactradius-go.com/display-ad/14409-2098704" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://review-au.sjv.io/i/5597632/2098704/14409" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Two lines are reported, the second of which is the `grep` process looking for commands with the string "passwd" in them. It's the first line that interests us, though, because that's the one for the `passwd` process `dave` launched.

 We can see the `passwd` process runs the same as it would if `root` had launched it.

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

##  Setting the SUID Bit

 It's easy to change the `SUID` bit with `[chmod](https://extra-guidance.techidaily.com/new-perfect-synchronization-enhancing-audio-visual-with-subtitles-in-wmp/)`. The `u+s` symbolic mode sets the `SUID` bit and the `u-s` symbolic mode clears the `SUID` bit.

 To illustrate some of the concepts of the SUID bit, we created a small program called `htg`. It's in the root directory of the `dave` user, and it doesn't have the `SUID` bit set. When it's executed, it displays the real and effective user IDs ([UID](https://en.wikipedia.org/wiki/User%5Fidentifier)).

 The real [UID](https://en.wikipedia.org/wiki/User%5Fidentifier) belongs to the person who launched the program. The effective ID is the account the program is behaving as though it had been launched by.

 We type the following:

ls -lh htg

./htg

![ls -lh htg in a terminal window](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/02/4-3.png) 

<!-- affiliate ads begin -->
<span id="1542129">
					<video width="864" height="1152" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1542129.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/16836-1542129">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1542129.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:540px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2F25home.pxf.io%2Fc%2F5597632%2F1542129%2F16836'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1542129/16836" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 When we run the local copy of the program, we see the real and effective IDs are both set to `dave`. So, it's behaving just as a normal program should.

 Let's copy it to the `/usr/local/bin` directory so others can use it.

 We type the following, using `chmod` to set the `SUID` bit, and then check that it's been set:

sudo cp htg /usr/local/bin

sudo chmod u+s /usr/local/bin/htg

ls -hl /usr/local/bin/htg

![sudo cp htg /usr/local/bin in a terminal window](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/02/5-2.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2115913/19272" target="_top" id="2115913">
  <img src="//a.impactradius-go.com/display-ad/19272-2115913" border="0" alt="https://techidaily.com" width="180" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2115913/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 So, the program is copied, and the SUID bit is set. We'll run it again, but this time we'll run the copy in the `/usr/local/bin` folder:

htg

![The htg program running in a terminal window](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/02/6-3.png) 

 Even though `dave` launched the program, the effective ID is set to the `root` user. So, if `mary` launches the program, the same thing happens, as shown below:

htg

![htg launched by user mary in a terminal window](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2020/02/9-2.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2115927/19272" target="_top" id="2115927">
  <img src="//a.impactradius-go.com/display-ad/19272-2115927" border="0" alt="https://techidaily.com" width="125" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2115927/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 The real ID is `mary`, and the effective ID is `root`. The program runs with the permissions of the root user.

<!-- affiliate ads begin -->
<span id="1982462">
					<video width="576" height="240" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1982462.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/22993-1982462">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1982462.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:360px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fhomestyler.sjv.io%2Fc%2F5597632%2F1982462%2F22993'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1982462/22993" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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

 The group of the new file is automatically set to "geek."

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
<li><a href="https://facebook-video-footage.techidaily.com/new-2024-approved-beyond-mainstream-a-list-of-6-exclusive-icon-and-logo-providers/"><u>[New] 2024 Approved Beyond Mainstream A List of 6 Exclusive Icon & Logo Providers</u></a></li>
<li><a href="https://facebook-video-share.techidaily.com/updated-expertise-in-film-perfecting-the-art-of-chroma-key/"><u>[Updated] Expertise in Film Perfecting the Art of Chroma Key</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/updated-in-2024-navigating-noise-free-networks-secrets-for-silencing-disruptions-on-gomeet/"><u>[Updated] In 2024, Navigating Noise-Free Networks Secrets for Silencing Disruptions on GoMeet</u></a></li>
<li><a href="https://on-screen-recording.techidaily.com/updated-in-2024-the-ultimate-playbook-for-professional-level-xbox-recording/"><u>[Updated] In 2024, The Ultimate Playbook for Professional-Level Xbox Recording</u></a></li>
<li><a href="https://fox-that.techidaily.com/bypass-airdrop-glitches-expert-advice-on-quick-fixes-with-16-effective-solutions/"><u>Bypass AirDrop Glitches: Expert Advice on Quick Fixes with 16 Effective Solutions</u></a></li>
<li><a href="https://techtrends.techidaily.com/diy-tips-for-banishing-subwoofer-vibrations-and-noise/"><u>DIY Tips for Banishing Subwoofer Vibrations and Noise</u></a></li>
<li><a href="https://some-techniques.techidaily.com/effortless-guide-projecting-your-maciphoneipad-display-onto-an-apple-tv/"><u>Effortless Guide: Projecting Your Mac/iPhone/iPad Display Onto an Apple TV</u></a></li>
<li><a href="https://some-techniques.techidaily.com/elevating-your-drive-top-6-upgrades-needed-in-the-next-android-auto-update/"><u>Elevating Your Drive: Top 6 Upgrades Needed in the Next Android Auto Update</u></a></li>
<li><a href="https://some-techniques.techidaily.com/enhancing-googles-core-functionality-over-emphasizing-artificial-intelligence/"><u>Enhancing Google's Core Functionality Over Emphasizing Artificial Intelligence</u></a></li>
<li><a href="https://extra-approaches.techidaily.com/step-by-step-process-for-making-a-stellar-podcast-launch-video-for-2024/"><u>Step-By-Step Process for Making a Stellar Podcast Launch Video for 2024</u></a></li>
<li><a href="https://win-answers.techidaily.com/troubleshooting-and-fixing-dev-error-5573-in-call-of-duty-vanguard/"><u>Troubleshooting and Fixing Dev Error 5573 in Call of Duty: Vanguard</u></a></li>
<li><a href="https://printer-issues.techidaily.com/unify-mf4770n-with-windows-environment-in-win11win87/"><u>Unify MF4770n with Windows Environment in Win11/Win8/7</u></a></li>
</ul></div>

