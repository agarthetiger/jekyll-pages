#!/usr/bin/env ruby
require 'jekyll'
require 'html-proofer'

task :build do
  config = Jekyll.configuration({
    'source' => './docs',
    'destination' => './docs/_site'
  })
  site = Jekyll::Site.new(config)
  Jekyll::Commands::Build.build site, config
end

task :test => [:build] do
  options = { :check_html => true , :check_img_http => true }
  HTMLProofer.check_directory("./docs/_site", options).run
end
