---
date: '2011-06-08'
title: Ios get current date time
tags:
- ios
---
<p><span> </span></p>
<p><strong>Source code says it all:</strong></p>
<p><span>NSCalendar<span class="s1"> *calendar = [[</span>NSCalendar<span class="s1"> </span><span class="s2">alloc</span><span class="s1">] </span><span class="s2">initWithCalendarIdentifier</span><span class="s1">:</span>NSGregorianCalendar<span class="s1">];</span></span></p>
<p class="p2"><span class="s3">NSCalendarUnit</span><span class="s1"> unitFlags = </span>NSYearCalendarUnit<span class="s1"> | </span>NSMonthCalendarUnit<span class="s1">| </span>NSWeekCalendarUnit<span class="s1"> |</span>NSDayCalendarUnit<span class="s1"> | </span>NSHourCalendarUnit<span class="s1"> | </span>NSMinuteCalendarUnit<span class="s1"> | </span>NSSecondCalendarUnit<span class="s1">;</span></p>
<p class="p3"><span class="s3">NSDate</span> *date = [<span class="s3">NSDate</span> <span class="s2">date</span>];</p>
<p class="p3"><span class="s3">NSDateComponents</span> *dateComponents = [calendar <span class="s2">components</span>:unitFlags <span class="s2">fromDate</span>:date];</p>
<p class="p3"><span class="s3">NSInteger</span> year = [dateComponents <span class="s2">year</span>];</p>
<p class="p3"><span class="s3">NSInteger</span> month = [dateComponents <span class="s2">month</span>];</p>
<p class="p3"><span class="s3">NSInteger</span> week = [dateComponents <span class="s2">week</span>];</p>
<p class="p3"><span class="s3">NSInteger</span> day = [dateComponents <span class="s2">day</span>];</p>
<p class="p3"><span class="s3">NSInteger</span> hour = [dateComponents <span class="s2">hour</span>];</p>
<p class="p3"><span class="s3">NSInteger</span> minute = [dateComponents <span class="s2">minute</span>];</p>
<p class="p3"><span class="s3">NSInteger</span> second = [dateComponents <span class="s2">second</span>];</p>
<p class="p3">&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;</p>
<p>This was copied directly from a <a href="http://www.dotnetishere.com/post/Objective-C-iOS-get-current-date-time-with-formatted.aspx">blog post of Murat Yilmaz</a> </p>