# f21

https://ucsb-cs148.github.io/f21/

Jekyll based website for UCSB CS148, Fall 2021

Website: <https://ucsb-cs148.github.io/f21/>

This version is intended to replace <https://ucsb-cs148-f21.github.io>.

It uses the new Jekyll theme approach to make these sites easier to maintain.

The theme currently being used can be find in the jekyll-theme value
in `_config.yml`

The navigation is set by the values in `_data/navigation.yml`

Jekyll status on Travis-CI: [![Build Status](https://travis-ci.com/ucsb-cs48/f21.svg?branch=main)](https://travis-ci.com/ucsb-cs148/f21)

* Travis-ci: https://travis-ci.com/ucsb-cs148/f21
* To add a status image like this in your README.md, see [these instructions](https://docs.travis-ci.com/user/status-images/)

To test locally:
* One time setup:
    * `git clone` the repo
    * Install rvm (the Ruby version manager)
    * Run `./setup.sh` to install correct ruby version, bundler version, and bundle the gems
* From then on, to test the site locally:
    * Run `./jekyll.sh
    * Point browser to <http://localhost:4000/f21/>


