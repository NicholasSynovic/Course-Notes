# Design Class Diagrams

## Table of Contents

- [Design Class Diagrams](#design-class-diagrams)
  - [Table of Contents](#table-of-contents)
  - [Intro](#intro)
  - [Visibility](#visibility)
  - [Steps to Design an Object Oriented System](#steps-to-design-an-object-oriented-system)
  - [Cohesion](#cohesion)
  - [Coupling](#coupling)
  - [The Law of Demeter](#the-law-of-demeter)

## Intro

- Steps for diagrams of a system:

1. Interaction diagrams of a system are dynamic models of object oriented software
2. Design class diagrams are based off of interaction diagrams

- Static model of a system
- Only shows how the different classes of a system interact and associate with one another
  - Classes and class hierarchies
  - Attributes
  - Operations
  - Whole-to-part associations
  - Qualified associations
    - These are associations between two objects that use a qualifier to select objects at either object
      - Qualifiers are a known variable that are unique between the two classes

3. Message composition diagrams are created that show how classes pass around information

- By now, the business layer of the application has been built

## Visibility

- Visibility is the ability for an object to reference another object
  - Four types

1. Reference Visibility

- Client object has reference to the server object

2. Parameter Visibility

- An object is provided a message by its parameter

3. Local Visibility

- Obtains visibility by declearing an object within itself

4. Global Visibility

- An object is required to have visibility of another

## Steps to Design an Object Oriented System

1. Produce an interaction diagram for each system operation identified during analysis.
2. Produce a design class diagram showing the operations from the interaction diagrams.
   1. Identify classes with their behavior.
   2. Add inheritance to the class diagram.
   3. Add associations to the class diagram.
   4. Create a final class diagram with
3. Specify the signature and the
algorithm for each operation.
4. Design the graphical user interface.
5. Define the interface to the presentation layer.
6. Define the interface to the storage layer.
7. Place the classes in packages.

## Cohesion

- Needs the Expert pattern
- Needs high cohesion
- Measures how strongly related and focused all of the associations are
  - Measure of attributes and diversity of classes

## Coupling

- Want low coupling
  - Sublcasses are a source of low coupling
- Measure of how much a class is connected to, has knowledge of, or relies on other classes

## The Law of Demeter

- A class should be able to send messages only to:
  - Itself
  - An object to which it contains a reference
  - A parameter of one of its methods
  - One of its local objects
  - A class
