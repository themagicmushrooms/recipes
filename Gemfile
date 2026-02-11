source "https://rubygems.org"

# Hello! This is where you manage which Jekyll version is used to run.
# When you want to use a different version, change it below, save the
# file and run `bundle install`. Run Jekyll with `bundle exec`, like so:
#
#     bundle exec jekyll serve
#
# This will help ensure the proper Jekyll version is running.
# Happy Jekylling!
gem "jekyll", "~> 4.3.3"

#gem "kramdown-parser-gfm"

# This is the default theme for new Jekyll sites. You may change this to anything you like.
gem "minima", "~> 2.5.1"

gem "csv"
gem "base64"


# or else I get:
# $ecipes/vendor/bundle/ruby/2.7.0/gems/eventmachine-1.2.7/lib/eventmachine.rb:8:in `require': libruby.so.2.7: cannot open shared object file: No such file or directory - $recipes/vendor/bundle/ruby/2.7.0/extensions/x86_64-linux/2.7.0/eventmachine-1.2.7/rubyeventmachine.so (LoadError)
# needed:
# gem uninstall eventmachine
# change this current file
# bundle-2.7 install
#gem 'eventmachine', '1.2.7', git: 'https://github.com/eventmachine/eventmachine.git', tag: 'v1.2.7'

# If you want to use GitHub Pages, remove the "gem "jekyll"" above and
# uncomment the line below. To upgrade, run `bundle update github-pages`.
# gem "github-pages", group: :jekyll_plugins

# If you have any plugins, put them here!
group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.17"
end

## Windows does not include zoneinfo files, so bundle the tzinfo-data gem
# and associated library.
#install_if -> { RUBY_PLATFORM =~ %r!mingw|mswin|java! } do
#  gem "tzinfo", "~> 1.2"
#  gem "tzinfo-data"
#end

## Performance-booster for watching directories on Windows
#gem "wdm", "~> 0.1.0", :install_if => Gem.win_platform?

