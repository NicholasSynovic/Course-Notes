# Domain Model

## Table of Contents

- [Domain Model](#domain-model)
  - [Table of Contents](#table-of-contents)
  - [Domain Model](#domain-model-1)
  - [Procedure for Object oriented Systems Analysis](#procedure-for-object-oriented-systems-analysis)
  - [Generalization Specialization Hierarchies](#generalization-specialization-hierarchies)
  - [System Operation Contracts](#system-operation-contracts)
    - [Creating System Operation Contracts](#creating-system-operation-contracts)
    - [System Postconditions](#system-postconditions)

## Domain Model

- Has many names
  - Domain model
  - Class diagram
  - Key System Components
  - Data Structure Diagram
  - Relational Data Design
- Only function is to provide a static model showing the conceptual scope of the entire system
  - Created one at a time to ensure that every object represented in the domain model has the proper associations, attributes, and concepts relevent to it and it alone
  - Contracts are created at the end of this process which are derived from Use Case Narratives
    - Contracts specifies what changes in the state of the system are required after the system operation has completed successfully

## Procedure for Object oriented Systems Analysis

1. Identify the business events and make an event table
2. Identify the use cases and produce a use case diagram for the system
3. Write a use case narrative describing the system's reposne to each business event
4. Draw a system sequence diagram for each use case scenario
5. Produce a domain model showing the concepts, attributes and associations in the problem domain of the system

- A concept is an abstraction of a thing
  - An object
  - Offen are nouns or noun phrases describing the problem domain
- An attribute is a characteristic of a concept which may have a value
  - An object's variables
  - Adjectives
- An association is a significant connection between concepts
  - One to one, one to many, reflexive, whole to part
  - Never assume association
  - Multiplicity
    - The number of instances of a concept which can be associated with one instance of another concept
    - One to many relationship
    - Must mark multiplicty using the value near the concept
  - Whole to Part
    - Aggregation
      - Multiplicty between two or more objects is greater than or equal to 1 on both sides
    - Composition
      - Multiplicty between two or more objects is greater than or equal to 1 on one side

6. Write a contract for each system operation

## Generalization Specialization Hierarchies

- Classifies a type of concept into its subtypes
  - Each instance of a subtype must also be an instance of its supertype
  - Subtypes have the same set of attributes as their supertypes
    - These are not listed in the domain model

## System Operation Contracts

- A system operation is an operation which the systems carries out in response to a system input
  - They both have the same name

### Creating System Operation Contracts

- Identify each system operation in a system sequence diagram
- Write the responsibilities of that operation in the contract
- Write the proeconditions in terms of the required changes in the domain model
- Add the postconditions and exceptions

### System Postconditions

- What instances of concepts must be created or deleted?
- What attributes have their values modified?
  - To what new values?
- Which instances of associations must be added or deleted?
- All postconditions use the past tense and a passive voice
