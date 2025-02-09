---
title: Struggling with Missing Migrated Documents in Linux? Examine Splits and Directories!
date: 2025-02-08T18:28:41.560Z
updated: 2025-02-09T19:38:29.057Z
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/1KKovVi9epE?si=EF7KA7b4KsEpWA-M" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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
<iframe width="560" height="315" src="https://www.youtube.com/embed/UJJbj1vbzs8?si=X3zd8thLJKprfuEa" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/HtM7d4dpN1I?si=2vN_xgVGD4eYGORu" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 To fix this, you can move your file to where it should have gone, and specify its proper name on the command line.

        `mv ~/Documents/backpu ~/Documents/backup/important-file.dat   
ls ~/Documents/backup  
`
    
![Moving and renaming the misspelled file](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/6-2.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/2Iv3DjT2Fyw?si=pR_z8ZDDVGF2MvKJ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 The confusion and the hunt for the missing, badly-named file could have been avoided by adding a trailing slash to the target directory on the command line. That way, if you make a typo, Bash reports an error.

mv ~/Downloads/src/important-file.dat ~/Documents/backpu/

![The trailing slash on the mv command line flags errors with the final directory name](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/7-2.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/JNxZ4Z6BVCg?si=522oz1OPSQDhNYWT" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://some-techniques.techidaily.com/new-garageband-strategies-for-perfect-podcast-editing/"><u>[New] GarageBand Strategies for Perfect Podcast Editing</u></a></li>
<li><a href="https://screen-recording.techidaily.com/new-in-2024-complete-guide-timer-addition-to-video-broadcast-platforms/"><u>[New] In 2024, Complete Guide Timer Addition to Video Broadcast Platforms</u></a></li>
<li><a href="https://fox-direct.techidaily.com/new-prime-win11-videography-software-for-editors/"><u>[New] Prime Win11 Videography Software for Editors</u></a></li>
<li><a href="https://facebook-video-share.techidaily.com/new-the-complete-checklist-for-youtube-video-resolution-and-size/"><u>[New] The Complete Checklist for YouTube Video Resolution and Size</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-giggle-guild-creepy-cybernetic-comedians/"><u>[Updated] Giggle Guild Creepy Cybernetic Comedians</u></a></li>
<li><a href="https://instagram-clips.techidaily.com/updated-harmony-in-frames-selecting-music-for-social-media-videos/"><u>[Updated] Harmony in Frames Selecting Music for Social Media Videos</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-exploring-hololens-by-microsoft-a-3d-dream-come-true/"><u>2024 Approved Exploring HoloLens by Microsoft A 3D Dream Come True</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-from-imagination-to-illustration-ranking-the-best-8-iphone-drawing-software/"><u>2024 Approved From Imagination to Illustration Ranking the Best 8 iPhone Drawing Software</u></a></li>
<li><a href="https://fox-http.techidaily.com/elevate-visual-content-with-free-animation-text-for-2024/"><u>Elevate Visual Content with FREE Animation Text for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/explore-top-picks-for-high-resolution-4k-panels-for-2024/"><u>Explore Top Picks for High-Resolution 4K Panels for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/frugal-flight-experts-choice-under-500-drone-guide-for-2024/"><u>Frugal Flight Experts' Choice Under $500 Drone Guide for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/how-to-change-netflix-playback-speed-in-2024/"><u>How to Change Netflix Playback Speed, In 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/ideal-platforms-creating-movies-from-photo-galleries-for-2024/"><u>Ideal Platforms Creating Movies From Photo Galleries for 2024</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/in-2024-android-unlock-code-sim-unlock-your-nokia-xr21-phone-and-remove-locked-screen-by-drfone-android/"><u>In 2024, Android Unlock Code Sim Unlock Your Nokia XR21 Phone and Remove Locked Screen</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-explore-the-best-free-after-effects-resources/"><u>In 2024, Explore the Best FREE After Effects Resources</u></a></li>
<li><a href="https://smart-video-editing.techidaily.com/updated-2024-approved-video-editing-mastery-how-to-add-professional-looking-effects-fast/"><u>Updated 2024 Approved Video Editing Mastery How to Add Professional-Looking Effects Fast</u></a></li>
<li><a href="https://fox-hovers.techidaily.com/virtual-worlds-real-learning/"><u>Virtual Worlds, Real Learning</u></a></li>
<li><a href="https://tech-recovery.techidaily.com/whats-next-for-google-pixel-projecting-cost-launch-dates-and-new-hardware-specs-in-focus/"><u>What's Next for Google Pixel: Projecting Cost, Launch Dates & New Hardware Specs in Focus</u></a></li>
<li><a href="https://howto.techidaily.com/xiaomi-13t-camera-not-working-unexpected-error-fix-it-now-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>Xiaomi 13T Camera Not Working Unexpected Error? Fix It Now | Dr.fone</u></a></li>
</ul></div>

