# Design and Sequence Diagrams

## Table of Contents

- [Design and Sequence Diagrams](#design-and-sequence-diagrams)
  - [Table of Contents](#table-of-contents)
  - [Intro](#intro)
  - [Design](#design)
  - [Types of Relationships](#types-of-relationships)
    - [Inheritence](#inheritence)
  - [Fundemental Concepts](#fundemental-concepts)
    - [Messages](#messages)
    - [Design by Contract](#design-by-contract)
    - [Patterns](#patterns)
      - [Facade](#facade)
      - [Creator](#creator)
      - [Expert](#expert)
      - [Singleton](#singleton)
    - [Interaction Diagrams](#interaction-diagrams)
      - [Collaboration Diagram](#collaboration-diagram)
      - [Sequence Diagram](#sequence-diagram)

## Intro

- Object Oriented designs can rely on these diagrams to provide a roadmap to completion
  - Make sure all requirements are implemented
  - Allows for independent development and tests
- UML is the design tool of these diagrams
  - Complete Objects are documented with Design Class Diagrams
    - These are the static models of the system
  - Collaboration of multiple objects is done with Sequence Diagrams
    - These are the dynamic models of the system doing something

## Design

- Design is important because it is a description that is sufficiently complete and accurate to assure that the solution can be constructed
  - Includes performance
- Design assigns responsibility to objects
  - It is an obligation to another object to make sure that it works
  - Needs to know its:
    - Attributes
    - Associated objects
    - Known operations

## Types of Relationships

### Inheritence

- The derived class is the base class
- The base class can be a derived class
- The derived class can replace the base case if need be

## Fundemental Concepts

### Messages

- Different systems or components of a system send messages between each other to ensure their visibility to other parts of the system
  - Individual components do not need to validate their own existence
    - They need to validate others

### Design by Contract

- When a component or system recieves a message, it is obligated to complete some task regarding the state of that message
  - Involves pre and post conditions
- Requirements:

1. Check if the precondition is true

- Can be done before system execution, during, or both

2. Every postcondition is true

### Patterns

#### Facade

- Problem:
  - Who should be responsible for handling a system operation message from an actor?
- Solution:
  - Assign this responsibility to an object representing the system as a whole

#### Creator

- Problem:
  - Who should be responsible for requesting the creation of a new object?
- Solution:
  - Assign this responsibility to a class which is in some way closely involved with the class

#### Expert

- Problem:
  - What is the most basic principle for assigning responsibilities to objects?
- Solution:
  - Assign the responsibility to the class which has the information necessary to fulfill it

#### Singleton

- Problem:
- Solution:

### Interaction Diagrams

- Shows collaboration between objects

#### Collaboration Diagram

- Follows the conventions of a domain model
- Shows the availible interactions of an object as well
- Shows all messages that could be sent

#### Sequence Diagram

- Messages are shown top to bottom in the order that they appear
- Only shows messages between actors and the system
