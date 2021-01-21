# COMP 371 Panopto Lectures

### B1
* We use languages to deliver some value
* What is the surrounding process that we use to develop software?
	* Waterfall design
		* Everything is done once and that is it
	* Agile process
		* Shorter release cycles and more interaction with the end customer
	* Lightweight Development Process
		* Automated Regression Testing
			* TDD
				* Represent expectations as to how the software should behave
				* Tests are convenient and easy to run
			* Retest every time a feature is added or refactored
		* Refactoring
				* Improve the quality of the code without changing its behavior
					* Meant to improve the quality of it
				* Macro level are nonfunctional requirements
				* Micro level are code smells
			* Continuous Integration
				* Automating the testing and build process

### B2
* Software requirements
	* Software is written to learn a language, solve a problem, or produce an asset
		* All three could be present
	* Functional Requirements
		* Output as a function of input
		* Description of observable behavior
	* Nonfunctional Requirements
		* Test ability
			* Most important nonfunctional requirement
			* Allows testing whether functional requirements are met
			* Good architecture often happens as a side effect such as separating I/O from core functionality
		* Performance
			* Big O
			* Speed
		* Scalability
			* Performance for large data sets
		* Reliability
			* The expected outcome is always the expected outcome
		* Maintainability
			* The software is available to be used at all times
		* Static vs Dynamic Nonfunctional Requirements
	* BUFD vs MVP
		* Big up front design
			* Waterfall, one shot design
			* Risky approach
		* Minimal Viable Product
			* Minimal system outcome to fill a design
			* Less risky approach
### B3
* Software Design Principles and Patterns
	* DRY
		* Don't repeat yourself
		* Automating as much as possible
		* No duplicate code or classes
	* SoC
		* Separation of Concern
			* A concern is an aspect of a system
				* Static concerns
					* Different classes for different things
				* Dynamic concerns
				* To often main has the computational functionality that prevents testing
					* Seperate out computational/ testable code from linker code that handles outputs from different classes and methods
	* SOLID
		* Single Responsibility
			* A class should only hava a single responsibility
		* Open Closed
			* Software should be open for extension but closed for modification
		* Liskov Substitution
			* Objects should be replaceable with instances of their subtypes without altering the correctness of that program
		* Interface Segregation
			* Client specific interfaces are better than one general purpose interface
		* Dependency Inversion
			* One should depend upon abstractions and not concretions
	* Design Patterns that we will later cover
		* Iterator
		* Strategy
		* Composite
		* Decorator
		* Visitor
		* Abstract Factory
		* Observer

### B4
* Programming Language History and Paradigms
	*  Abstraction: Avoid requiring something to be stated more than once; factor out the recurring pattern.
	* Automation: Automate mechanical, tedious, or error-prone activities.
	* Defense in Depth: Have a series of defences so that if an error isn’t caught by one, it will probably be caught by another.
	* Information Hiding: The language should permit modules designed so that (1) the user has all of the information needed to use the module correctly, and nothing more; and (2) the implementor has all of the information needed to implement the module correctly, and nothing more.
	* Labeling: Avoid arbitrary sequences more than a few items long. Do not require the user to know the absolute position of an item in a list. Instead, associate a meaningful label with each item and allow the items to occur in any order.
	* Localized Cost: Users should only pay for what they use; avoid distributed costs.
	* Manifest Interface: All interfaces should be apparent (manifest) in the syntax.
	* Orthogonality: Independent functions should be controlled by independent mechanisms.
	* Portability: Avoid features or facilities that are dependent on a particular machine or a small class of machines.
	* Preservation of Information: The language should allow the representation of information that the user might know and that the compiler might need.
	* Regularity: Regular rules, without exceptions, are easier to learn, use, describe, and implement.
	* Security: No program that violates the definition of the language, or its own intended structure, should escape detection.
	* Simplicity: A language should be as simple as possible. There should be a minimum number of concepts, with simple rules for their combination.
	* Structure: The static structure of the program should correspond in a simple way to the dynamic structure of the corresponding computations.
	* Syntactic Consistency: Similar things should look similar; different things different.
	* Zero-One-Infinity: The only reasonable numbers are zero, one, and infinity.

### B5
* Popularity Indices and Performance Comparisons
	* PYPL
		* Popularity of Programming Languages
			* Based off of Google Searches
				* Most number of searches = more popular
	* TIOBE
		* Based off of Developers and search engines
			* Most number of searches = more popular
	* Github Language Popularity
		* Based off of projects on Github
	* Shootout
		* Compares the languages based on performance on a series of benchmarks 
* These comparisons are only the math portion of choosing a language
	* Often the choice comes down to the human component of programming

### C3
* org.scalatest
	* The only testing suite for Scala that you would use
* com.novocode.juinit-interface
	* Junit testing suite to test Scala code
* Traits
	* A generalization of a Java interface

### C5a
* Defining Domain Models in Imperative and Object-Oriented Languages
	* Basic Type Abstractions
		* Addressing
			* Pointers
			* References
		* Aggregation
			* Structs and Records
			* Arrays
		* Variation
			* Tagged Unions
			* Multiple implementations of an interface
				* Mutable set abstraction
					* Add element
					* Remove element
					* Check for element existence
					* Check if empty
					* Return element count
					* Implementations
						* Preferred
							* Binary Search tree
							* Hash table
							* Bit vector
						* Meh
							* Array
							* Linked list
			* Structural Recursion
				* defining a type in terms of itself, usually involves aggregation and variation
					* A tree interface with implementation classes for leaves and interior nodes
				* Genericity
					* When a type is parametric in terms of one or more type parameters
						* Collections parametric in their element type
							* Can accept any element type as long as it is the same element type

### C5b
* Object oriented Scala as a better Java
	*  Improvements
		* Unified types
			* No distinction between primitives and reference types
				* Int and Integer are mostly the same 
		* Standalone higher order functions
		* Standalone objects
			* Can create an object on the fly without describing it earlier
		* Case classes
			* A lightweight method of creating domain models
		* Pattern matching
			* Basically allows for branching based off of structural matches and binding variable names to the structure you are matching
				* Functional programming benefit
		* Traits
			* Generalization of interfaces and restricted form abstract classes
				* Can be combined and/or stacked
		* Package structure decoupled from folder hierarchy
		* Higher Kinded types
	* Java echoing Scala
		* Lambda expressions
		* Default methods in interfaces
		* Local type inference
		* Streams

### C6a
* Using Scala Traits for Modularity and Dependency Injection
	* For some reason this shit was mute so IDK what was going on

### D1a
* Solving Problems using Built In Types and Behaviors
	* ProcessTree Example solves the problem of prettifying a process list
		* Tab indentation
* Iterators vs List
	* List stores a lot of data in memory all at once
	* Iterators allow for only one piece of data to be in memory at once as well as the calculation to generate the next input
* Package Object
	* Allows for type aliasing
		* Creating custom types that inherit the properties of other types
* Fold can build up a list quickly
* _ is essentially an abstract variable referencing the current index/ value of some list or iterator
* groupBy is a function for finite iterators that returns a map grouped by some key
* Scala infers types
* Mutable objects are called buffers 
* Sbt Stage creates startup scripts for the files 
	* More efficient way of testing and executing scala code
	* Recompiles if you change the build configuration
	* Stored in the target folder 