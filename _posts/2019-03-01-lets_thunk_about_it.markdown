---
layout: post
title:      "Lets Thunk About It"
date:       2019-03-01 15:49:43 +0000
permalink:  lets_thunk_about_it
---

When building React apps, especially when connecting to a Rails API, lost of developer utilize Middleware to help make certain requests to the API. I used middleware to make specific Asynchronous calls to the Rails API on the back end of the application. The use of middleware is ideal for developers because it makes state changes predictable and transparent. Middleware can be used for a number of reasons including logging actions, reporting errors, making an asynchronous request, and dispatching new actions. 

Thunk is a widely used middleware, especially when working with Redux applications. I utilized the Thunk middleware for my React/Redux portfolio project. I utilized Thunk because it allowed me to return functions from my action creators as opposed to a specific action while also being able to dispatch a specific action. There are a bunch of different types of middleware available to a developer. However, I found Thunk to be a commonly used piece of the middleware spectrum. 

In order to incorporate thunk I needed to run `npm start redux-thunk`. After I installed I needed to import that middleware into my `App.js` file. After importing I am able to start utilizing thunk to return functions within my action creators to get passed down the action reducers. After those reducers find a case that matches the type from the action creator, the store gets updated. Upon the store updating, the components displaying information will be updated and re-render the updated data through those components to the user's display. Retrieving data from API’s can be problematic when working/building Redux applications, this is why Middleware and Thunk are very useful tools. Again, Using thunk allows the developer to return a function inside of our action creator instead of a Plain Javascript Object. The Returned function receives a store’s dispatch function and it will dispatch multiple actions. One will update the state to a loading state and the other to update the store with updated data for the user to see/interact with. 

Overall I think Thunk is a very useful piece of middleware to utilize. Especially if working with an external API such as a rails API like I did in my project. Thunk will help developers not only understand how the data is flowing through the application but it will also provide the user with a better conceptual understanding of how the action reducers and creators play a role in updating components and containers to contain an updated data for the user. 

