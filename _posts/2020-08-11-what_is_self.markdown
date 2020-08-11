---
layout: post
title:      "What Is Self"
date:       2020-08-11 21:54:29 +0000
permalink:  what_is_self
---

Self can be determined differently depending whether you are using it in the definition of a class method or if you are using self inside a instance method. If self is being used in the definition of a class method then self is refering to the class itself, but if used in an instance method it refers to the same object that the method is being called on.

For example, if you make a new class and create a instance method and inside the method body you puts self. Afterwards you create a new instance or object and self will refer to that instance or object the method is being called on. So when you call the method on the new object the method would puts out the actual instance of that object. Also every method that is called is received by an object and the object receiving the call is called the receiver. So if you were to call a method without a receiver, the implicit receiver would be self.

