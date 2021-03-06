---
date: '2011-06-10'
title: How to access the contents of the iphone hard disk drive
tags:
- iphone
---
<p>You may want to see and access the files you&#8217;re creating in your Documents or tmp directories while coding with iOS. Directly accessing those folders with Finder turns out to be rather difficult.</p>
<p>It was recommended to me in #iphonedev (freenode) to do the following in order to view the files in iTunes:</p>
<p>1) In Xcode, open up your &lt;appname&gt;-Info.plist file and add a new string by Ctrl-clicking an existing row and clicking &#8220;add row&#8221;:</p>
<p>The string should be set to: &#8221;Application supports iTunes file sharing&#8221;, it should be a Boolean, and the value should be YES</p>
<p>2) Open up iTunes and access it from the Apps section of your device.</p>

<p>So I was doing it this way, and received this dreaded message: </p>

{% asset_img usure.png iTunes you will be the death of me. %}

<p><strong>My iPhone is associated with a different mac&#8230; And I don&#8217;t want to delete everything just to access it from my development machine. To get around this, you will need to spend money on an application called Phone Disk.</strong></p>
<p>Phone Disk gives you direct access to your root directory of your iPhone. It worked perfectly for what I needed.</p>
<p>The trial allows you to transfer up to 100MB. A license is $9.99. You can find it here: <a href="http://www.macroplant.com/phonedisk/"><a href="http://www.macroplant.com/phonedisk/">http://www.macroplant.com/phonedisk/</a></a></p>
