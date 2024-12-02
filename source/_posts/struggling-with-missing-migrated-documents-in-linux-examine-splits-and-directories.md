---
title: Struggling with Missing Migrated Documents in Linux? Examine Splits and Directories!
date: 2024-11-27T21:51:01.738Z
updated: 2024-12-01T23:21:04.286Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/a-magnifying-glass-pointed-at-the-linux-mascot-next-to-a-file-folder.jpg
---

## Struggling with Missing Migrated Documents in Linux? Examine Splits and Directories!

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/RBN1gYY5hUs?si=p89CMiMzeJzU0wGu" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

### Quick Links

* [How This Particular Problem Foxes People](https://vimeo-videos.techidaily.com/2024-approved-discovering-vimeo-home-for-high-quality-films/)
* [The Part Slash Plays in the mv Command](https://youtube-help.techidaily.com/in-2024-optimized-video-engagement-with-peak-post-times/)
* [It’s Not Exactly Slash’s Fault](https://mondly-stories.techidaily.com/film-and-television-as-educational-resources/)

 Typically, mv is one of the first Linux commands you learn. But one little slip, and things can get surprisingly confusing for the user. Sometimes it looks like moved files have simply vanished.

##  How This Particular Problem Foxes People

 Moving a file on the [command line is pretty simple](https://buynow-help.techidaily.com/misinterpretation-of-gram-staining-results-can-lead-to-incorrect-identification-affecting-treatment-decisions-in-clinical-settings/). You specify the file you want to move, and where you want to move it to. But still, it’s easy for a new user to find themselves exasperated and frustrated over mv.

 They try to move a file into a directory, and it seems to work. They don’t get a confirmation message, but neither do they get an error message. Linux often takes the no news is good news approach. If you don’t get an error message, it must have worked.

 Or did it? When they cd into the target directory, the file isn’t there. And of course, because mv moves the file from the original directory, it’s not there either. It’s starting to look like the file has been lost in the ether. This is usually the point where the frustrated user reaches out for help.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/5EKBEujWCw4?si=PwVvvervi8OrYaEA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/pGHmqD53gc8?si=ymgHIB6Aa7_MoUUf" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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

 The original and target directories are both empty. Where did the file go?

 Bash tries to find a directory called backpu, but can't find one. It concludes you want to rename your moved file to backpu. You’ll find a file called backpu one directory level higher than your target directory.

ls -l ~/Documents

![The location of the missing and misspelled file.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/5-2.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/LT4sdZgUvRQ?si=SvQD5FouEzu4UHpJ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/4qA2pGQ5qmw?si=1mAA9WTi2Z5F7n6s" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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
<li><a href="https://some-techniques.techidaily.com/new-in-depth-analysis-the-best-livestreaming-video-tech/"><u>[New] In-Depth Analysis The Best Livestreaming Video Tech</u></a></li>
<li><a href="https://eaxpv-info.techidaily.com/updated-2024-approved-from-frames-to-fun-youtube-gifs-creation-made-simple/"><u>[Updated] 2024 Approved From Frames to Fun YouTube GIFs Creation Made Simple</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-expertise-in-spotify-advertising-a-playbook-guide/"><u>[Updated] Expertise in Spotify Advertising A Playbook Guide</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-gamers-guide-to-elite-streaming-platforms/"><u>[Updated] Gamers' Guide to Elite Streaming Platforms</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-hero5-vs-yi-evaluating-cutting-edge-cameras/"><u>[Updated] Hero5 Vs. YI Evaluating Cutting-Edge Cameras</u></a></li>
<li><a href="https://facebook-clips.techidaily.com/updated-in-2024-expanding-your-fb-video-scope-full-hd/"><u>[Updated] In 2024, Expanding Your Fb Video Scope Full HD</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-fabricate-fascinating-face-painting-gifs-on-giphy/"><u>2024 Approved Fabricate Fascinating Face-Painting Gifs on Giphy</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-guiding-steps-for-effective-gopro-time-lapse-capture/"><u>2024 Approved Guiding Steps for Effective GoPro Time-Lapse Capture</u></a></li>
<li><a href="https://audio-shaping.techidaily.com/2024-approved-pro-level-mp3-cutting-discover-the-top-5-online-platforms/"><u>2024 Approved Pro-Level MP3 Cutting Discover the Top 5 Online Platforms</u></a></li>
<li><a href="https://extra-tips.techidaily.com/androids-prime-collage-app-selection-overview/"><u>Android's Prime Collage App Selection Overview</u></a></li>
<li><a href="https://screen-sharing-recording.techidaily.com/excellent-pc-screen-grabbers-the-most-useful-1-5/"><u>Excellent PC Screen Grabbers The Most Useful #1-#5</u></a></li>
<li><a href="https://tech-recovery.techidaily.com/exploring-the-appeal-of-the-light-phone-3s-simplicity-and-mechanical-features/"><u>Exploring the Appeal of the Light Phone 3'S Simplicity and Mechanical Features</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-gigglygraphics-mememakers-haven/"><u>In 2024, GigglyGraphics MemeMaker's Haven</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-implementing-precise-timing-features-for-engaged-youtube-audiences/"><u>In 2024, Implementing Precise Timing Features for Engaged YouTube Audiences</u></a></li>
<li><a href="https://win11.techidaily.com/mastering-the-art-of-correcting-errored-photo-transfers-from-iphones/"><u>Mastering the Art of Correcting Errored Photo Transfers From iPhones</u></a></li>
<li><a href="https://win-comparisons.techidaily.com/section-4a-advanced-topic-ocular-immunology/"><u>Section 4A: Advanced Topic - Ocular Immunology</u></a></li>
<li><a href="https://discover-deluxe.techidaily.com/troubleshooting-guide-fixing-non-operational-windows-11-task-scheduler/"><u>Troubleshooting Guide: Fixing Non-Operational Windows 11 Task Scheduler</u></a></li>
</ul></div>

