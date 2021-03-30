# Database Operations on Objects

## Table of Contents

- [Database Operations on Objects](#database-operations-on-objects)
  - [Table of Contents](#table-of-contents)
  - [Databases](#databases)
  - [Three Tiers of System Architecture](#three-tiers-of-system-architecture)

## Databases

- The Singleton pattern produces a single, globally visible object to act as this interface
  - Creating a globally accessible database connection in order to prevent the unnecesary need for multiple connections to the same database
- A data base is a systematically partitioned, reusable, integrated collection of data which can be shared by many individual users as well as by multiple applications.
  - Provide the following benefits
    - Logical independence of the data and
    - Physical independence of the data
    - Integrity constraints
    - Security
- Objects should be stored in an object database
  - Most of the time they are stored in a relational database
    - A relational database is organized into tables, rows and columns
- Databases need to be able to perform CRUD, store, and load data
- At the beginning of a system, the database should be spun up
  - Before the database closes, the database should be safely shut down

## Three Tiers of System Architecture

1. Presentation
2. Business
3. Storage

- This layer should remain seperate from all of the other layers
- None of the layers can operate without this layer
- If integrated with other layers, complexity and security issues can arise
