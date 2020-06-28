---
layout: post
title:      "CLI Project: COVIDTracker"
date:       2020-06-27 11:32:22 -0400
permalink:  cli_project_covidtracker
---


I decided to have my CLI project be related to something that has impacted many people across the country, and that is COVID-19. I wanted to get information that could reflect the status of COVID -19 across the United States by showing confirmed cases, deaths, and active cases. I chose the following API to get my information: https://documenter.getpostman.com/view/10808728/SzS8rjbc?version=latest#63fda84a-6b43-4506-9cc7-2172561d5c16. This was a great resource and I wanted to make sure my numbers were as accurate as possible. Once I decided on the information, it was time to build the project. I wanted to make sure I had a good understanding of the workflow of my project, and I needed to make sure that I built small and tested A LOT! The first part was to get the my environment file situated. I needed to have the following gem in my file:


COVIDTracker.gemspec
gemspec

gem "rake", "~> 12.0"
gem "rspec", "~> 3.0"

gem "httparty", "~> 0.18.1"

gem "pry", "~> 0.13.1"

gem "colorize', '~> 0.8.1"

I needed to use HTTParty to get the information from the API, and I also needed my handy 'pry' gem. I also added the 'colorize' gem to add a little flare to the project, by colorizing my text. Once, that was done, it was time to set up the environment file. The environment file holds my project together, and allows my files to run smoothly together: 

require_relative "./COVIDTracker/version"
require_relative './api_manager'
require_relative './cli'
require_relative './cases'

require 'pry'
require 'httparty'
require 'colorize'

module COVIDTracker
  class Error < StandardError; end

end

After getting my environment file set up, it was time to get the bin file working to start the application in the terminal:

#!/usr/bin/env ruby

require_relative '../lib/environment'

COVIDTracker::CLI.new.start 

After that, it was all about building the application and making sure that I ran a lot of tests throughout the process. The biggest takeaway for me on this project was to really start small and test often. Once I felt confident with the code that I was focusing on, I moved on to the next block/ method that I needed to work on. All in all, it was a great project and I am very happy with the results! I am looking forward to expanding my knowledge around software development and tackle other projects in the future! Stay tuned! 
