---
layout: post
title:      "Recipes, Rails, Magic, and More!"
date:       2018-10-31 11:45:26 -0400
permalink:  recipes_rails_magic_and_more
---


For my third project in the Flatiron School curriculum I was tasked with building a rails application from scratch. This project tested the knowledge I learned and helped solidfy my understanding of rails and "Magic" that rails has to offer. I have always been passionate about cooking and I can not tell you the number of times I wanted to make a specific dish and could not find the recipe I needed. This is what lead me to the decision of creating a recipe app for thsi sepcific project. 

To get started I knew I would need a blue print for my project. Without this blueprint I wouldnt have been able to understand how the application needed to function from the inside out. Think of it this way, you decide you want to drive across the country but realize you dont have a map or GPS to get you there. Doesnt make much sesne does it? Inside of this blue print I was able to outline how I wanted to set up my Models, Views, and controllers and most importantly how they will all commnicate/connect to each other. 

After establishing the blueprint I needed to get started on the app, I started creating the files I was going to need which included: models, views, and controllers. In order to get started, I first needed to realize the relationships I was going to need in order to get the functionality I wanted. One of the impaortant relationships I needed was figuring out how I was going to join my models together. This was done with the Quantity model as I realized that quanitities were going to belong to ingredients and recipes. This was important because without the join table my app would not function the way I had envisioned. This relationship can be seen below. 
`class Quantity < ApplicationRecord
    belongs_to :recipe
    belongs_to :ingredient
    accepts_nested_attributes_for :ingredient
end`

After my relationships have been established I needed to start thinking of what each controller was going to need to render based on the views I was going to create. I realized that my recipes controller and the views corresponding to my recipe would be where most of my coding was going to take place. I also needed to make sure that witgh the views I was generating in my terminal that each view had th ecorresponding method inside of the controller to make sure the data/information was being rendered properly. However, that was only half of the battle. I also needed to make sure I had proper routing inside of my config/routes.rb file. Since rails uses relationships to help with the rails magic I needed to create some nested routes. 

These nested routes started simple but I quickyl realized I needed to reconfigure them to only allow access to specific REStful routes inside of my nested routes. I hjave included a snippet of my nested route below. 
```
resources :users, only: [:new, :create] do
    resources :recipes, only: [:new, :create, :index, :update, :edit]
  end
```
This nested resource route ended up saving me a lot of code and helped me get a visual representation of how my app needed to function and route properly between the different files I have generated so far. After establshing the routing I quickly realized I was going to need to reconfigure alot of the method I had originally set up that I thought were going to be needed. However after I had a good idea of how my MVC's needed to commnicate and route properly I was able to confidently start building out the rest of the application. 

After working through my app and debugging for a few days I quickly realized I set up my rouyting wrong. My old routing code was displaying the text in the url for /users/user_id/recipes/1. The user_id was supposed to be pulled/generated from each user that signed up and logged in with exisiting credentials. This led to a bunch of problems including Users having the ability to maniuplate the URL to be able to a ccess a different users data including their recipes. I quickly realized even though its a project that this is not a good feature. In fact, this can be viewed as a massive security breach. I personally would be upset if someone could change their Facebook URL to see all of my information. In order to get this fixed, I haf to take a look at my routing as well and the controllers themselves. I realized I needed to update the update method inside of my Recipe Controller. I was able to make sure the params[:user_id] was in fact the current user that was logged in. After making sure this current user was who they say they were, I created a few flash messages that informed the User that they were unable to change anothers Users data. To make the check for the current user easier, I decided to create a current_user helper method in application controller. This allows me to reference this current user Method inside any of the other controller that inherit from the ApplciationController. Please see the snippet below for how I set up this method. 
```
class ApplicationController < ActionController::Base
    helper_method :current_user
    
    def current_user
     @current_user ||= User.find(session[:user_id]) if session[:user_id]
    end

end
```

After a large amount of trial and error, googling, looking for resources, I finally was confident enough to be able to finish my application. This project was a true test of my knowledge and skills I have learned so far in Flatiron as a developer. After most of the functionality had been completed, I decided to test my self even more by attempting to add a small amount of styling to my application. With the help of external resources I was able to upload a bootstrap temple for a nice, clean looking Navbar. 

This project has not only taught me alot but boosted my confidence tremendously with what I have learned in the curriculum. Before starting the project, I was hesitant to dive head first due to not having a good "grasp" on how rails truly works. I was able to utilizie google and external resources which in combination with the Flatiron Curriculum gave me the resources and tools I needed to not only complete the project but also help solidify what I have learned. To look back and think of where I was with minimal knowledge before starting Flatiron I never would have thought I would get the skills needed to complete a project like this!




