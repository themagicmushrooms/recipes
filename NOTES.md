<!-- styling, just for a better local live preview -->
<link rel="stylesheet" href="https://unpkg.com/picnic">


Created with, based on <https://jekyllrb.com/>:

~~~
sudo gem install bundler jekyll
jekyll new recipes
# ^^^^ interrupted because it was asking for a password
cd recipes
bundle install --path vendor/bundle
~~~

Run with

~~~
bundle exec jekyll serve
~~~


Lol, changing the theme on github (with their UI), changes the _config.yml file but not the Gemfile, so:

~~~
In Gemfile

-gem "minima", "~> 2.0"
+gem "jekyll-theme-tactile"
~~~

and update the theme (or more), with

~~~
bundle install
bundle exec jekyll serve
~~~

-> we get a blank page, like on github

