---
layout: post
title:      "Object, Classes, Instances..."
date:       2018-07-24 12:21:21 -0400
permalink:  object_classes_instances
---

Objects, classes, methods. What are they? what do they do? how are they Used? Classes are designed to hold different pieces of information just like a blueprint. Some of which are only used for that specific class where as others can be used within different methods. For example we can use the Dog Class to store different pieces of information about our dogs as well as create new instances of our dogs. This information can differ between all of our dogs that we create. 

Lets say we create 2 new dogs using our Dog Class. The first is named "Doggo" and the other is named "Pupper". Both Doggo and Pupper are OBJECTS of the Dog Class even though their information isnt the exact same. Both dogs should have the same abilities such as run, walk, jump, bark, etc. However their attributes of what makes them a dog will be different (such as height, breed, name, etc). the abilities that I have listed above will be the INSTANCES of the Dog class. Which the Instances we have defined within the Dog class are available for any of our Dog objects to use within the class. 

There are a few differences between Class and Instance methods, lets take a look and see what separates them from each other. Most Class Methods are defined by using "def self.method_name" and they are used when not dealing with in an iniividual instance of that class. An instance method on the other hand requires a new instance of the class to be created in order to execute the code. Using the Example from Above. I creat a new instance of the Dog Class named Doggo, I would use the Instance method of #bark to teach Doggo how to bark. 

Classes are also known as Objects within Ruby. This means any class method that is defined only exists within that class in which they are defined, or within the object. You can use the "self" to define a class method because it will always refer to the current object/class that you are working inside of. Now if we wanted to define a method that was an instance of the class we could have a bark method (in reference to our previous example) that would teach Doggo how to bark. We will only be able to call on the instance of bark within our Dog class. However we can always reference another class by calling on it within a different class. 

In conclusion, Class methods are what define our objects or classes within our program. Instance methods are used to help define methods that can be used to give our objects in our class objects (in this case dogs) different attributes. 

Coding Example:

```
class Dog
attr_accessor :name

@@all = []

def initialize (name)
@name = name
end

def self.all
  @@all
end

   def name 
      @name
   end


   def bark
     puts "woof"
  end


end
```


```
doggo = Dog.new("doggo")

doggo.name
#=> "doggo"


Dog.all
#We call the class of Dog on the class method of .all because we are wanting to pull ALL instances/objects of the dogs that we have created inside of our Dog class. Class methods can only be called on the class in which it is defined in. 
```

```
doggo.bark
# => "woof"
```





