---
layout: post
title:      "Upgrading Node For React"
date:       2019-05-09 14:55:10 +0000
permalink:  upgrading_node_for_react
---


Today was one of those days that I woke up with a lot of inspiration and I had an idea to build out a personal portfolio website to display my projects from school through React. If you are familiar with React, it is an awesome framework that allows developers to easily create and manage the application with a few easy commands. I wanted to be able to create the application and then proceed to build out some of the core functionality. In order to get started with React I needed to run a `create-react-app <app_name>`.

However, when I ran the command I was able to get everything started and my terminal was running everything fine until I got an error for not having an updated version of node. This seems fair since I haven't updated Node.js in a while (can't remember when I updated, I think the last update was when it was installed). Apparently, I needed at least a 10.2 version of node and I was running 6.11.2 locally on my MacBook. First steps I took was to run a standard `npm install -g n` and then run `sudo n latest`. This seemed to be going well and after the install took place I ran `node -v` hoping to see the version increase but it stayed the same. So I was back to where I originally started. 

Next step I was going to try was to update Node through homebrew. Homebrew was something that I installed a few months back. I haven't really thought about needed to update it but I read online that the node version can be updated by updating homebrew itself. The first step in this process was to run `brew install node`. After the install took place I ran 2 additional commands in the following order, 1. `brew update` and then 2. `brew upgrade node`. This resulted in both good news and bad news. The good news was that I updated homebrew but the bad news was the node didn't update. Again, back to square one. 

The FInal step I tried was to update the nvm directly. This unlike the other steps had a single command line that needed to be ran. The code I entered on the command line was `nvm install node --reinstall-packaghes-from=node`. After running this command the terminal started updating lots of things on the back end and I patiently waited for the status bar to reach 100% and finish the installation itself. After a few seconds of waiting, the install took place and it was time for the moment of truth. I ran the `node -v` command and the computer outputted that my node version had been updated to `v12.2.2`. 

Now that I was able to successfully update my Node locally on my mac, I was ready to try and get my new project started. I circled back to the original command I wanted to run which was `npx create-react-app <app_name>`. The computer-executed the command appropriately and within minutes I was able to open up the project in my local environment and start coding! One big thing I learned from this process is to continue to research and try everything you can to achieve the functionality you are wanting. The internet is a wonderful place to find resources and even learn new/easier ways to execute code!

