---
layout: post
title:      "Using Active Model Serializers"
date:       2019-03-27 15:30:51 +0000
permalink:  using_active_model_serializers
---


Rails is a great language to utilize when working with an API especially if you are working with another language like Javascript for the front end of the application. Serializers are a gem that allows us to format JSON without having to manipulate the front end of our application. Developers can select the specific information they want as well access other pieces of the rails backend with a single request. Most developers will choose to use serializers considering they are easy to manipulate, add and remove as needed while also being able to shorten code where possible. 

Installing the Serializer gem is pretty straightforward like most gems in rails. `gem ‘active_model_serializers’` and then we will need to run bundle install. Thankfully rails makes it easy to simply run these commands within the terminal. Of course, you will want to check in the gemfile that the AMS gem was actually installed before moving on. 

We know that we have some basic data depending on the app we are working on. In order to set up some of our files needed we have some basic commands to run within the rails terminal to get the correct file structure needed. First, we will need to run ` rails g serializer “name of file”`. This is can also be hardcoded by manually creating the files within this structure `/app/serializers/cat_serializer.rb` Please note, the name of the file in this command is contingent based on the app and the types of data your app will be manipulating. If you are building a pet website maybe it will be dogs, cats, fish, or something along those lines. Each model we will be working with will have a corresponding serializer. This is due to the favt that we will pass an object to `render: json` in the controller of the rails app. 

Im sure after reading the last paragraph you are wondering what the object actually is that is being rendered through JSON. Great question! Inside of the serializer we will have an attribute called an `object` this can be whatever JSON object its going to pass through in the moment. Serializer only iterate through/over what it is given to. Let's say we have two routes, an index and show route. The serializer will loop through each object inside and format it regardless of which route we are actually working with within the application. 

This is just a brief overview of what serializers and are and how they can be utilized in these specific types of applications. There is more to cover but this should be just enough to allow you to get the API working on the rails side utilizing the actual rails API and the Active Model Serializers. 

