# COMP 313

## Week 7
### Project 3
* Visitor is generic on type interface Result
* Outline and StrokeColor are decorators and Polygon accepting classes
	* Anything that is drawn on the Android canvas require that these decorators exist
	* Point and Location are decorators
		* Points are meant to be a shape without an outline
			* It is a circle of zero radius
		* Outlines create polygons from shapes
	* Decorators have a child object that they work with
* Shape is the primary interface for all the shapes that can be drawn on the canvas
	* Not generic, but has a generic method
		* Told by the angle brackets around the type
* Fixtures is a class that provides static shape structures that are used in tests
### UML
* Class Name in the top box
* Attributes below that
	* Instance variables
* Methods below that
* Attributes, parameters, and methods often have - or + in front of them
	* Relationships between classes shown with arrows
		* Inheritence done with a solid arrow line
		* Implements is done with a dashed arrow line
		* If a class depends on another, the dependency points to the parent
		* Associations are done with one arrow pointing from one class to another
		* An open diamond shows ownership of one class
		* A closed diamond shows that one class is part of another one
## Week 9
### Principles of OO Design
* SOLID
	* S - Single Responsibility Principle
	* O - Open Closed Principle
	* L - Liskov Substitution Principle
	* I - Interface Segregation Principle
	* D - Dependency Inversion Principle
* You don't want software to break when you try to change it
* Single Responsibility
	* Every method in a class has one responsibility
		* A responsibility is defined as a reason to change
		* Split classes
* Open Closed Principle
	* Software should be open for extension, but closed for modification
		* You can add more methods by implementing a class, but you should not be able to adjust the source code of the original class
			* Use interfaces and visitors
* Liskov Substitution Principle
	* Subclasses should be exactly substitutable
		* If the parent class has a method, the subclass should also have that method and a return type for that method
		* Subclasses need the same base traits as the parent (arguements, methods, parameters, return types)
* Interface Segregation Principle
	* Clients should not be forced to depend on methods they don't use
		* Making a class do everything is often times not beneficial to the end user
			* Divide the class into its necessary bits and take whatever is left and make their own classes from that
* The Dependency Inversion Principle
	* High level modules should not depend on low level modules
		* Abstract the low level code from the high level code
			* Having low level code in a high level method is fine, but having a high level module depend on a low level module is not
* Benefits of SOLID
	* Low coupling between modules
	* High cohesion
		* Many small pieces can be stacked together to make a larger piece
	* Encapsulation
		* Modules are encapsulated into their own parts
### Android Application Development
* Android Framework
		* Android is built on the Linux kernel
			* Then libraries on top of that
				* Frameworks on top of that
					* Applications finally on top
		* Each app is given a unique Linux user ID
* An activity is the entry point for interacting with the user
* Android Activity Life Cycle
	* Starting -> Running -> Paused -> Back to Running OR Stopped -> Back to Running OR Destroyed IF Stopped
* Kotlin is a possible language to program Android Apps
* Java Features
	* Lamba expressions
		* Treat methods as variables
		* Allows methods to have custom logic based off of an input
	* Parallel Operations (streams)
		* Can process information across multiple threads
	* Concurrency
	* New Date and Time API
	* Better Security 
## Week 11
### Design Patterns
* Patterns are classified by purpose
	* Creational - create objects
	* Structural - composition of classes
		* Adapter
			* Translates on interface for a class into a compatible interface
				* Could transfer data from one type to another to allow for a system to work
			* Class adapter specifies its requirements via an interface
				* Implements and extends methods
			* Object adapter can extend, override, and delegate methods between classes
			* A wrapper
		* Facade
			* Provides an interface to a larger body of code in a simpler manner
			* An adapter changes data, a facade does not
	* Behavioral - interactions of classes
		* Observer
			* Allows different clients to know if an object changes state
			* Minimizes coupling between classes
		* State
			* Resembles the Strategy pattern
			* Allows for an object to change its behavior at runtime given some input
		* Command
			* Get a list of objects at a given state and execute on those objects at a latter time
### Model View Adapter/ Controller
* MVC allows for the UI and the backend to be seperate from one another
	* Allows for the UI to be adjusted without the backend becoming depricated and vice versa
* MVA sits in between the model and the view and has the logic for both of them
	* Listener to both the model and the view
	* Advantages
		* All of the complex logic is in a centralized location
### UML State Diagram
* State diagram is used to describe the states of various systems
* UML state machine is an object oriented state diagram
