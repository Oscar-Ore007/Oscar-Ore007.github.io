---
layout: post
title:      "ColumbusBeer My first CLI project "
date:       2020-03-25 21:04:43 -0400
permalink:  columbusbeer_my_first_cli_project
---

Wrapping up my first CLI project, there are definately some key take aways that I would like to discuss and how I embarked on this journey to create my project. At first, I wanted to create a sneaker application using a free API, focused mainly on allowing the user to select a shoe based on the brand of their choosing and shoe size. However, the API that I chose had some javascript and that was something that I wanted to avoid. My second attempt at my CLI project took me on a journey to create a Sports application that would generate NBA players, teams, and their stats, but creating the application, I decided that start over......AGAIN. 

Throughout this process, I learned that no matter what, you have to stay patient and never give up. I decided that I wanted to talk about a subject that I can relate to, and that's beer. Moving to Columbus, I wanted to pay homage to a special brewery here in town and decided to create a beer application! But first, I had to make sure that I had the right information to work with to avoid having to start over again. I wanted to use an API for this project because I could parse a JSON API with Ruby by using HTTParty: 

```
require 'httparty'

url = 'https://api.spotify.com/v1/search?type=artist&q=tycho'
response = HTTParty.get(url)
response.parsed_response
```

Once I was able to parse my JSON API, I was able to use `Name `and `Description` to give the user 10 different beer selections, as well as a description of their beer selection. Once I created my application, I decided to use ASCII to create a greeting to the user, and I also discovered the gem `colorize` and used that to add finishing touches to my project. 

All in all, the projected opened my eyes on how I need to study throughout my time here at Flatiron. I am thankful to be surrounded by like-minded individuals who truly care about your success in the long run. It was a great experience!
