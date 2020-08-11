---
layout: post
title:      "What Is Self"
date:       2020-08-11 17:54:30 -0400
permalink:  what_is_self
---

Self can be determined differently depending whether you are using it in the definition of a class method or if you are using self inside a instance method. If self is being used in the definition of a class method then self is refering to the class itself, but if used in an instance method it refers to the same object that the method is being called on.

For example, if you make a new class and create a instance method and inside the method body you puts self. Afterwards you create a new instance or object and self will refer to that instance or object the method is being called on. So when you call the method on the new object the method would puts out the actual instance of that object. Also every method that is called is received by an object and the object receiving the call is called the receiver. So if you were to call a method without a receiver, the implicit receiver would be self.

Examples:

> class Dog

>   def show_self
>      puts self *self refers to the object the method is being called on*
>   end
  
> end

 => :show_self 
 
> fido = Dog.new
 => #<Dog:0x00007f87809e96e8> 
 
> fido.showing_self *calling the method on the object returns a Dog instance that is the object*
 =>#<Dog:0x00007f87809e96e8>
 
 
> class Foo

>   def foo
>     "foo"
>    end

>   def bar
>     self.foo *explicit receiver "self" *
>     foo *calls same method on same object but with implicit receiver*
>    end

> end
 => :bar 
 
> obj = Foo.new
 => #<Foo:0x00007f8780988c58>
 
 > obj.foo
 => "foo" 




