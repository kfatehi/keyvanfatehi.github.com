---
date: '2012-07-31'
title: Zlib error on gem install on debian squeeze
tags: 
- debian
---
<p>Despite having all libzlib dependencies installed, I would still get an error when trying to use <code>gem install</code></p>

<p>As it turns out you need to do an additional step to solve this problem, using your ruby source.</p>

<p><code>cd &lt;ruby_source&gt;/ext/zlib</code></p>

<p><code>make</code></p>

<p><code>make install</code></p>

<p>Now <code>gem install</code> will work fine.</p>
