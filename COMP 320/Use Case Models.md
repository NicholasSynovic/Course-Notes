# Use Case Models

## Table of Contents

- [Use Case Models](#use-case-models)
  - [Table of Contents](#table-of-contents)
  - [Overview](#overview)
  - [Use Cases](#use-cases)
  - [Actors](#actors)
  - [Components of a Use Case Diagram](#components-of-a-use-case-diagram)
    - [Figures](#figures)
    - [Terms](#terms)
  - [System Sequence Diagrams](#system-sequence-diagrams)
    - [Message Format](#message-format)

## Overview

- UML is a standard notation for describing object oriented systems
- Use case diagrams show the use cases within the scope of the system and the actors in the environment with which each use case is associated
  - At least one use case narrative for each use case
- Expanded use case narratives are written for every use case corresponding to an external event
  - Captures the sequence of messages from an actor to the system as well as the system's response to each message
  - Reveals the content of the messages
- Use case narratives should be essential
- Diagrams shows graphically what the use case narratives describe
- there is one system sequence diagram for each use case corresponding to an external event

## Use Cases

- A use case is the sequence of actions which occur when an actor uses a system to complete a process
  - Model of a requirement
  - Use case name is a short phrase beginning with a verb
    - Department submits class schedule (an event) -> Submit Department Class Schedule (an Use Case)
  - Each event corresponds to at least one use case

## Actors

- Actors is something which interacts with a system by sending messages or receiving messages to and from the system
  - They play roles with respect to the system
  - They were identified during event analysis
- Initiating Actors initiates a use case via an external event
- A praticipating actor is involved in a use case but does not initiate it
  - Typically recieve outputs from the system

## Components of a Use Case Diagram

### Figures

- Stick Figures represent actors
- Use Cases are represented via ovals
- Associations between an iniaiting actor and a use case is a line with a stick arrowhead
- Association between a participating actor and a use case is a line
- System boundary is shown with a rectangle

### Terms

- Preconditions are conditions which must be true for the the system to begin and produce proper results
- Postconditions are conditions which must be true after the system has produced a result in order to shut down
- Special Requirements are something that is critical to the users acceptance and use of the system
- Alternative flow of events are what the system should do in the case of exceptional conditions or errors
- <\<includes>> always occurs when the use case which includes it occurs
  - Occurs when one use case starts another use case with the same message
- <\<extends>> association depends on a true condition in the use case which it extends

## System Sequence Diagrams

- A system sequence diagram shows the interaction between an actor and the system for one use case scenario
  - Shows:
    - The system
    - Initiating actors
    - Each external system
    - Messages
    - Sequence of messages
- Focuses on the content and structure of the system input
  - Shows repeated or alternative messages
  - Not the place to show the design of the detailed interaction between the user and the system

### Message Format

- Message name followed by a parameter list
- All names begin with a lower case letter
- There are no spaces in a name
- Upper case letters separate words within a name
- Names in the parameter list are separated with commas
