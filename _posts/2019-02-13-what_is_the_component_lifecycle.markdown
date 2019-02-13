---
layout: post
title:      "What is the Component Lifecycle?""
date:       2019-02-13 13:41:45 +0000
permalink:  what_is_the_component_lifecycle
---


The Component Life Cycle is the heart and soul of a React application. The lifecycle is used to acknowledge a user action, moving the data throughout the application with the ultimate end goal of returning the updated data by re-rendering any components that would change due to an updated store. I personally struggled with React when I first started to read about it. There seemed to be a small gap for me in reference to being able to connect the starting point until the endpoint. I want to take some time and run through the Component Lifecycle within a React application. 

React itself is a component-based Javascript library. These components are used to update what we call the Virtual DOM. What is the virtual DOM you asre asking? Great question! The Virtual DOM is a node tree that lists elements and their attributes and content as objects and properties. Programmers utilize different methods in their React applications in order to push specific types of data to the Virtual DOM. These methods also tell the computer what you want to happen in certain cases. The 2 main types of methods are Updating and Mounting. These methods can be used to push and update data in the React application. 

```
Component mounting Methods(initialization):
* constructor()
* componentWillMount()
* render()
* componentDidMount()
```


```
Component Updating Methods(updating). 

* componentWillReceiveProps
* shouldComponentUpdate
* componentWillUpdate
* render
* componentDidUpdate
```


After gaining an understanding of how the Component lifecycle methods work, I was quickly able to grasp how data moved through the application. These methods are used widely in different React apps a they all serve a specific purpose. I am eager to keep learning more about react and working towards gaining the best understanding of the library as I can throughout my years as a programmer. 

