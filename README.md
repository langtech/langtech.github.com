langtech.github.com
===================

Prerequisites
-------------

1. Ruby
2. RubyGems

Installation
------------

1. gem install bundler
2. bundle install
3. mkdir build
4. cd build

Now we initialize a production git repo in build:

5. git init
6. Modify .git/config so it points origin to the langtech repo.

    [remote "origin"]
      fetch = +refs/heads/*:refs/remotes/origin/*
      url = git@github.com:langtech/langtech.github.com.git

Look and edit website locally
-----------------------------

1. bundle exec middleman
2. open localhost:4567

Deploy the website
------------------

1. bundle exec rake

Note: This builds the site in ./build (which contains a repo pointing to master), then pushes it from the build directory. 