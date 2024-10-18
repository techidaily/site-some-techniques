---
title: Struggling with Missing Migrated Documents in Linux? Examine Splits and Directories!
date: 2024-10-15T20:20:50.931Z
updated: 2024-10-17T22:16:10.231Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/a-magnifying-glass-pointed-at-the-linux-mascot-next-to-a-file-folder.jpg
---

## Struggling with Missing Migrated Documents in Linux? Examine Splits and Directories!

### Quick Links

* [How This Particular Problem Foxes People](https://vimeo-videos.techidaily.com/2024-approved-discovering-vimeo-home-for-high-quality-films/)
* [The Part Slash Plays in the mv Command](https://youtube-help.techidaily.com/in-2024-optimized-video-engagement-with-peak-post-times/)
* [It’s Not Exactly Slash’s Fault](https://mondly-stories.techidaily.com/film-and-television-as-educational-resources/)

 Typically, mv is one of the first Linux commands you learn. But one little slip, and things can get surprisingly confusing for the user. Sometimes it looks like moved files have simply vanished.

##  How This Particular Problem Foxes People

 Moving a file on the [command line is pretty simple](https://buynow-help.techidaily.com/misinterpretation-of-gram-staining-results-can-lead-to-incorrect-identification-affecting-treatment-decisions-in-clinical-settings/). You specify the file you want to move, and where you want to move it to. But still, it’s easy for a new user to find themselves exasperated and frustrated over mv.

 They try to move a file into a directory, and it seems to work. They don’t get a confirmation message, but neither do they get an error message. Linux often takes the no news is good news approach. If you don’t get an error message, it must have worked.

 Or did it? When they cd into the target directory, the file isn’t there. And of course, because mv moves the file from the original directory, it’s not there either. It’s starting to look like the file has been lost in the ether. This is usually the point where the frustrated user reaches out for help.

##  The Part Slash Plays in the mv Command

 Let’s say you’re moving a file to a different directory. You’re going to keep the same filename. In theory, this makes things easy because you don’t need to specify a target filename on the command line. By default, mv uses the original filename.

 We’ve got a file in the \~/Downloads/src directory. We move it to the \~/Documents/backup directory. As expected, it’s now in the backup directory, and it has been removed from the src directory.

        `ls ~/Downloads/src  
mv ~/Downloads/src/important-file.dat ~/Documents/backup   
ls ~/Documents/backup/  
ls ~/Downloads/src  
`
    
![Moving a file with the mv command](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/1-4.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2135352/19272" target="_top" id="2135352">
  <img src="//a.impactradius-go.com/display-ad/19272-2135352" border="0" alt="https://techidaily.com" width="160" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135352/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 That’s nice and simple, and everything works as expected. If we look into our target directory, we find the moved file, and we get on with the rest of our work.

![A moved file in its new directory.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/2-4.png) 

 But let's say our Linux newcomer isn’t using [tab completion](https://desktop-recording.techidaily.com/new-2024-approved-an-impartial-appraisal-the-power-of-recordcast/). They're typing the directory paths by hand. If they misspell the name of the final directory, we get a very different behavior.

mv ~/Downloads/src/important-file.dat ~/Documents/backpu

![Trying to use the mv command with a typo in the final directory name.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/3-3.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1948881/19272" target="_top" id="1948881">
  <img src="//a.impactradius-go.com/display-ad/19272-1948881" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1948881/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 They’ve made a typo with the target directory name, but mv exits silently back to the command prompt. On the face of it, it looks like the file move worked.

 Let’s check.

        `ls ~/Downloads/src  
ls ~/Documents/backup/  
`
    
![Using ls to look for the file in the original and new directories.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/4-2.png) 

 The original and target directories are both empty. Where did the file go?

 Bash tries to find a directory called backpu, but can't find one. It concludes you want to rename your moved file to backpu. You’ll find a file called backpu one directory level higher than your target directory.

ls -l ~/Documents

![The location of the missing and misspelled file.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/5-2.png) 

<!-- affiliate ads begin -->
<a href="https://imp.i357552.net/c/5597632/1001446/11832" target="_top" id="1001446">
  <img src="//a.impactradius-go.com/display-ad/11832-1001446" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://imp.i357552.net/i/5597632/1001446/11832" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 To fix this, you can move your file to where it should have gone, and specify its proper name on the command line.

        `mv ~/Documents/backpu ~/Documents/backup/important-file.dat   
ls ~/Documents/backup  
`
    
![Moving and renaming the misspelled file](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/6-2.png) 

<!-- affiliate ads begin -->
<span id="1834906">
					<video width="864" height="864" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1834906.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/16836-1834906">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1834906.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:540px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2F25home.pxf.io%2Fc%2F5597632%2F1834906%2F16836'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1834906/16836" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 The confusion and the hunt for the missing, badly-named file could have been avoided by adding a trailing slash to the target directory on the command line. That way, if you make a typo, Bash reports an error.

mv ~/Downloads/src/important-file.dat ~/Documents/backpu/

![The trailing slash on the mv command line flags errors with the final directory name](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/7-2.png) 

 The trailing slash explicitly tells Bash that this is a directory name, not a filename. Because Bash can’t find the misspelled directory, it reports the error to you and doesn’t move anything.

 This is a better outcome for failures. You’re alerted to the error, and the original file remains touched.

 Using the Bash tab completion feature not only speeds up the entry of directory paths, it gives a few extra bonuses. All the directory names are automatically spelled correctly, and a trailing slash is added to the final directory.

##  It’s Not Exactly Slash’s Fault

 Slash didn’t make the typo, after all. But if slash is present and on duty, you're told about the error before mv does anything questionable with your file.

 As is often the case, a good diagnostic first step is to check the [command history](https://article-posts.techidaily.com/2024-approved-precision-techniques-shifting-bulk-video-data-from-iphone-to-mac/) and see what command was actually issued, not what you think you typed. If you spot a typo, look for a file with that misspelled name, one directory level higher than where you expect it to be.

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
<li><a href="https://some-techniques.techidaily.com/new-hubs-for-high-quality-vr-watching/"><u>[New] Hubs for High-Quality VR Watching</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-innovating-audio-visuals-podcast-covers-explained/"><u>[New] Innovating Audio Visuals Podcast Covers Explained</u></a></li>
<li><a href="https://facebook-video-footage.techidaily.com/updated-break-free-from-the-norms-crafting-your-own-streamer-identity-for-2024/"><u>[Updated] Break Free From The Norms Crafting Your Own Streamer Identity for 2024</u></a></li>
<li><a href="https://screen-recording.techidaily.com/updated-recording-made-simple-a-comprehensive-guide-to-archiving-roblox-games-on-your-macbook/"><u>[Updated] Recording Made Simple A Comprehensive Guide to Archiving Roblox Games on Your MacBook</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-expertly-handling-timecodes-in-srt-using-macos-tools/"><u>2024 Approved Expertly Handling Timecodes in SRT Using macOS Tools</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-flight-to-imagery-a-review-of-dji-sparks-miniature-drone-innovation/"><u>2024 Approved Flight to Imagery A Review of DJI Spark's Miniature Drone Innovation</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-incorporating-captions-in-photography-a-user-friendly-guide-on-pc-and-mac/"><u>2024 Approved Incorporating Captions in Photography A User-Friendly Guide on PC & Mac</u></a></li>
<li><a href="https://facebook-videos.techidaily.com/2024-approved-linkedin-image-aspect-ratios-explained/"><u>2024 Approved LinkedIn Image Aspect Ratios Explained</u></a></li>
<li><a href="https://win-answers.techidaily.com/1722984057600-how-to-overcome-crashes-in-disco-elysium-on-your-windows-computer-solutions-worked/"><u>How to Overcome Crashes in Disco Elysium on Your Windows Computer - Solutions Worked</u></a></li>
<li><a href="https://change-location.techidaily.com/how-to-teleport-your-gps-location-on-vivo-v27-pro-drfone-by-drfone-virtual-android/"><u>How To Teleport Your GPS Location On Vivo V27 Pro? | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/ideal-action-cameras-for-stabilized-shots-for-2024/"><u>Ideal Action Cameras for Stabilized Shots for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-exploring-the-sky-the-syma-x5c-for-drone-beginners/"><u>In 2024, Exploring the Sky The Syma X5C for Drone Beginners</u></a></li>
<li><a href="https://buynow-info.techidaily.com/is-spotify-on-track-to-discontinue-their-innovative-car-thing-feature/"><u>Is Spotify on Track to Discontinue Their Innovative 'Car Thing' Feature?</u></a></li>
<li><a href="https://some-approaches.techidaily.com/top-15-free-budget-friendly-web-photo-editors-2023-review-for-2024/"><u>Top 15 Free, Budget-Friendly Web Photo Editors - 2023 Review for 2024</u></a></li>
<li><a href="https://tech-revival.techidaily.com/unlock-secure-pdfs-expert-guide-to-bypassing-and-eliminating-pdf-passwords/"><u>Unlock Secure PDFs: Expert Guide to Bypassing & Eliminating PDF Passwords</u></a></li>
</ul></div>

