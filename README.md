langtech.github.com
===================

Everything is happening in the "master" branch. 

Prerequisites
-------------

1. Ruby
2. RubyGems

Installation
------------

On a command line, enter:

1. gem install bundler
2. bundle install

Look at and edit website locally
--------------------------------

On a command line, enter:

1. bundle exec jekyll serve -w

You should see this output:

    be jekyll serve -w
    Configuration file: /Users/hanke/temp/langtech.github.com/_config.yml
                Source: /Users/hanke/temp/langtech.github.com
           Destination: /Users/hanke/temp/langtech.github.com/_site
          Generating... done.
     Auto-regeneration: enabled
        Server address: http://0.0.0.0:4000
      Server running... press ctrl-c to stop.

2. open localhost:4000

Deploy the website
------------------

On a command line, enter:

1. git push origin gh-pages