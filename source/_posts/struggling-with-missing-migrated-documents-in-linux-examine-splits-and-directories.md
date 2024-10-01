---
title: Struggling with Missing Migrated Documents in Linux? Examine Splits and Directories!
date: 2024-09-30T04:00:49.698Z
updated: 2024-09-30T18:01:53.763Z
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

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2049382/7443" target="_top" id="2049382">
  <img src="//a.impactradius-go.com/display-ad/7443-2049382" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2049382/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  How This Particular Problem Foxes People

 Moving a file on the [command line is pretty simple](https://buynow-help.techidaily.com/misinterpretation-of-gram-staining-results-can-lead-to-incorrect-identification-affecting-treatment-decisions-in-clinical-settings/). You specify the file you want to move, and where you want to move it to. But still, it’s easy for a new user to find themselves exasperated and frustrated over mv.

 They try to move a file into a directory, and it seems to work. They don’t get a confirmation message, but neither do they get an error message. Linux often takes the no news is good news approach. If you don’t get an error message, it must have worked.

 Or did it? When they cd into the target directory, the file isn’t there. And of course, because mv moves the file from the original directory, it’s not there either. It’s starting to look like the file has been lost in the ether. This is usually the point where the frustrated user reaches out for help.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1938677/19272" target="_top" id="1938677">
  <img src="//a.impactradius-go.com/display-ad/19272-1938677" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1938677/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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
<a href="https://bluettius.sjv.io/c/5597632/2139113/17108" target="_top" id="2139113">
  <img src="//a.impactradius-go.com/display-ad/17108-2139113" border="0" alt="https://techidaily.com" width="320" height="90"/>
</a>
<img height="0" width="0" src="https://bluettius.sjv.io/i/5597632/2139113/17108" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 That’s nice and simple, and everything works as expected. If we look into our target directory, we find the moved file, and we get on with the rest of our work.

![A moved file in its new directory.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/2-4.png) 

 But let's say our Linux newcomer isn’t using [tab completion](https://desktop-recording.techidaily.com/new-2024-approved-an-impartial-appraisal-the-power-of-recordcast/). They're typing the directory paths by hand. If they misspell the name of the final directory, we get a very different behavior.

mv ~/Downloads/src/important-file.dat ~/Documents/backpu

![Trying to use the mv command with a typo in the final directory name.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/3-3.png) 

 They’ve made a typo with the target directory name, but mv exits silently back to the command prompt. On the face of it, it looks like the file move worked.

 Let’s check.

        `ls ~/Downloads/src  
ls ~/Documents/backup/  
`
    
![Using ls to look for the file in the original and new directories.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/4-2.png) 

<!-- affiliate ads begin -->
<a href="https://unicoeye.pxf.io/c/5597632/2134238/18498" target="_top" id="2134238">
  <img src="//a.impactradius-go.com/display-ad/18498-2134238" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://unicoeye.pxf.io/i/5597632/2134238/18498" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 The original and target directories are both empty. Where did the file go?

 Bash tries to find a directory called backpu, but can't find one. It concludes you want to rename your moved file to backpu. You’ll find a file called backpu one directory level higher than your target directory.

ls -l ~/Documents

![The location of the missing and misspelled file.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/5-2.png) 

 To fix this, you can move your file to where it should have gone, and specify its proper name on the command line.

        `mv ~/Documents/backpu ~/Documents/backup/important-file.dat   
ls ~/Documents/backup  
`
    
![Moving and renaming the misspelled file](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/6-2.png) 

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
<li><a href="https://screen-sharing-recording.techidaily.com/new-in-2024-digital-diary-top-picks-for-personal-video-devices/"><u>[New] In 2024, Digital Diary Top Picks for Personal Video Devices</u></a></li>
<li><a href="https://screen-recording.techidaily.com/new-in-2024-the-complete-blueprint-to-record-hulu-playback/"><u>[New] In 2024, The Complete Blueprint to Record Hulu Playback</u></a></li>
<li><a href="https://facebook-video-share.techidaily.com/updated-best-youtube-beginnings-15-editing-samples-for-2024/"><u>[Updated] Best YouTube Beginnings 15 Editing Samples for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-exclusive-content-review-the-best-15-youtube-unboxers-of-2024/"><u>[Updated] Exclusive Content Review The Best 15 YouTube Unboxers of 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-go-pro-karma-drone-review/"><u>[Updated] Go Pro Karma Drone Review</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-hypervision-pro-all-in-one-4k-screen-desks/"><u>[Updated] HyperVision Pro All-in-One 4K Screen Desks</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-harmonizing-hues-audio-fade-techniques-in-logic-pro/"><u>2024 Approved Harmonizing Hues Audio Fade Techniques in Logic Pro</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/2024-approved-how-to-design-a-post-that-sparks-wide-scale-interest-in-fb-giving/"><u>2024 Approved How to Design a Post That Sparks Wide-Scale Interest in FB Giving</u></a></li>
<li><a href="https://some-techniques.techidaily.com/file-sync-up-the-5-fundamental-ways-for-your-computer-upload-for-2024/"><u>File Sync-Up The 5 Fundamental Ways for Your Computer Upload for 2024</u></a></li>
<li><a href="https://hardware-help.techidaily.com/1722967627564-get-your-free-windows-8-amd-radeon-graphics-software-update-now/"><u>Get Your Free Windows 8 AMD Radeon Graphics Software Update Now!</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-excellent-choices-comprehensive-paid-and-free-macpc-video-decoders/"><u>In 2024, Excellent Choices Comprehensive Paid & FREE Mac/PC Video Decoders</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-honoring-artistry-essential-stop-motion-movies-top-15/"><u>In 2024, Honoring Artistry Essential Stop-Motion Movies (Top 15)</u></a></li>
<li><a href="https://bypass-frp.techidaily.com/in-2024-how-to-bypass-google-frp-lock-on-honor-x7b-devices-by-drfone-android/"><u>In 2024, How to Bypass Google FRP Lock on Honor X7b Devices</u></a></li>
<li><a href="https://youtube-web.techidaily.com/24-secure-song-transfers-to-youtube-channel/"><u>In 2024, Secure Song Transfers to Youtube Channel</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/in-2024-thinking-about-changing-your-netflix-region-without-a-vpn-on-apple-iphone-11-pro-drfone-by-drfone-virtual-ios/"><u>In 2024, Thinking About Changing Your Netflix Region Without a VPN On Apple iPhone 11 Pro? | Dr.fone</u></a></li>
<li><a href="https://buynow-reviews.techidaily.com/redefining-power-efficiency-a-comprehensive-review-of-apples-revolutionary-arm-based-mac-mini/"><u>Redefining Power Efficiency: A Comprehensive Review of Apple's Revolutionary ARM-Based Mac Mini</u></a></li>
</ul></div>

