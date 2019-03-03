# GitHub Pages with Jekyll and TravisCI

[![Build Status](https://travis-ci.org/agarthetiger/jekyll-pages.svg?branch=master)](https://travis-ci.org/agarthetiger/jekyll-pages)

## Overview
This is a simple repo demonstrating auto-generation of documentation using Jekyll, hosted on GitHub Pages. Often there is more to a repository than just a Jekyll website, so the Jekyll site source is under a docs folder. GitHub Pages will take care of the [publishing](https://help.github.com/en/articles/about-github-pages-and-jekyll#jekylls-build-process) of Jekyll websites, and the repository is configured to use the docs folder on the master branch as the Pages source. There is no build process required to publish the website, so Travis CI is used purely to ensure the site will build correctly and run some basic checks with [html-proofer](https://github.com/gjtorikian/html-proofer).

## Local Jekyll site testing
As with code, all changes should be tested prior to raising a PR to the integration branch. This can be doen automatically on the CI server with a branch builder or run locally. Putting aside any discussions of pros and cons of each, ensure you have Ruby installed, run `bundle install` to install all dependencies then run `bundle exec rake test` to run the tests locally.
