---
layout: post
title:      "What is This?"
date:       2019-03-08 13:16:29 +0000
permalink:  what_is_this
---


We have all seen and used the word "this" while working within the Javacript programming language but what does "this" even mean? The word this can be used in a variety of different 3ways within the english language as well as within programming. The value of "this" differs depending on how a function is invoked (the call site), so we can’t know the value of this just by looking at the function itself, but we need to know the context in which the function is invoked. Functions are used to figure out what the context of this is based on the actual function itself or sometimes lack there of. Lets take a look. 

The first snippet you will see is what allows ut to refer to this as the global window. The highest level/value that this can have within an application itself. In modern web browsers, the global window refers to the browser itself. if you were to run a basic console.log in the console of the browser on a blank web page like so, ```console.log(this)``` , this will log out the window itself since it is logging at the highest level of the application. This however can differ when this is referenced inside of different functions. 

Inside a standalone function this will refer to gthe global windown again. 
```
function foo() {
	console.log(this)
}

foo()
```

The next case for using this is inside of an object method. Object methods are properties of objects within the Javascript language. Inside of this method, this will refer to the object on which the method is called.
```
let cat = {
	name: “Josh”,
	breed: “Himalayan”,
	speak: function () {
		console.log(`${this.name} says MEOW!`)
	}
}

dog.speak()
```
In this particular method the :this: inside this console.log refers to the cat object that the method is beiong called on. 

This can also be called inside of a function within another function. This is where things can get a little tough to understand/follow. In most cases "this" inside of a function within a function will always be traced back outside of the internal function to the global window. However with certain object methods the "this" can refer to the glabl window and not the trace of the functions that have been defined this far. 

As Youll see throughout this post I have documented alot of different ways "this" can be used and a little bit of a better understanding of how to find the value of this depending on where it is being used. 

* You can use bind(), call(), and apply() to set the context of the “this” keyword.
* You can use bind(), call(), and apply() to set the context of the “this” keyword.
* In a function that is not tied to an object directly (including a function inside a function), “this” will refer to the global object.
* If using “strict mode”, “this” will be undefined.
* Arrow functions do not define their own context for this. Instead, “this” will refer to whatever context is defined by the parent context.
* Inside an object method, “this” will refer to the object that is receiving the method call.
* Outside of any function, “this” refers to the global object, which, in the case of a web browser, is the window.
