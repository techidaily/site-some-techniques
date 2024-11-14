---
title: Struggling with Missing Migrated Documents in Linux? Examine Splits and Directories!
date: 2024-11-07T17:19:18.384Z
updated: 2024-11-12T23:55:24.585Z
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

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1884002/19272" target="_top" id="1884002">
  <img src="//a.impactradius-go.com/display-ad/19272-1884002" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1884002/19272" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://imp.i357552.net/c/5597632/1001446/11832" target="_top" id="1001446">
  <img src="//a.impactradius-go.com/display-ad/11832-1001446" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://imp.i357552.net/i/5597632/1001446/11832" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://appsumo.8odi.net/c/5597632/2132161/7443" target="_top" id="2132161">
  <img src="//a.impactradius-go.com/display-ad/7443-2132161" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2132161/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 To fix this, you can move your file to where it should have gone, and specify its proper name on the command line.

        `mv ~/Documents/backpu ~/Documents/backup/important-file.dat   
ls ~/Documents/backup  
`
    
![Moving and renaming the misspelled file](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/6-2.png) 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1918698/19272" target="_top" id="1918698">
  <img src="//a.impactradius-go.com/display-ad/19272-1918698" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1918698/19272" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://some-techniques.techidaily.com/new-full-review-comprehensive-look-at-videoshow-in-24/"><u>[New] Full Review - Comprehensive Look at VideoShow in '24</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-hosting-charismatic-chats-keeping-audiences-hooked-live/"><u>[New] Hosting Charismatic Chats Keeping Audiences Hooked Live</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-how-to-effectively-move-files-between-two-ios-units/"><u>[New] How to Effectively Move Files Between Two iOS Units</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-how-to-watch-record-and-edit-football-matches-for-free/"><u>[New] How to Watch, Record, and Edit Football Matches for Free</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/new-in-2024-end-scene-excellence-your-guide-to-yt-outro-mastery/"><u>[New] In 2024, End Scene Excellence Your Guide to YT Outro Mastery</u></a></li>
<li><a href="https://extra-approaches.techidaily.com/new-nikon-d500-unveiled-the-frontier-of-high-definition-photography/"><u>[New] Nikon D500 Unveiled The Frontier of High-Definition Photography</u></a></li>
<li><a href="https://digital-screen-recording.techidaily.com/updated-audiovisual-pro-perfect-ppt-presentation-recording-for-2024/"><u>[Updated] Audiovisual Pro Perfect PPT Presentation Recording for 2024</u></a></li>
<li><a href="https://extra-information.techidaily.com/updated-cerebral-showcase-2024-exclusive-selection-of-trivia-streaming-sites/"><u>[Updated] Cerebral Showcase 2024 Exclusive Selection of Trivia Streaming Sites</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/updated-unlocking-audio-mp3-conversion-from-skype-no-price/"><u>[Updated] Unlocking Audio Mp3 Conversion From Skype, No Price</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-highest-quality-costless-clocks/"><u>2024 Approved Highest Quality Costless Clocks</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-husqvarnas-sky-high-adventure-with-h501s-x4-review/"><u>2024 Approved Husqvarna's Sky-High Adventure with H501S X4 Review</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-illustrators-secret-creating-seamless-image-movement/"><u>2024 Approved Illustrator's Secret Creating Seamless Image Movement</u></a></li>
<li><a href="https://audio-editing.techidaily.com/exploring-toms-hardware-the-ultimate-guide-to-new-technology/"><u>Exploring Tom's Hardware: The Ultimate Guide to New Technology</u></a></li>
<li><a href="https://technical-tips.techidaily.com/guide-to-configuring-various-network-setups-on-your-mac-for-optimal-connection-management-cnet-news/"><u>Guide to Configuring Various Network Setups on Your Mac for Optimal Connection Management | CNET News</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/in-2024-all-you-need-to-know-about-mega-greninja-for-lava-blaze-curve-5g-drfone-by-drfone-virtual-android/"><u>In 2024, All You Need To Know About Mega Greninja For Lava Blaze Curve 5G | Dr.fone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-expert-iphone-videography-strategies-to-elevate-your-work-top-8/"><u>In 2024, Expert iPhone Videography Strategies to Elevate Your Work (Top 8)</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-from-raw-images-to-stunning-photos-your-guide-to-iphone-photomosaic-creation/"><u>In 2024, From Raw Images to Stunning Photos Your Guide to iPhone Photomosaic Creation</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/secrets-to-proficient-gaming-recordings/"><u>Secrets to Proficient Gaming Recordings</u></a></li>
<li><a href="https://extra-information.techidaily.com/the-future-of-filming-xs-100is-bold-journey/"><u>The Future of Filming XS 100I's Bold Journey</u></a></li>
</ul></div>

