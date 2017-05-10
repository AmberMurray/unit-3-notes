# Object Oriented Programming

Example:  

```
waterBottle = {

color: 'purple',
haslid: 'true',
volume: '32oz',
content: 'H2O',
brand: 'Nalgene'

}

spill ()
close ()
open ()
drink ()
fill ()

The state/behavior of the waterBottle:  
open  
close  
content  
volume  
 ```

Instances - this is just one instance of the waterBottle object (or blueprint, or class). The 'blueprint' will show the properties, but not the values (it's the class construct). Instantiation is the initialization of an instance of the master object.

Why OOP?  
Adds a framework to structure your code, organization  
You can make some safe assumptions when you're coding with it  
Code reuse - so we don't have to recreate things over and over  
Reasoning - it's easy to understand a concept or idea as an object   
Design patterns - makes communication about projects easier across the world 🌎

Use cases:  
Games  


# Definitions

Class  
- A class is a template (a factory, a blueprint, etc.) used to generate independent JavaScript objects.  

Constructor
- Each class has the ability to specify a constructor, a function that is invoked upon instantiation -- when an instance when it is created. The constructor can take arguments (which can also be functions) which would be specified upon instantiation with new.  

          ex: class Dog {
                constructor (name) {  
                  * this.name is an instance variable  
                  this.name = name  
                }  

                * bark is the instance method  
                bark () {    
                  some stuff  
                }  
              }  

              * var fido is an instance of Dog  
              var fido = new Dog ('fido')  

Instance  
- To generate the independent JavaScript objects, we use the keyword new. The process is known as instantiation and the objects created become instances.

Instance Variable    
 - Instances can have a property -- or instance variable -- that is created for all instances of the class. An instance variable can be set with a default value or have the value set dynamically per instance. Instance variables allow us to build objects from a template, but identify the differences between them.  

Instance Method  
- An instance method is a function assigned to an instance variable (a behavior an individual instance can perform). (A function that is called on an individual instance.) These methods allow an instance to have behavior based on the properties defined in our instance variables. A method is able to have the same reference to the this variable in its definition.  

This Keyword
- The this keyword references the new instance being created, not the class. This allows us to specify a variable (ex: in this case numberOfFloors) on each individual (ex: building) instance.  

Dependency injection
- Some dependency that is needed by our code and injecting it in is making it available to the dependency somewhere else in our code... basically it makes code available somewhere else

Inheritance  
- This allows the ability for a class to use instance variables and methods from another class. It is usually described as a child class inheriting instance variables and methods from a parent class. Alternatively, it can be described as a subclass inheriting instance variables and methods from a superclass.

Extend Keyword
- We define the inheritance using the extends keyword where the subclass extends from the superclass.

Super Keyword  
- When inheriting a class, the subclass will have access to a new keyword, super. This references the superclass it is inheriting from. It can be used in two ways:

  - Invoking super() calls the constructor on the superclass. This ensures the initial values are set from a super class (See the constructors on OfficeBuilding and ResidentialBuilding). Calling super() in the constructor is required in order to use this in the constructor
  - Calling super.methodName() allows the ability to call a method from the superclass specifically. This allows the ability to override methods while still being able to include the functionality from the superclass (See the addFloor() method of the OfficeBuilding).  

          ex: class Dog extends Animal {  
                constructor {  
                  this.something = some shit here  

                  * super pulls from the Animal class
                  * you can pass arguments in here if the Animal class takes them
                  * you have to call super here in order to have access to anything in the Animal class
                  * you get all of the properties of Animal with super - you can't specify  

                  super()  
                }  
                method () {
                  super.animalMethod()
                }
            }  

          * Dog is the subclass of Animal (the super class)  
          * super.animalMethod() is a method of the Animal class

Interface  
- The vehicle that allows us to interact with things... the similar methods and properties of parent and child classes and the way in which we interact with them. Interface allows us to assume that we can interact with these things.    

Polymorphism  

Getter  

Setter  

Encapsulation  

Object oriented programming   
