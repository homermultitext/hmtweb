# `hmtweb`


Jekyll web site for www.homermultitext.org using [Hydejack](https://hydejack.com/docs/) theme.


## Prerequisites

- ruby with bundler (install ruby and run `gem install bundler`)

## Quick start

Within the `jekyll` directory, run `bundle install` (one-time setup), then:

-  to run locally, `bundle exec jekyll serve --watch`
-  to build, `bundle exec jekyll build`
-  to install on www.homermultitext.org, `rsync -avz --no-perms --no-owner --no-group _site/ AUTHORIZEDUSER@www.homermultitext.org:/var/www/html/hmt`


Tip:  the `facsimiles` directory includes hundreds of individual files.  Jekyll needs several minutes to index these files. Without the `facsimiles` directory, jekyll can serve or build the site in a few seconds, so to work on the site   it's much easier to move the `facsimiles` folder temporarily outside the `jekyll` directory before serving or building.  (Obviously, that's not an option if you're actually working on the facsimiles.)
