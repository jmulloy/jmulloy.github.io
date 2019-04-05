---
layout: post
title:      "'While' Inside of Javascript Loops"
date:       2019-04-05 12:23:51 +0000
permalink:  while_inside_of_javascript_loops
---


Javascript is a common and widely used programming language. Throughout my experience, Javascript was mainly used for the development of SPA or Single Page Applications. Single Page applications are referred to hen a program, app, or website can navigate seamlessly from one page to the next without having the browser conduct a “hard refresh”. For those of you unfamiliar with refreshes, think about when the website you clicked on won't fully load. Your first instinct is to probably hit the refresh button located to the left of the navigation bar in most browsers. You will notice if you were to refresh the page you are reading this blog on the website will make a fresh http request from the server and this will cause all of the data to disappear for a few moments. Think of it as clearing the canvas and allowing new information to be displayed. 

One of the many great things about Javascript is that the language itself can be used to write complex functionality for most of the applications that are built with it. One of those pieces of functionality that I have been working with for a few months now is loops. Looping in programming, in specific within Javascript, is a feature which facilitates the execution of a set of instructions/functions repeatedly while some condition evaluates to true. There are a few different types of loops that can be used. The first one we are going to discuss today is the while loop. Let's take a look at some code. 

```
Var age = 5;

While (age < 10) {

   console.log (“Your age is less than 10”);
   
	 age ++;
	 
}

document.write (“you are now over 10”)
```

Let's break down our code above. Our first line is a standard variable declaration for the variable of age and we have set it equal to 5 meaning our starting is 5, pretty straight forward. Next line you will see the beginning of our “while” loop. We are essentially setting our loop to say while the age variable is less than the number, we want to `console.log the phrase “Your age is less than 10”`. After each console.log we also want to make sure that we work towards exceeded the limit of 10 to exit the loop. This is done by incrementing the integer value of the age variable by 1 each time. This can be seen on the 4th line with `age++`. This loop will console.log the statement as many times as it takes to exceed the number 10 which will be 5 loops. After the 5th loop the final line in the code will run and will return `“you are now over 10”`.

So loops are very useful in programming to prevent repeating large amounts of code when it can ultimately be done with just a few lines of code. This is a basic example but this process can be very useful when working with bigger loops that need to excute hundreds or thousands of times before another action will take place. I hope this blog has been informative and helpful. I plan to follow this blog up with the use of “for” in loops within Javascript. 
