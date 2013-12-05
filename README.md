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

    gem install bundler

Then:

    bundle install

Look at and edit website locally
--------------------------------

On a command line, enter:

    bundle exec jekyll serve -w

You should see this output:

    Configuration file: [...]/langtech.github.com/_config.yml
                Source: [...]/langtech.github.com
           Destination: [...]/langtech.github.com/_site
          Generating... done.
     Auto-regeneration: enabled
        Server address: http://0.0.0.0:4000
      Server running... press ctrl-c to stop.

To open the website, open a browser at [http://localhost:4000](http://localhost:4000):

    open localhost:4000

Deploy the website
------------------

On a command line, enter:

    git push
    
If that doesn't work, try:
    
    git push origin master

Troubleshooting
---------------

Start the server using the "same" command that Github uses (with safe rendering):

    bundle exec jekyll serve -w --safe

And see if it renders correctly.