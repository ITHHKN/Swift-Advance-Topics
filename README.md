# Swift-Advance-Topics

IOS Basic Concepts : 


#1- Closure 
Closure are self-contained blocks of functionality that Group and executes together, without creating a named function

1.1 - Global Functions : Closure that have a name and do not capture any value.
1.2 - Nested Functions : Closure that have a nice and can capture value from their enclosing function. 
1.3 - Closure Expression : Unnamed closure written in lightweight syntax that can capture values from their surrounding context.


#2 - High Order functions
High order functions are simply functions that operate on other functions by either taking a function as an argument or returning a function. 


1.1 - Sorted : Call on array & sort all data as ascending order 
1.1.0 - Sorted By : Specify exactly how we want to sort the array sorted(by:)

1.2 - Map : It iterates the array and changes each elements of array based on the closure passed to the method 

1.3 - ForEach : Will iterate through all elements in an array and will not return anything  

coins.forEach { (coin) in 
	print("\(coin)$", terminator: " “) 
}


1.4 - Filter : Will return an array that has only elements that pass your filter specified in your closure

let numberLessThanFive = number.filter {$0 < 5}


1.5 : Reduce - Will allows you to combine all the elements in an array and return an object of any types
 
let sumOfAllNumbers = numbers.reduce(“”) { $0 + string ($1) }

1.6 : FlatMap - Converts 2D array into one dimensional array 

1.7 : CompactMap : Will iterate through all elements in an array and will return an updated array only with the elements those satisfied the condition


#3 : Enumeration 
3.0 - an enum (short for enumeration) is a user-defined data type that has a fixed set of related values.


Link : programiz.com/swift-programming/enum
https://www.programiz.com/swift-programming/associated-value-enum


#4 : Structure : value type
- Most important differences between structures and classes is that structures are always copied when they’re passed around in your code, but classes are passed by reference.

Class : Reference type 

#5 : Struct Vs Class

Struct : Each time assign the object copy a new object and lost old values
Class : Each time assign the object copy the old object as well 

Listed example below : 

Link : https://www.avanderlee.com/swift/struct-class-differences/




#6 : init and super.init

https://stackoverflow.com/questions/36916788/swift-difference-between-init-and-super-init



#7 : Codable 
https://www.hackingwithswift.com/articles/119/codable-cheat-sheet


#8 : Concurrency 
Use async to mark a function that runs asynchronously.



#9 - Equatable & hashValue 

Equatable is a protocol that allows two objects to be compared using the == operator. The hashValue is used to compare two instances
programiz.com/swift-programming/equatable 

#10 - First-Class Functions
functions can be stored in constants and variables
functions can be passed as arguments to other functions
functions can be returned by other functions

#11- Functional programming languages : 
Functional programming languages are specially designed to handle symbolic computation and list processing applications

#12 - List Processing
List processing is a list of programming codes, including abstract data structure, used to calculate specified variables in a certain order. A value may repeat more than once.


#13 - LLVM compiler 
LLVM is a set of compiler and toolchain technologies that can be used to develop a front end for any programming language and a back end for any instruction set architecture
Swift is a successor to both the C and Objective-C languages. It includes low-level primitives such as types, flow control, and operators. It also provides object-oriented features such as classes, protocols, and generics, giving Cocoa and Cocoa Touch developers the performance and power they demand.
https://developer.apple.com/swift/



#14 - Strong and Weak References
https://www.programiz.com/swift-programming/strong-weak-reference


#15 - Typealias
programiz.com/swift-programming/typealias


#16 - tuple : 
Group of different values and each value inside tuple is different data type 

#17 - Generics : 
Write code that works for multiple data types


#18 - Type inference
Swift is a statically typed language, meaning that the type of every property, constant and variable that we declare needs to be specified at compile time but due to support type inference assign value to property , compiler figure out on run time 

#19 - Protocols
A protocol is an interface, that is, it contains abstract methods, constants, and variables. Protocols provide shared functionality between classes. You can implement multiple protocols.

#20- Abstract classes & methods
Abstract classes cannot be instantiated, but they can be subclassed. An abstract method is a method that is declared without an implementation (without braces, and followed by a semicolon)

#21- Can object be nil in objective-c and swift : Object-c Yes but in swift only optionals 

#22- Subscripts : Access the elements of a collection.


#23 - optionals : type that can store nil value


#24 - Name two types of data structure for memory allocation.
- Stack & heap memory 


#25 - Stack : FIFO memory structure
reference of portion of local variable 
parameter of reference type  ﻿ ﻿

Heap : 
Contain random non lined objects store in memory so any random object to be allocated or released in a random order  

Stack is used for static memory allocation, Heap is used for dynamic memory allocation.
Link : https://manasaprema04.medium.com/memory-management-in-swift-heap-stack-arc-6713ca8b70e1

#26 - Types : Use built-in named and compound types.
named types: classes, structures, enumerations
compound types: type without a name (Int, (Int, Int))

#27 - difference between NSArray and NSMutable?
NSArray : when you dont want to resize or change data store in array
NSMutable : when you want to add, remove and change data in array 


#28 - Dynamic method resolution   :Single method which can be applied to solve multiple problems. 
Ex: Consider Shape is an interface and has method name draw. you have Rectangle and Circle classes implements Shape Interfac

#30 - Ways to pass data from one controller to another 
1 - transition 
2 - protocols 

#32 - inout parameters : inout	
All variable used as function params are constant variables , you can’t change them but if you use inout you will be able to change them without creating new variable 

#33 - Mutating methods
You created a structure as constant so all the properites of methods are constant properties , so if you want to change any constant struct property you can use keyword mutating , you will be allowed to change the value of property 

#34 - GCD : Grand Central Dispatch : low-level API for managing concurrent operations ( multi-tasking with sync and async options ) 
https://medium.com/@nimjea/grand-central-dispatch-in-swift-fdfdd8b22d52

#34 - Auto Layout? 
-System in the xcode that dynamically calculate the size and position of all the views based on constraints places on the view 

#35- Persistent core data : Data storage provided by the apple
Storing any type of data to disk so that the same data can be retrieved without being altered when the user opens the app next time

#36- Difference between bounds and frame
Frame refers to the coordinate system of the view's container (parent view). Bounds refer to the own coordinate system of the view.


#37 - What is a singleton?
A design pattern in programming where you can only use one instance per class. This instance is called a "shared instance".


#38 - What is a design pattern?
These are solutions to programming problems like an OOP pattern implemented in the right situation.
provides a general reusable solution for the common problems that occur in software design.


#39 - delegate pattern
A design pattern that enables a class or structure to hand off (or delegate) some of its responsibilities to an instance of another type


#40 -  category in Swift - extend the feature of class in swift is know as extension and object-c as category 

Best to learn : 
1- https://www.programiz.com/swift-programming
2- https://www.swift.org/getting-started/
3 - https://www.ideamotive.co/ios/interview


Interview : 
https://www.hackingwithswift.com/interview-questions

