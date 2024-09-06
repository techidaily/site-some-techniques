---
title: Struggling with Missing Migrated Documents in Linux? Examine Splits and Directories!
date: 2024-09-05T05:27:32.725Z
updated: 2024-09-06T05:27:32.725Z
tags:
  - desktop
categories:
  - tech
thumbnail: https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/a-magnifying-glass-pointed-at-the-linux-mascot-next-to-a-file-folder.jpg
---

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2082536/7443" target="_top" id="2082536">
  <img src="//a.impactradius-go.com/display-ad/7443-2082536" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2082536/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Struggling with Missing Migrated Documents in Linux? Examine Splits and Directories!

### Quick Links

* [How This Particular Problem Foxes People](https://vimeo-videos.techidaily.com/2024-approved-discovering-vimeo-home-for-high-quality-films/)
* [The Part Slash Plays in the mv Command](https://youtube-help.techidaily.com/in-2024-optimized-video-engagement-with-peak-post-times/)
* [It’s Not Exactly Slash’s Fault](https://mondly-stories.techidaily.com/film-and-television-as-educational-resources/)

 Typically, mv is one of the first Linux commands you learn. But one little slip, and things can get surprisingly confusing for the user. Sometimes it looks like moved files have simply vanished.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1934292/19272" target="_top" id="1934292">
  <img src="//a.impactradius-go.com/display-ad/19272-1934292" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1934292/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
##  How This Particular Problem Foxes People

 Moving a file on the [command line is pretty simple](https://buynow-help.techidaily.com/misinterpretation-of-gram-staining-results-can-lead-to-incorrect-identification-affecting-treatment-decisions-in-clinical-settings/). You specify the file you want to move, and where you want to move it to. But still, it’s easy for a new user to find themselves exasperated and frustrated over mv.

 They try to move a file into a directory, and it seems to work. They don’t get a confirmation message, but neither do they get an error message. Linux often takes the no news is good news approach. If you don’t get an error message, it must have worked.

 Or did it? When they cd into the target directory, the file isn’t there. And of course, because mv moves the file from the original directory, it’s not there either. It’s starting to look like the file has been lost in the ether. This is usually the point where the frustrated user reaches out for help.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2094422/7443" target="_top" id="2094422">
  <img src="//a.impactradius-go.com/display-ad/7443-2094422" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2094422/7443" style="position:absolute;visibility:hidden;" border="0" />
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

 That’s nice and simple, and everything works as expected. If we look into our target directory, we find the moved file, and we get on with the rest of our work.

![A moved file in its new directory.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/2-4.png) 

 But let's say our Linux newcomer isn’t using [tab completion](https://desktop-recording.techidaily.com/new-2024-approved-an-impartial-appraisal-the-power-of-recordcast/). They're typing the directory paths by hand. If they misspell the name of the final directory, we get a very different behavior.

mv ~/Downloads/src/important-file.dat ~/Documents/backpu

![Trying to use the mv command with a typo in the final directory name.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/3-3.png) 

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2075476/7443" target="_top" id="2075476">
  <img src="//a.impactradius-go.com/display-ad/7443-2075476" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2075476/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 They’ve made a typo with the target directory name, but mv exits silently back to the command prompt. On the face of it, it looks like the file move worked.

 Let’s check.

        `ls ~/Downloads/src  
ls ~/Documents/backup/  
`
    
![Using ls to look for the file in the original and new directories.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/07/4-2.png) 

<!-- affiliate ads begin -->
<a href="https://imp.i357552.net/c/5597632/1006793/11832" target="_top" id="1006793">
  <img src="//a.impactradius-go.com/display-ad/11832-1006793" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://imp.i357552.net/i/5597632/1006793/11832" style="position:absolute;visibility:hidden;" border="0" />
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

<!-- affiliate ads begin -->
<a href="https://laganoo.pxf.io/c/5597632/1528703/16446" target="_top" id="1528703">
  <img src="//a.impactradius-go.com/display-ad/16446-1528703" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://laganoo.pxf.io/i/5597632/1528703/16446" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://screen-video-capture.techidaily.com/new-2024-approved-maximizing-the-potential-of-virtual-dialogue-secrets-from-a-pro-zoom-chat-guru/"><u>[New] 2024 Approved  Maximizing the Potential of Virtual Dialogue  Secrets From a Pro ZOOM Chat Guru</u></a></li>
<li><a href="https://facebook-video-footage.techidaily.com/new-affordable-online-education-hosting-on-youtube-for-2024/"><u>[New] Affordable Online Education  Hosting on YouTube for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-filmeditingsuite-assessment-detailed-insights/"><u>[New] FilmEditingSuite Assessment – Detailed Insights</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-from-camera-clicks-to-youtube-clips-an-experts-step-by-step-visual-instruction-manual/"><u>[New] From Camera Clicks to YouTube Clips  An Expert's Step-by-Step Visual Instruction Manual</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-from-fuzzy-frames-to-sharpness-the-v22-journey/"><u>[New] From Fuzzy Frames to Sharpness - The V2.2 Journey</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-from-ground-to-sky-discovering-mavic-pro-wonders/"><u>[New] From Ground to Sky - Discovering Mavic Pro Wonders</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-game-masters-unleashed-an-in-depth-look-at-kinemaster-on-android/"><u>[New] Game Masters Unleashed  An In-Depth Look at KineMaster on Android</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-guide-to-top-frame-rates-in-slow-motion-video-production/"><u>[New] Guide to Top Frame Rates in Slow-Motion Video Production</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-how-to-transfer-photos-and-videos-from-android-phone-to-an-iphone/"><u>[New] How to Transfer Photos and Videos From Android Phone to an iPhone</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-ideal-starter-accessories-for-gopro-newbies/"><u>[New] Ideal Starter Accessories for GoPro Newbies</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-immersive-exploration-mastering-close-up-views-in-minecraft/"><u>[New] Immersive Exploration  Mastering Close-Up Views in Minecraft</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/new-pro-iphone-photo-illumination-tricks/"><u>[New] Pro Iphone Photo Illumination Tricks</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/updated-2024-approved-5-tricks-for-instantly-boosting-youtube-subscribers/"><u>[Updated] 2024 Approved  5 Tricks for Instantly Boosting YouTube Subscribers</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-foremost-12-gps-enabled-cctv-cameras-for-motion-recording/"><u>[Updated] Foremost 12 GPS-Enabled CCTV Cameras for Motion Recording</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-guide-to-accessing-price-null-picture-content/"><u>[Updated] Guide to Accessing Price-Null Picture Content</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-innovate-funny-graphics-share-on-giphy-platform/"><u>[Updated] Innovate Funny Graphics, Share on Giphy Platform</u></a></li>
<li><a href="https://digital-screen-recording.techidaily.com/updated-real-time-tv-broadcast-preservation-the-easy-guide/"><u>[Updated] Real-Time TV Broadcast Preservation - The Easy Guide</u></a></li>
<li><a href="https://extra-support.techidaily.com/2024-approved-perfecting-titles-on-footage-step-by-step-tutorial-for-windows-photos-app/"><u>2024 Approved  Perfecting Titles on Footage  Step-by-Step Tutorial for Windows Photos App</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/can-t-open-mov-files-on-samsung-galaxy-a25-5g-by-aiseesoft-video-converter-play-mov-on-android/"><u>Can't open MOV files on Samsung Galaxy A25 5G</u></a></li>
<li><a href="https://techtrends.techidaily.com/effective-instant-chatting-in-mozilla-thunderbird-step-by-step-tutorial/"><u>Effective Instant Chatting in Mozilla Thunderbird – Step-by-Step Tutorial</u></a></li>
<li><a href="https://some-techniques.techidaily.com/get-to-know-the-pros-of-engaging-with-asmr-for-2024/"><u>Get to Know the Pros of Engaging with ASMR for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/harnessing-lut-power-for-free-high-quality-colorization-for-2024/"><u>Harnessing LUT Power for Free, High-Quality Colorization for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/hdr-rating-does-aurora-deliver-quality-in-2024/"><u>HDR Rating  Does Aurora Deliver Quality, In 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/how-much-video-can-64gb128gb-hold-in-2024/"><u>How Much Video Can 64GB/128GB Hold, In 2024</u></a></li>
<li><a href="https://activate-lock.techidaily.com/how-to-bypass-icloud-by-checkra1n-even-on-iphone-13-pro-if-youve-tried-everything-by-drfone-ios/"><u>How To Bypass iCloud By Checkra1n Even On iPhone 13 Pro If Youve Tried Everything</u></a></li>
<li><a href="https://some-techniques.techidaily.com/illuminating-images-in-lightroom-a-step-by-step-hdr-guide-for-2024/"><u>Illuminating Images in Lightroom  A Step-by-Step HDR Guide for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-exceptional-environments-the-best-screen-snapshots/"><u>In 2024, Exceptional Environments  The Best Screen Snapshots</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-expert-editions-selecting-high-quality-blu-ray-players-freepaid/"><u>In 2024, Expert Editions  Selecting High-Quality Blu-Ray Players (Free/Paid)</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-from-idea-to-implementation-crafting-a-powerful-documntary-narrative/"><u>In 2024, From Idea to Implementation  Crafting a Powerful Documntary Narrative</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-full-dissection-gopro-silver-hero4-model-insight/"><u>In 2024, Full Dissection  GoPro Silver Hero4 Model Insight</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-go-beyond-basics-with-these-advanced-whatsapp-features/"><u>In 2024, Go Beyond Basics with These Advanced WhatsApp Features</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-illuminating-images-in-lightroom-a-step-by-step-hdr-guide/"><u>In 2024, Illuminating Images in Lightroom  A Step-by-Step HDR Guide</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-image-illumination-choose-best-websites-with-photo-framing-features/"><u>In 2024, Image Illumination  Choose Best Websites with Photo Framing Features</u></a></li>
<li><a href="https://extra-tips.techidaily.com/superior-supplements-to-enhance-gopro/"><u>Superior Supplements to Enhance GoPro</u></a></li>
<li><a href="https://mondly-stories.techidaily.com/thrilling-techniques-for-latin-learning/"><u>Thrilling Techniques for Latin Learning</u></a></li>
<li><a href="https://howto.techidaily.com/troubleshooting-guide-how-to-fix-an-unresponsive-samsung-galaxy-f54-5g-screen-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>Troubleshooting Guide How to Fix an Unresponsive Samsung Galaxy F54 5G Screen | Dr.fone</u></a></li>
<li><a href="https://techtrends.techidaily.com/vizio-wi-fi-woes-learn-how-to-troubleshoot-and-restore-connection-easily/"><u>Vizio Wi-Fi Woes? Learn How to Troubleshoot & Restore Connection Easily</u></a></li>
</ul></div>
