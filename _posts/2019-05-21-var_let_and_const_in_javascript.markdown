---
layout: post
title:      "var, Let, and Const in Javascript"
date:       2019-05-21 13:01:11 +0000
permalink:  var_let_and_const_in_javascript
---


If you have found this blog post you are probably looking for an answer in reference to a question. Hopefully, your question is in reference to setting up variables in the Javascript language. For those of you who might be new to development, variables are used to hold specific values for our program. I think of programming variables in the same way as I would use them in Algebra. You declare a variable and set it equal to value. Seems easy enough right? Well, unlike Algebra there are a few different types of ways to “declare” our variables depending on the need/use of the variable and it also depends on where the variable is being defined within the code of the application. 

We have 3 main variable declaration types: let, var, and const. I will define the use for each one of these types and hope to paint a clearer picture for those of you who might be as confused as I was when I was first getting exposed to Javascript. Ok, enough with the small talk, let's talk about some code. 

The first of the 3 variables I would like to talk about it the <var> variable. Var was the main variable type used before the introduction of ES6. If you are a programmer then I am sure you are aware that the tech stacks we work with are forever evolving and changing for the developers to use and understand. The scope of Var is generally globally or function(ly) scoped. In English this means that if a var declaration is outside of a function then it can be referenced inside the entire application. In the code below I will show you an example of a global declaration and a function declaration 

```
Var greeter = “say Hello World”
function newFunction() {
	Var hello = “hello”
}
```

The let Variable is similar to var in a few ways but it is also rather different than var. Just li,ke var a Let variable can be updated, however, it cannot be redeclared. In the code below I will show you how to update rather than redeclare the value of the let vasriable.  

```
Let greeter = “say Hi”
Greeter - “say Hello”
```

At first, we declare greeter to have an initial value of “say Hi” in a string. Underneath it, you can see that without using the the let variable again we are able to update the variable greeter with a new value by just setting it equal to a new string or value type. 

The final way we can declare a variable within Javascript is with the const declaration. The important thing to remember with const is that it can only be referenced within the scope it was defined. The declaration is what we call “Block scoped” and they can't be updated or redeclared. As I am sure you could guess, we can not give it a new value once we have declared that variable. 

```
Const greeter = “Say Hellow World”
Greeter = “Say Hello computer
Const greeter = “new hello string”
```


After the first declaration for greeter the other 2 lines won't be recognized. They won't update the variable we have already declared in the first line code. 

All of this information can be a bit overwhelming at first. I found that practicing the declarations in repl.it with generic code blocks is the best way to understand/ practice the set up of these variable declarations. 
