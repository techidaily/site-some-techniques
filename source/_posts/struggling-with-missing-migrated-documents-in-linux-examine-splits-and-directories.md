---
title: Struggling with Missing Migrated Documents in Linux? Examine Splits and Directories!
date: 2024-10-23T17:43:17.038Z
updated: 2024-10-29T17:23:48.729Z
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

 That’s nice and simple, and everything works as expected. If we look into our target directory, we find the moved file, and we get on with the rest of our work.

![A moved file in its new directory.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/2-4.png) 

 But let's say our Linux newcomer isn’t using [tab completion](https://desktop-recording.techidaily.com/new-2024-approved-an-impartial-appraisal-the-power-of-recordcast/). They're typing the directory paths by hand. If they misspell the name of the final directory, we get a very different behavior.

mv ~/Downloads/src/important-file.dat ~/Documents/backpu

![Trying to use the mv command with a typo in the final directory name.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/3-3.png) 

<!-- affiliate ads begin -->
<a href="https://laganoo.pxf.io/c/5597632/1484940/16446" target="_top" id="1484940">
  <img src="//a.impactradius-go.com/display-ad/16446-1484940" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://laganoo.pxf.io/i/5597632/1484940/16446" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 They’ve made a typo with the target directory name, but mv exits silently back to the command prompt. On the face of it, it looks like the file move worked.

 Let’s check.

        `ls ~/Downloads/src  
ls ~/Documents/backup/  
`
    
![Using ls to look for the file in the original and new directories.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/4-2.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2094482/7443" target="_top" id="2094482">
  <img src="//a.impactradius-go.com/display-ad/7443-2094482" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2094482/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 The original and target directories are both empty. Where did the file go?

 Bash tries to find a directory called backpu, but can't find one. It concludes you want to rename your moved file to backpu. You’ll find a file called backpu one directory level higher than your target directory.

ls -l ~/Documents

![The location of the missing and misspelled file.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/5-2.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2087262/19272" target="_top" id="2087262">
  <img src="//a.impactradius-go.com/display-ad/19272-2087262" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2087262/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 To fix this, you can move your file to where it should have gone, and specify its proper name on the command line.

        `mv ~/Documents/backpu ~/Documents/backup/important-file.dat   
ls ~/Documents/backup  
`
    
![Moving and renaming the misspelled file](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/6-2.png) 

 The confusion and the hunt for the missing, badly-named file could have been avoided by adding a trailing slash to the target directory on the command line. That way, if you make a typo, Bash reports an error.

mv ~/Downloads/src/important-file.dat ~/Documents/backpu/

![The trailing slash on the mv command line flags errors with the final directory name](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/7-2.png) 

<!-- affiliate ads begin -->
<a href="https://aidotcom.pxf.io/c/5597632/2134501/19576" target="_top" id="2134501">
  <img src="//a.impactradius-go.com/display-ad/19576-2134501" border="0" alt="https://techidaily.com" width="640" height="90"/>
</a>
<img height="0" width="0" src="https://aidotcom.pxf.io/i/5597632/2134501/19576" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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
<li><a href="https://some-techniques.techidaily.com/updated-humorhatchery-studio/"><u>[Updated] HumorHatchery Studio</u></a></li>
<li><a href="https://youtube-lab.techidaily.com/approved-chuckle-trail-your-guide-to-hilarious-online-stars/"><u>2024 Approved Chuckle Trail Your Guide to Hilarious Online Stars</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-examining-updates-the-2023-samsung-bd-j5900/"><u>2024 Approved Examining Updates The 2023 Samsung BD-J5900</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-expert-tips-for-navigating-the-telegram-online-experience/"><u>2024 Approved Expert Tips for Navigating the Telegram Online Experience</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-implementing-soft-decline-in-logic-pro-audio/"><u>2024 Approved Implementing Soft Decline in Logic Pro Audio</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-increase-snapshot-size-no-quality-compromise/"><u>2024 Approved Increase Snapshot Size - No Quality Compromise</u></a></li>
<li><a href="https://youtube-zero.techidaily.com/approved-youtube-revenue-analysis-made-simple/"><u>2024 Approved YouTube Revenue Analysis Made Simple</u></a></li>
<li><a href="https://win-help.techidaily.com/download-your-favorite-songs-from-youtube-as-mp3-or-flac-files-with-easy-steps/"><u>Download Your Favorite Songs From YouTube as MP3 or FLAC Files with Easy Steps!</u></a></li>
<li><a href="https://some-techniques.techidaily.com/exemplary-narratives-distributed-by-category-for-2024/"><u>Exemplary Narratives Distributed by Category for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/full-range-locomotion-appraisal-for-2024/"><u>Full Range Locomotion Appraisal for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/how-to-switch-on-windows-11s-hdr-functionality-for-2024/"><u>How to Switch On Windows 11'S HDR Functionality for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/ignite-your-design-prowess-top-14-text-animation-snapshots-for-2024/"><u>Ignite Your Design Prowess Top 14 Text Animation Snapshots for 2024</u></a></li>
<li><a href="https://android-unlock.techidaily.com/in-2024-7-ways-to-unlock-a-locked-vivo-phone-by-drfone-android/"><u>In 2024, 7 Ways to Unlock a Locked Vivo Phone</u></a></li>
<li><a href="https://android-frp.techidaily.com/in-2024-easy-guide-to-oneplus-nord-3-5g-frp-bypass-with-best-methods-by-drfone-android/"><u>In 2024, Easy Guide to OnePlus Nord 3 5G FRP Bypass With Best Methods</u></a></li>
<li><a href="https://youtube-help.techidaily.com/in-2024-leveraging-video-for-maximum-impact-with-these-5-youtube-strategies/"><u>In 2024, Leveraging Video for Maximum Impact with These 5 YouTube Strategies</u></a></li>
<li><a href="https://fox-boxes.techidaily.com/lustrous-android-video-techniques-for-every-user-for-2024/"><u>Lustrous Android Video Techniques for Every User for 2024</u></a></li>
<li><a href="https://facebook-video-share.techidaily.com/overcoming-green-tint-in-youtubes-on-mac-a-guide-for-2024/"><u>Overcoming Green Tint in YouTubes on Mac A Guide for 2024</u></a></li>
<li><a href="https://tech-renaissance.techidaily.com/understanding-facebook-from-humble-beginnings-to-global-phenomenon-and-what-makes-it-popular/"><u>Understanding Facebook: From Humble Beginnings to Global Phenomenon & What Makes It Popular</u></a></li>
<li><a href="https://win11-tips.techidaily.com/wav-mp3ogg-movavi/"><u>WAV 파일을 쉽게 MP3/OGG로 전환하세요: Movavi의 공식 오픈소스</u></a></li>
</ul></div>

