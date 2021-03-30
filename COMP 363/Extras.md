# Extras

## Table of Contents

- [Extras](#extras)
  - [Table of Contents](#table-of-contents)
  - [Note](#note)
  - [Data Stores and APIs](#data-stores-and-apis)
    - [What is NoSQL?](#what-is-nosql)
    - [Resources](#resources)
  - [Design Mockups](#design-mockups)
    - [Application Appearance](#application-appearance)
    - [Hi-Fi Mockups](#hi-fi-mockups)
    - [Hi-Fi Prototypes](#hi-fi-prototypes)
    - [Low-Fi mockups](#low-fi-mockups)
    - [Rapid Prototyping](#rapid-prototyping)
    - [Resources](#resources-1)
  - [Version Control](#version-control)
    - [Intro](#intro)
    - [What is it?](#what-is-it)
  - [Node.js and Express](#nodejs-and-express)
    - [Resources](#resources-2)
  - [Node.js and MongoDB](#nodejs-and-mongodb)
    - [Resources](#resources-3)
  - [Node.JS and NPM](#nodejs-and-npm)
    - [Resources](#resources-4)
  - [Array and LinkedList Datastructures](#array-and-linkedlist-datastructures)
    - [Array Datastructure](#array-datastructure)
    - [LinkedList Datastructure](#linkedlist-datastructure)
    - [App to Memory](#app-to-memory)
    - [Process and Memory Usage](#process-and-memory-usage)
  - [Basics](#basics)
    - [Binary Search Algorithm](#binary-search-algorithm)
    - [Big O Common Runtimes](#big-o-common-runtimes)
    - [Traveling Salesman Problem](#traveling-salesman-problem)
  - [Big O Part 2](#big-o-part-2)
    - [Average Case vs Worst Case vs Best Case](#average-case-vs-worst-case-vs-best-case)
    - [Resources](#resources-5)
  - [Binary Search Tree Datastructure](#binary-search-tree-datastructure)
    - [Issues](#issues)
    - [Implementation](#implementation)
  - [Divide and Conquer Algorithm](#divide-and-conquer-algorithm)
    - [Resources](#resources-6)
  - [Hash Table Datastructure](#hash-table-datastructure)
  - [Quicksort Algorithm](#quicksort-algorithm)
    - [Resources](#resources-7)
  - [Recursion](#recursion)
    - [Cost](#cost)
  - [System Memory Structure](#system-memory-structure)
    - [System Components](#system-components)
    - [Processes](#processes)
    - [Kernel and Communication](#kernel-and-communication)
    - [Kernel and Process Control Blocks](#kernel-and-process-control-blocks)
    - [Process Manager](#process-manager)
    - [Kernel and the File System](#kernel-and-the-file-system)
    - [CPU and the Kernel](#cpu-and-the-kernel)
  - [Observer Pattern](#observer-pattern)
  - [PubSub Pattern](#pubsub-pattern)

## Note

- These documents were meant to be read in a specific order. I did not do that.

## Data Stores and APIs

- Databases allow for us to hold persistent data
  - MongoDB is a NoSQL database
  - We can use JS to write CRUD SQL commands

### What is NoSQL?

- Works like SQL, without SQL commands

### Resources

- [MongoDB](https://www.mongodb.com)
- [MongoDB - Documentation](https://docs.mongodb.com/manual/installation/)
- [MongoDB Driver - up to v3.6](https://mongodb.github.io/node-mongodb-native/)
- [MongoDB Driver - latest](https://docs.mongodb.com/drivers/node/a)
- [Robo 3T](https://robomongo.org/)
- [Robo 3T - Download](https://robomongo.org/download)

## Design Mockups

### Application Appearance

- A prototype or mockup helps us plan and visualise an application's appearance and interface
  - High or low fidelity
  - Mockups do not specify behaviro
  - Prototypes are interactive software in their own right

### Hi-Fi Mockups

- Look like the finalized product
- Represent and visualise the appearance of the user interface
  - Allows us to test colors
- No actual interaction

### Hi-Fi Prototypes

- Act as an interactive application
  - Not the final application
  - A working simulation
- Rapid, working example of functional components of an app
- Code often sufficient to simulate and replicate results for a given action and scenario
  - No persistent data storage
  - May simply simulate and demonstrate action of saving the data
- Can be time consuming to produce

### Low-Fi mockups

- Rough sketch or outline
  - Referred to as wireframes
- Their simplicity can offer an inherent utility and speed of creation
- Not trying to recreate the exact look and feel of an app
  - More interested in layout of visual components and elements
- Quick to modify and update

### Rapid Prototyping

- Provides quick examples of an application's design
- Iterative design helps encourage feedback early in the design process
  - Consider what needs to be prototyped early and often
    - Usually the most common design elements and interactions
    - Work out how different componenets interact with one another
  - Choose your iterations for prototypes

### Resources

- [HTML, CSS, JavaScript, Bootstrap](http://getbootstrap.com/)...
- [Adobe Photoshop](http://goo.gl/GsIYY0)
- [Illustrator](http://goo.gl/9K8Kfw)
- [Sketch](http://bohemiancoding.com/sketch/)
- [Proto.io](ttps://proto.io/)
- [Flinto](https://www.flinto.com/)
- [framer](http://framerjs.com/)
- [Google Drawings](http://goo.gl/qPRCfG)
- [XCode Interface Builder](https://developer.apple.com/xcode/interface-builder/)
- [Apple’s Keynote](http://keynotopia.com/guides/)

## Version Control

### Intro

- Ensures tthat we keep track of changes, updates, contributions, suggessted modifications
- Uses exploaratory coding style
  - Involves researching, learning, checking what does and does not work correctly
  - Often used methodology for coders and small groups
- Version Control leads to many small changes and updates in the code

### What is it?

- Allows for comparisons to be made across different versions of the project or file
- Maintains defined, labelled points in our code
- Can easily refer back to them or revert to an earlier state if needed
- Important tool for collaborative work with other developers
- Several VCS tools exist
  - Subversion, Mercurial, Git
    - Git is currently the most accessible

## Node.js and Express

- Express is a web application framework used to create HTTP applications

### Resources

- Express
  - [Express web framework](http://expressjs.com/)
  - [API Reference](http://expressjs.com/en/4x/api.html)
  - [ExpressJS](http://expressjs.com/)
  - [ExpressJS body-parser](https://github.com/expressjs/body-parser)
- Node.JS
  - [Node.js home](https://nodejs.org/en/)
  - [Node.js - download](https://nodejs.org/en/download/)

## Node.js and MongoDB

- Express used for server hosting and routing
  - Can also read and write JSON from and to the server
- MongoDB allows for persistant data to be stored in the cloud
  - NoSQL based
  - Document oriented database
    - Stores objects in collections
      - No tables and rows, only documents of information
    - Stores these documents in the BSON format
      - Binary JSON
  - Three Levels of abastraction
  - Can be accessed via Node.JS with `mongoose`

1. Database

- One database per app

2. Collection

- A grouping of similar pieces of data

3. Document

- A single item in the database

### Resources

- MongoDB
  - [MongoDB - For Giant Ideas](https://www.mongodb.org/)
  - [MongoDB - Getting Started (Node.js driver edition)](https://docs.mongodb.org/getting-started/node/)
  - [MongoDD - Getting Started (shell edition)](https://docs.mongodb.org/getting-started/shell)
- Mongoose
  - [MongooseJS Docs](http://mongoosejs.com/index.html)
- Node.js
  - [Node.js home](https://nodejs.org/en/)
  - [Node.js - download](https://nodejs.org/en/download/)
- ExpressJS
  - [ExpressJS](http://expressjs.com/)
  - [ExpressJS body-parser](https://github.com/expressjs/body-parser)

## Node.JS and NPM

- Node.JS is a JavaScript runtime environment designed to be ran outside of the browser
  - Turns JS from a web tool to a backend programming tool
  - It is fast
- Node.JS uses an event driven architecture
  - Better suited for I/O bound events not CPU bound events
    - Uses I/O callbacks to allow for thousands of I/O operations to happen at once
- NPM is the Node.JS package manager
  - Can also upgrade Node.JS

### Resources

- NPM
  - [npmjs](https://www.npmjs.com/)
- Node.JS
  - [Node.js home](https://nodejs.org/en/)
  - [Node.js - download](https://nodejs.org/en/download/)

## Array and LinkedList Datastructures

- Data is stored with an address in the computer's availible memory
  - This address will be ready for both the system and the application
- To store multiple pieces of data in an organized manner, we need a data structure

### Array Datastructure

- Different implementations can yield different benefits and comprimises
- A basic array structure can
  - Add data
  - Move data
  - Manage data
  - Read data
  - Resize data
- Arrays can be bounded or unbounded by size
- Reading is O(1)
- Insertion is O(n)
  - Has to shift the entire structure down to make room for the element at a given index
  - Same for deletion

### LinkedList Datastructure

- Data can be stored anywhere in memory as each piece of data references the next piece of data in the following index
  - Data does not need to be moved arround
  - Is unbounded
- Good for reading data sequentially
- Bad for reading a data value at a specific index
  - Has to read all of the data before that value to find it
- Reading is O(n)
- Insertion is O(1)
  - Can just reassign memory values to point to the new value
  - Same for deletion

### App to Memory

- Memory management relative to a process can be considered broadly as follows
  - Ensure each process has enough memory to execute
  - Different memory types must be organised efficiently

### Process and Memory Usage

- Kernel controls access for a process to memory addresses
  - The state of an applicatin can be monitored by the system's kernel and the process will wait until resources are available to allow a change in state
- Process manager is responsible for processes in a system
  - Controlled by the kernel to
    - Create and terminate processes
    - Resource allocation and protection
    - Cooperation with device manager to implement I/O
    - Implementation of address space
    - Process scheduling
- The system determines the best process choice to ensure a system runs efficiently and without apparent delays
  - Includes:
    - First-come, first-served
    - Shortest job next
    - Round robin
    - Multi-level priority queue

## Basics

### Binary Search Algorithm

- Common for finding individual items in a larger dataset
  - Returns the index position for a matched result or null
- Guesses a random number X, if that number is larger than the expected value, delete everything 0 to X, if it is higher, delete everything from X to the bound
- Relies on a sorted data set
- Scalable
- O(log n)

### Big O Common Runtimes

- Simple Search
  - O(n)
- Binary Search
  - O(log n)
- Quicksort
  - O(n * log n)
- Selection sort
  - O(n^2)
- Traveling salesman problem
  - O(n!)

### Traveling Salesman Problem

- The salesman has to travel to five cities via the most minimum distance possible

## Big O Part 2

- To calculate Big O, do not include constants
  - Only care about the largest exponent in the equation

### Average Case vs Worst Case vs Best Case

- Average Case
  - If the best option for an alogithm is not choosen, but niether is the worst case, it is the average case
- Best Case is if the algorithm immediatly solved the problem
- Worst Case is if the algorithm has to go through the entire datastructure

### Resources

- [Quicksort - Java - YouTube up to 4:40](https://youtu.be/SLauY6PpjW4?t=205)
- [Quicksort - Java - YouTube up to 8:42](https://youtu.be/SLauY6PpjW4?t=281)

## Binary Search Tree Datastructure

- It is a binary tree
  - Every node has a node to its left or right
    - Values that are less than the current node are on the left
    - Values that are greater than the current node are on the right
  - Every node also has a comparable key and an associated value
    - The tree is sorted by this key
- A binary search of the tree takes O(log n) on average, O(n) for the worst case
  - Faster than arrays for insertions and deletions

### Issues

- Binary search trees do not provide random access
- Performance times are averages
- Different implementations provide different benefits
  - A red-black tree is self balancing by design

### Implementation

- Use a map or dictionary for the basic implementation
- Methods include
  - Min
  - Max
  - Floor
  - Ceiling
  - Selection
  - Rank
  - Delete
  - Delete Min
  - Delete Max
  - Range Search
  - Insert
- Insetion would require all of the following nodes to be reassigned
  - Same with deletion

## Divide and Conquer Algorithm

- Recursive
- Steps:

1. Define the base case
2. Divide and decrease the underlying problem until it is the base case

### Resources

- [Divide and Conquer - YouTube](https://youtu.be/11V7Ik0IBHU?t=65)
- [Euclid and the Greatest Common Divisor - YouTube](https://youtu.be/Q9HjeFD62Uk?t=321)

## Hash Table Datastructure

- Useful and fast
- Conceptually:
  - Store each item in an easily derermined location
  - No ordering to maintain
- Abstractlly look like tables
- Prevent duplicate entries
- Seaching, insertion, and deletion on average tak O(1)
  - Worst case for all three is O(n)
- Load factor can be calculated by
  - Number of items in hash table / total number of slots
  - Can be used to see if there is enough space for all of the information at once

## Quicksort Algorithm

- Sorting algorithm
- Works like divide an conquer
  - Take an unsorted data structure, divide it in two. Take these partitions and divide them, repeat until the length is at a given value K. Sort the individual partitions and reassemble into a sorted data structure

### Resources

- [Algorithms and Sorting - YouTube up to 22:03](https://youtu.be/Q9HjeFD62Uk?t=880)
- [Quicksort - Java - YouTube - up to 3:25](https://youtu.be/SLauY6PpjW4?t=10)

## Recursion

- Define a base case and use a recursive case to arrive at that base case
- Stacks are useful to conduct recursion on
  - LinkedLists are good too

### Cost

- The more recursion that needs to happen, the larger the call stack becomes

## System Memory Structure

- Successfully developing an application assumes that the computer is fully functional

### System Components

- An OS may have a:
  - Process manager
  - Memory manager
  - File system manager
  - Device or I/O manager
- Common System Call Types are:
  - Communication
  - Device management
  - File management
  - Information management
  - Process control
- Calls are converted by the kernel to executable functions such as
  - Create
  - Delete
  - Open
  - Rename
  - Copy
  - Read data
  - Write data
  - Append data
  - Delete file contents
  - Reposition file pointer

### Processes

- Managed by the kernel
- Each process is a child of another
  - The root one in Unix is init
- init Acts as system boot
  - Kernel is responsible for executing it
  - It uses the fork() command to create child processes
- Child Processes use the exec() method to execute commands
  - wait() can be used to gracefully terminate a program
- When created, processes are assigned a spot in memory
  - Kernel can access and manipulate these addresses
- Processes have states which can be monitored by the kernel

### Kernel and Communication

- Synchronisation of the kernal and other components is tested using one of these classic problems
  - Shared buffer
  - Producers and consumers (bounded buffer)
  - Readers and writers
  - Dining philosophers
  - Cigarette smokers
  - Barbershop
- A locking mechanism is utilized to coordinate shared resources
  - Monitors are used to check on this locking mechanism
- There are APIs in place to create and destroy processes
  - System interupts
  - Communication
  - Device management
  - File management
  - Information management
  - Process control

### Kernel and Process Control Blocks

- Process Control Blocks (PCBs) isolate applications from one another
  - Allows for system commands to be executed by multiple programs without having to deal with issues such as parellization or multithreading
- PCBs have:
  - Register values
  - Logical state
  - Page map table mapping logical addresses to physical addresses
  - Type & location of resources it holds
  - List of resources it needs
  - Parent process identification
  - Security keys

### Process Manager

- Managed by the kernel
- Responsibile for all of the monitoring, creation, and termination of processes
  - Other responsibilities:
    - Process creation and termination
    - Resource allocation and protection
    - Cooperation with device manager to implement I/O
    - Implementation of address space
    - Process scheduling
- Process scheduling is done to provide a fast and efficient system
  - Processes are paused and created only when there is enough resources to do so
  - Monitors system metrics to make sure that the system is running at optimal conditions
    - Metrics include:
      - CPU utilisation
      - Throughput
      - Waiting time for process in ready state
      - Service time by CPU for a given process
      - Turnaround time for a process
      - Response time (time from first submission of process to completion...)

### Kernel and the File System

- The kernel is responsible for the file system
  - Operations include:
    - Create, delete, open, close a file
    - Rename, copy a file
    - Read data from and write data to a file
    - Append data to end of specified file
    - Delete file contents (truncate content) - file remains with content wiped
    - Reposition file pointer in defined file
  - Done so using disk scheduling

### CPU and the Kernel

- CPU executes kernel instructions
- The CPU has Compute Units (CU) and Arithmetic Logical Units (ALU)
  - CU responsibile for the allocation and communication of instructions to and from the kernel
  - CU and ALU work together
- CPUs have instruction registers

## Observer Pattern

- This pattern allows for the creation of one to many associations between objects
  - Used in one to many, one way, or event driven systems
  - Promotes loose coupling between components
- Two components
  - Subject
    - Provides interface for observers to subscribe and unsubscribe
    - Sends notifications to observers for changes in state
    - Maintains record of subscribed observers
  - Observer
    - Includes a function to respond to subject notifications
- There is the potential for in a system multiple observers have to be created to handle multiple subjects, some of which may be the same subject but reporting to two distinct observers

## PubSub Pattern

- A variation of the observer pattern
  - Typically used in JS
  - Avoids dependency between observer and subject
- The subscriber (subject) listens for notifications about a specific topic (event) from the publisher (observer)
  - Reverses the roles of the observer pattern
