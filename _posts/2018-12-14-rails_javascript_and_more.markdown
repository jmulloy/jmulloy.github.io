---
layout: post
title:      "Rails, Javascript, and More!"
date:       2018-12-14 19:03:53 +0000
permalink:  rails_javascript_and_more
---


For my 4th project in the fullStack Web Developmnent program I was tasked with converting my rails application from my previous project and add JS functionality. This posed as a difficult task at first. I quickly realized what I needed to do in order to get my project finished and turned in.

My first task was to set up a clone and mirror the exisiting rails application. After a couple google searches and help from other students, I was able to easily set up a "mirrored" clone of the application. After I was able to set up the rails application (ensure that it still functioned), my first task was to set up the JS file needed for the Javascript functioanlity I was planning to incorporate. I created the file recipes.js. This file served as a my "base camp" for all of my JS code. After I set up the approriate files and added the require jquery to the application.js file, I was able to start working on serializers. 

I learned in the curriculum that I am able to use a standard rails generator in order to create the serializers. I struggled with getting the proper information inside of each serializer based on hwo the models looked. After reading over the curriculum and with help from the project support I realized I needed to replicate the same structure of the models with relationships inside of each serializer. Once the serializers were set up, I quickly realized that I wanted to have a separate page in my application for my JS functionality compared to the rails side of the application.

This led me to create a "landing" page for my JS application. I had to create a new view for the landing and I set up a div container for all of my JS and Jquery to display in. The next step was to set up a get and post route for this landing page to make sure the applicastion was functioning properly. After the landing routes were set up the last step was to set up a method inside of my recipes controller. 

After getting the layout coded in, I was ready to dive into the JS code itself. Based on what I learned in the curriculum, I knew I was going to need to add event listeners for each of the links I wanted a user to interact with. Once I had the listeners working and preventing the default actiosn from taking place, I started diving deep into the code to get everything coded in so when All Recipes, My Recipes, or Create a Recipe was clicked the JS framwork would take over for rails and give the app the functionality. 

One thing I struggled with was setting up the jquery calls to make sure I was grabbing the right information and setting it up properly. Another issue I ran into was building the html I wanted to append to the page so the user could get the same functionality with JS as they would for the rails side of the application. Luckily I was able to reference my notes, curriculum, and Google (lots and ltos of googling) to get past each of the obstacles that were presented throughout the project. Another major problem was getting the actual form to render properly when the create a recipe linlk was clicked. I had to set a customer variable to grab the proper URL so the applciation new which URL to grab the form from. Once that was completed I simply used AJAX to finish the functionality of the Create a Recipe function.

Overall I found this project to be difficult when I first started, but I quickly realized how much I had actually learned in the 2 JS sections which gave me the confidence I needed to push through, overcome obstacles and ultimately get the application built to meet the requirements. This project helped solidify my understanding of basic Javascript as well as the combinastion of using Javascript inside of a rails application with the ability to replicate the functionality in a new language. I am excited to present this project and be one step closer to my goal of graduating anf comepleting all coruse work required by the Flatiron School.
