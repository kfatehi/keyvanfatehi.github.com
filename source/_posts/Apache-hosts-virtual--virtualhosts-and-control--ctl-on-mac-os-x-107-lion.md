---
date: '2012-06-08'
title: Apache hosts virtual  virtualhosts and control  ctl on mac os x 107 lion
tags: 
---
<p><a href="https://rapd.wordpress.com/2008/06/09/apache2-vhosts-for-multi-host-names/">https://rapd.wordpress.com/2008/06/09/apache2-vhosts-for-multi-host-names/</a></p>
<p>Indeed, I forget as well. Thanks.</p>
<p>Here&#8217;s info on apachectl, used to stop, start, restart your apache2 httpd server</p>
<p><a href="http://www.cyberciti.biz/faq/restarting-apache-under-oxs-commandline/">http://www.cyberciti.biz/faq/restarting-apache-under-oxs-commandline/</a></p>
<p>Still having issues? Did you remember to uncomment </p>
<p># Virtual hosts</p>
<p># Include /private/etc/apache2/extra/httpd-vhosts.conf</p>
<p>in the httpd.conf file?</p>
<p>Still pretty relevant even though it&#8217;s old: <a href="http://www.fuzzylizard.com/archives/2008/05/29/947/">http://www.fuzzylizard.com/archives/2008/05/29/947/</a></p>