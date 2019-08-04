<!-- styling, just for a better local live preview -->
<link rel="stylesheet" href="https://unpkg.com/picnic">
<style>body { margin: 2em; }</style>

## Yummy recipes

View the site <https://themagicmushrooms.github.io/recipes/>

## Build etc

### Created with, based on <https://jekyllrb.com/>:

~~~
sudo gem install bundler jekyll
jekyll new recipes
# ^^^^ interrupted because it was asking for a password
cd recipes
bundle install --path vendor/bundle
~~~

Then pushed on github, set master as the github-pages branch (on github, in repo settings).

### Run with

~~~
bundle exec jekyll serve -l
~~~

The **`-l` is for livereload, which is very convenient** (the browser refreshes automatically).

### Github showing unstyled thing

In `_config.yml`

~~~
baseurl: "/recipes"
~~~
to correspond to the fact that the site is hosted on `https://....../recipes`

### Changing theme...

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
so we switch back to minima


## Generating an epub

~~~
pandoc https://themagicmushrooms.github.io/recipes/aio -o food-good.epub
# @send food-good.epub
~~~

also available at https://dl.heeere.com/food-good.epub


## Importing images

~~~
# e.g.
convert '/home/.../DSC_0701.JPG' -resize 512 assets/tempeh-marine-saucisses.jpg
~~~

