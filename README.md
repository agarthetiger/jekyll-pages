# GitHub Pages with Jekyll and TravisCI

## Overview
This is a simple repo demonstrating auto-generation of documentation using Jekyll, hosted on GitHub Pages. Often there is more to a repository than just a Jekyll website, so the Jekyll site source is under a docs folder and GitHub is configured to use the gh-pages branch to serve the documentaiton. Changes in the repository will trigger TravisCI, which will only publish to the gh-pages if the changes have been made or merged to the master branch, the Jekyll build passes and html-proofer doesn't find any problems. 

## Local Jekyll site testing
As with code, all changes should be tested prior to raising a PR to the integration branch. This can be doen automatically on the CI server with a branch builder or run locally. Putting aside any discussions of pros and cons of each, here are the steps needed to run the site locally, to perform the same automated tests and also to serve the site so the content can be checked manually. 

1. Do something
1. Do something else
1. etc
1. WIP
