---
layout: post
title:      "Rails Project: Coffee Reviewer"
date:       2020-10-30 23:17:16 +0000
permalink:  rails_project_coffee_reviewer
---


My Rails project is all about my favorite drink to consume in the morning and that is COFFEE! Coffee Reviewer allows users to input their favorite coffee flavors and brands all while reviewing other brands and flavors from other users as well. First, I needed to establish my associations for my project:

**Rails Associations:**

belongs_to
has_many
has_many :through



Once the set up my associations, it time to start building! During the project build, I wanted to focus on error handling using validations. Validations are used to ensure that only valid data is saved into your database. There are several other ways to validate data before it is saved into your database, including native database constraints, client-side validations and controller-level validations. Here is an example of how I used validations within my user model:

```
class User < ApplicationRecord
    has_many :reviews 
    has_many :reviewed_coffees, through: :reviews, source: :coffee 

    has_many :coffees 

    has_secure_password 

    validates :username, :email, presence: true 
    validates :username, uniqueness: true
```

Throughout the rest of the project, I had to overcome alot of challenges around implementing the frontend of my application. With the help of Bootstrap, I was able to use a CSS framework that could change the way the application looked!  Although I still have alot to learn, I am happy with my results and I am looking forward to improving my frontend skills with Javascript! 
		
		
		
