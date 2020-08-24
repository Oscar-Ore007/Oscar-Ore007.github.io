---
layout: post
title:      "Sinatra Project: Record Holder"
date:       2020-08-24 02:14:03 +0000
permalink:  sinatra_project_record_holder
---


 The Sinatra Final Project was great! It was my first time making an actual web application and I can't help but thank the corneal gem for exsiting. The corneal gem really set me up for success as the gem takes care of alot of the styling of the project. For Example, the corneal gem has the following file structure: 

```
├── config.ru
├── Gemfile
├── Gemfile.lock
├── Rakefile
├── README
├── app
│   ├── controllers
│   │   └── application_controller.rb
│   ├── models
│   └── views
│       ├── layout.erb
│       └── welcome.erb
├── config
│   ├── initializers
│   └── environment.rb
├── db
│   └── migrate
├── lib
│   └── .gitkeep
└── public
|   ├── images
|   ├── javascripts
|   └── stylesheets
|       └── main.css
└── spec
    ├── application_controller_spec.rb
    └── spec_helper.rb
```

Now with our file structure set up, it was time to create the application! I recent bought a record player and I knew that making an application around music would be great! I had to establish a couple of things first, my models, views, and controller fiiles. With the help with Active Record, I was able to create a database that would create a User table and a Record table. Once I created the schema, it was time to create the models. I created a User.rb file and a Record.rb file to establish the has_many, belong to relationship. Once that was done, it was time to move on to the rest of my MVC structure. While I was working on this project, I knew I needed to make sure that I created the appropriate routes for the application to flow smoothly! Thats where the Controllers come in. Controller handles users' request and returns a response. The Views folder contains HTML files for the application. I struggled with the views portion of the project, maninly due to my typos that I experiened with some of my <html> tags. All in all, the project allowed me to take a small glimpse into what goes into creating a web application from scratch! 
