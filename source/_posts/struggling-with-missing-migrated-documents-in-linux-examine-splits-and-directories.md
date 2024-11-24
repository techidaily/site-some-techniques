---
title: Struggling with Missing Migrated Documents in Linux? Examine Splits and Directories!
date: 2024-11-19T02:59:04.219Z
updated: 2024-11-23T21:14:02.693Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/a-magnifying-glass-pointed-at-the-linux-mascot-next-to-a-file-folder.jpg
---

## Struggling with Missing Migrated Documents in Linux? Examine Splits and Directories!

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/poI1NQxHfjc?si=ZLG0wziYcTKIKwL5&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

### Quick Links

* [How This Particular Problem Foxes People](https://vimeo-videos.techidaily.com/2024-approved-discovering-vimeo-home-for-high-quality-films/)
* [The Part Slash Plays in the mv Command](https://youtube-help.techidaily.com/in-2024-optimized-video-engagement-with-peak-post-times/)
* [It’s Not Exactly Slash’s Fault](https://mondly-stories.techidaily.com/film-and-television-as-educational-resources/)

 Typically, mv is one of the first Linux commands you learn. But one little slip, and things can get surprisingly confusing for the user. Sometimes it looks like moved files have simply vanished.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/9wiIVztRIqQ?si=GBgdwQ78k5hbeFDv&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/wVVp-GggK3U?si=RJb1ClNQV7GjTu_3&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 But let's say our Linux newcomer isn’t using [tab completion](https://desktop-recording.techidaily.com/new-2024-approved-an-impartial-appraisal-the-power-of-recordcast/). They're typing the directory paths by hand. If they misspell the name of the final directory, we get a very different behavior.

mv ~/Downloads/src/important-file.dat ~/Documents/backpu

![Trying to use the mv command with a typo in the final directory name.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/3-3.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/P6Wfzj6YNDM?si=WRZQD9zCdQ1_tW1b&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/lxv4NM-89CU?si=Uj5rOkhrwZ_6QIuW&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://some-techniques.techidaily.com/new-gopro-karma-demystified-a-comprehensive-look/"><u>[New] GoPro Karma Demystified A Comprehensive Look</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-honored-proposals-leading-ringtone-creators-iphone/"><u>[New] Honored Proposals Leading Ringtone Creators iPhone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-gigglegallery-craft-and-share-your-own-funny-faces/"><u>[Updated] GiggleGallery Craft and Share Your Own Funny Faces</u></a></li>
<li><a href="https://remote-screen-capture.techidaily.com/updated-in-2024-premier-selection-of-windows-11s-high-quality-capture-software/"><u>[Updated] In 2024, Premier Selection of Windows 11'S High-Quality Capture Software</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-innovative-android-for-ultimate-3d-playback/"><u>[Updated] Innovative Android for Ultimate 3D Playback</u></a></li>
<li><a href="https://extra-resources.techidaily.com/2024-approved-churn-out-custom-internet-echo-jokes/"><u>2024 Approved Churn Out Custom Internet Echo Jokes</u></a></li>
<li><a href="https://some-techniques.techidaily.com/explore-infinite-artistic-possibilities-with-top-10-apps-for-2024/"><u>Explore Infinite Artistic Possibilities with Top 10 Apps for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/hitting-a-pixel-snag-a6400s-video-problems-for-2024/"><u>Hitting a Pixel Snag A6400's Video Problems for 2024</u></a></li>
<li><a href="https://techidaily.com/how-to-reset-xiaomi-redmi-note-12r-without-the-home-button-drfone-by-drfone-reset-android-reset-android/"><u>How to Reset Xiaomi Redmi Note 12R Without the Home Button | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-future-sighted-the-foremost-cameras-excellence/"><u>In 2024, Future Sighted The Foremost Cameras Excellence</u></a></li>
<li><a href="https://technical-tips.techidaily.com/integrating-pinterest-tabs-into-your-facebook-page-a-comprehensive-guide/"><u>Integrating Pinterest Tabs Into Your Facebook Page: A Comprehensive Guide</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/the-best-android-sim-unlock-code-generators-unlock-your-nokia-c300-phone-hassle-free-by-drfone-android/"><u>The Best Android SIM Unlock Code Generators Unlock Your Nokia C300 Phone Hassle-Free</u></a></li>
<li><a href="https://tech-haven.techidaily.com/the-future-of-ai-with-gpt-5-when-can-we-expect-to-see-it-launch/"><u>The Future of AI with GPT-5: When Can We Expect to See It Launch?</u></a></li>
<li><a href="https://techno-recovery.techidaily.com/unlock-your-iphones-hidden-potential-how-to-utilize-the-in-built-timer-for-stunning-photography/"><u>Unlock Your iPhone's Hidden Potential: How to Utilize the In-Built Timer for Stunning Photography</u></a></li>
<li><a href="https://smart-video-editing.techidaily.com/updated-the-best-free-imovie-replacements-you-need-to-know-about/"><u>Updated The Best Free iMovie Replacements You Need to Know About</u></a></li>
</ul></div>

