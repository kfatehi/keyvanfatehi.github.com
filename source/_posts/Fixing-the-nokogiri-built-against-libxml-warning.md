---
date: '2013-04-15'
title: Fixing the nokogiri built against libxml warning
tags:
- ruby
---
<p>Just installed Mountain Lion 10.8 fresh on my Mac Mini with a new SSD. As I get my rails environment up and running I ran into this common problem:</p>

<p><code>WARNING: Nokogiri was built against LibXML version 2.9.0, but has dynamically loaded 2.7.8</code></p>

<p>I had installed nokogiri with bundler. Unfortunately I don&#8217;t know which of these things quite resolved my issue, but this is what I did:</p>

<pre>
gem uninstall nokogiri
brew update
brew uninstall libxml2
brew install libxml2 --with-xml2-config
bundle exec gem pristine nokogiri
</pre>

<p>After all this, the warning was gone. I wish I knew which of these was extraneous, if any, but I guess I&#8217;ll find out next time assuming this common problem doesn&#8217;t get smoothed out upstream.</p>

<p><em>Sources:</em></p>

<p><a href="https://gist.github.com/devpuppy/1349681">https://gist.github.com/devpuppy/1349681</a></p>

<p><a href="http://stackoverflow.com/questions/6802410/warning-nokogiri-was-built-against-libxml-version-2-7-8-but-has-dynamically-lo">http://stackoverflow.com/questions/6802410/warning-nokogiri-was-built-against-libxml-version-2-7-8-but-has-dynamically-lo</a></p>
