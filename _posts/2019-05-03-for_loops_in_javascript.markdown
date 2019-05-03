---
layout: post
title:      "For Loops in Javascript"
date:       2019-05-03 13:32:36 +0000
permalink:  for_loops_in_javascript
---


If you have found access to my blog posts then I am sure you will have noticed that we have covered almost all the major loop types that can be found and ised within the Javascript Language. I would like to take some time to briefly go over what loops are, why we can use them, and then ultimately what the for loop can be used for. Loops are a great way to apply a DRY or Do Not Repeat Yourself principle in coding. They allow developers to write a block code that will continuously run until a certain condition is met or a specific number of times. For Loops can be very useful when a developer wants run a block code a certain number. Lets take a look at some code below and then we will break it down  line by line. 

```
Var answer = 0 
Var start_value = 1
Var end_value = 11

For ( start_value, start_value < end_value, start_value ++) {
	Answer = answer + start_value;
}
console.log(“answer=” + answer);
```

As you can see starting with the first 3 lines of code we simply decalrwed a few variables using var. We have 3 variables that we can now access inside of the for loop underneath them. We have an answer, start_value, and an end_value. To start our for loop we first need to get our method set up which we do by setting up for followed by a group of parenthesis(). Lets take a look at what is going on within the parenthesis. The first value we see is just the starty_value and this is executed once before the code block gets executed. The second argument in the parenthesis defines the condition for the coding block. Which as we can see we want this loop to run as long as the start_value is less than the end_value. The last value we see is start_value++, this is ran after the code block has been executed which in this case we want to increase the value of the start_value variable by 1 each time the code block is ran. 

Now after the loop is set up with our “conditions”, we wil need something to happen so the loop can continue running until the arguments have been met. The code block in the example above will take the value of our answer varaible and add it to whatever the value of the start_value variable is after each code block has been executed in the loop. To help make this a little easier, our answer variable has an initial value of 0 to start, after the first loop we will add 0 + 1 and our new Answer will be equal to 1. The code block will run again adding the 0+2. This will continue to happen as long as the start value is less than the end value. After 10 iterations in the loop the loop will end since the start value will no longer be less than the original end_value we declared before the loop. 

