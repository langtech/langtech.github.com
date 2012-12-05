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
3. In "build": git init
4. In "build": Modify .git/config so it points origin to the langtech repo.

Deployment
----------

1. rake

Note: This builds the site in ./build (which contains a repo pointing to master), then pushes it from the build directory. 