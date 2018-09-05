---
layout: post
title:      "Josh's List App - Sinatra Application"
date:       2018-09-05 14:44:28 +0000
permalink:  joshs_list_app_-_sinatra_application
---


For my second project in the Full Stack Web Development Curriculum with Flatiron School, I decided to build a to do list that can be ran within a browser on a computer. As a student with Flaatiron I was tasked with building a functional Sinatra application that allows users to sign up, login, create, edit, update, and delete information (lists and tasks) within my application. This was a challenging project to complete from start to finish. Thjis project was my next personal milestone in the curriculum. This project presented multiple challenges from the point of starting the application all the way until the end when I was ready to present my application. 

Starting the project was a difficult part due to the fact that as students we got to choose which direction we wanted to go with our app. I was unsure of what I wanted to for my project. I wanted to build an app that I can use in real life and also enjoy programming. Once I got an understanding of what I wanted my application do I quickly realized how much of a skill set I have gained since starting the course only 3 months ago. After forming a blue print ofhow I wanted my application to function I was able to confidently navigate from start to finish. However even . with confidence multiple problems still presented themselves along the way. 

I chose to build a to do list for my project. The inspiration from this project came from personal experiences of never remembering everything I needed to get done around the house, pick up from the store, and just daily activities in general. I thought this would be a great time to seize the opportunity to create something not only I could use but possibly could benefit other people in my life!

One of my biggest frustrations since starting the course has been working on a lab or in this case the sinatra project in particular when things dont work the way you originally planned. It was brought to my attention that this is just the way things are in programming and that it is up to me as a soon to be developer to work through these frustrations and make sure everything is consistently working properly.

**Project Structure**

In order to keep things concise and clear within the application I decided to make the information accessible in my application customizable and dependent on a users persoanl input to make sure the application can be catered to multiple users. This would result in four distinct models in my architecture:

List- The “List” model is the central aspect of this data structure. Lists have a title and then each list can have items added and manipulated based on the users discretion. IUsers will be able to use this list to add any and all types of data they choose to within the text box laid out after each list has been created.

Tasks - The Task Model  is the bread and butter of each list. Most people (programmers and users) included know how a basic to do list should function whether it is in a browser on a computer or it is on pen and paper in their pocket. The tasks model was constructed to belong to lists. Which in return the lists belong to a single user. 

User- The User model is responsible for the data in this architecture. Users have a username and secure password. The users have many lists depending on the number of lists that are created by an individual user. The user also has to have a unique username to be able to sign up for the application as well as a valid email address in order to be able to sign up to use the application. 

I had a few issues come up throughout the process of building the application. These errors ranged from simple syntax errors, bootstrap errors, undefined methods, as well as issues with my controllers. They were difficult to debug. However one thing I realized when working on this project is that Siantra applications have a general "flow" that needs to be followed. Most of the views, models, and controllers have a flow that they need to have set up in order to function properly. Figuring out the flow itself was quite challenging. These challenges were easy to identify but were sometimes difficult to understand/ debug to make sure my applkciation functioned properly from start to finish. One major issue I personally had ewas getting the flash message to generate properly. I had to reference google as well as previous labs to get the flash message to not only shoew up properly but to asl display the correct message. Thankfully I was able to work with fellow students and some instructors with the Flatiron school to get my flash message to function properly regardless of the information that was inputed into the username, password, and email fields when signing up. flash[:message] = "{@user.errors.full_messages.join(", ")}" this sedtion of code was difficult to get hard coded into my app to help with there input errors that a user could result in with lack of information when Signing up for the application. 

I did use multiple resoucres online to clarify my understanding of how the controllers are supposed to function with the different types of routes a controller can have. Also I used the information below to help me get an idea of how the flow should work in my application. I realized quickly that the controllers are what helps your application function properly and navigates the user to the correct pages and different view files. 


Method	General use-case example

get()	- Performing basic HTTP GET requests like loading pages
post() -	Used when posting form data
put() -	Used when updating resources
patch()	- Similar to post(), but used when updating one field of a resource
delete() -	Used when deleting resources
options() -	Determine options available for an associated resource
link() -	Link relationships between existing resources
unlink() -	Unlink relationships between existing resources

By the end of the application construction I was truly impressed with my personal progress throughout the course of being a student here at Flatiron. I am now confident in my abilites to code routes and controllers for different applications. I realized the importance of the Sinatyra section from a programmers perspective from the start to finish of my project. Even after hours of frustration, I was able to finally get my code working the way I originally planned. This project was a true test of my skills and now that I am almost across the finish line my excitement has grown to continue on my path to become the best developer I possibly can. This project not only tested my abilities and skills as a programmer but also my patience to stay calm and continuously work towards getting my program to function flawlessly. I am looking forward to more challenges and projects in the future throughout the rest of my time here at Flatiron!

I am planning to revisit this application down the road once my skill set has grown even more to add different features as well as different programming styling to my application to make it more complex and have a better layout/UI. I am excited to keep moving forward in the curriculum and testing my skills with each lab/project throughout the rest of the curriculum. 




