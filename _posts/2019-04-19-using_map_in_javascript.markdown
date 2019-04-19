---
layout: post
title:      "Using .map() in Javascript"
date:       2019-04-19 09:08:15 -0400
permalink:  using_map_in_javascript
---


Javascript is probably one of my favorite frameworks/languages I have learned to program in. In my experience/schooling I used Javascript to mainly work with and on the client side of applications. Javascript is one of the more common languages that companies are starting to use and incorporate into their platforms and applications. There all lots of “methods” that can be used within the Javascript language. There is one in particular that I wanted to discuss today and that is `.map()`. 

What is `.map()`? Great question! `.map()` is a method that we can use within our code to create a new array with different data than the existing array. We can use `.map()` to apply a function on every element in an existing array. You will here programmers use the phrase. “`.map(`) through the array.” An easy way to think about .map() is very similar to generic for loop that can be used in Javascript. The for loop is used to execute the same block of code a specified number of times or while a specified condition is true.

Lets take a look at an example below:

```
let newArr = oldArr.map((val, index, arr) => {
 // return element to new Array
});
```

As you can see in the example above, we start out be declaring a new variable which in this case is being called newArray. We set the newArray equal to our old array that has a .map() method called on the end of the array variable. As you can see, our map method is taking in a few arguments (these arguments can vary based on the function or array that map is being used in. For example purposes our method is taking in a value, index, and array. We are then opening up a function where we can tell the method to return whichever data we choose to and then the function is closed out at the bottom. 

Using .map can be very helpful when trying to achieve the functionality of generating a new array by running a function across an entire array of elements. As mentioned before this is very similar to a for loop however the code used in the example above is a shorthand version of using a for loop with the Javascript language. 

