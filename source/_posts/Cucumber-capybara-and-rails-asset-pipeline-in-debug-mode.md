---
date: '2012-09-27'
title: Cucumber capybara and rails asset pipeline in debug mode
tags: 
- testing
- debugging
---
<p><strong>features/support/env.rb</strong></p>

<pre>
Capybara.server_port = 3001
Capybara.app_host = "http://localhost:3001"

ActionController::Base.asset_host = Capybara.app_host
</pre>

<p><strong>config/environments/cucumber.rb</strong></p>

<pre>
config.assets.enabled = true
config.assets.debug = true
</pre>

<hr><p>Source: <a href="http://johnbintz.github.com/blog/2012/01/07/cucumber-capybara-asset-pipeline-debug-mode/">http://johnbintz.github.com/blog/2012/01/07/cucumber-capybara-asset-pipeline-debug-mode/</a></p>
