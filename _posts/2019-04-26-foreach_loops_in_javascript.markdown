---
layout: post
title:      "forEach() Loops in Javascript"
date:       2019-04-26 11:56:50 +0000
permalink:  foreach_loops_in_javascript
---


If you are familiar with the blogs I have posted in the past then I am sure you have noticed that I have a passion for front end development, specifically working in the Javascript language. Javascript has a lot of useful methods that can be used within functions. One thing I noticed while learning Javascript was that there were a few different loop “types” that I was using throughout my code depending on the functionality I was trying to achieve. If you havent already seen it, I wrote a blog post previously about while loops and today I want to discuss the `.forEach() `loop that javascript programmers use/need to understand as part of the framework. 

Loops are used in Javascript as a way to run a specific section of code mulltiple times until a condition is met. This is a very basic definiton about loops, so lets dive into the specifics of using the `forEach()` loop. The way I like to think about forEach loops is to think of it as a loop I want to run when I want loop to array over “each” individual element. In specifc, lets say we have an array with 5 elements in. I would use a forEach() loop to iterate over all 5 elements within that array until a specific condition is met which in this case would be after all the elements have iterated over. Lets take a look at some code.

```
arr.forEach(function (item) {
  someFn(item);
})
```

As you can see in the code snippet above, we call `.forEach()` just like we would call any other type of loop. We attach the loop to the arr variable (which in the example is an array with a few elements). Then we set up a callback function inside of the argument of the method. Inside of the callback function we call on the individual item(s) or elements that we would like to iterate over inside of the actual loop. After the loop has completed we a variety of options in reference to what we can do after this loop has completed. Usually as a developer we will either want to use the results of the loops or have an idea if what we want to get out of the loop when we originally set it up. This allows the developer to have control of the code and make sure that they are getting the functionality they need with this specific type of loop. 

