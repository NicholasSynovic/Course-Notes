# COMP 333 Lecture Notes

## Week 1

### Lecture 1
* Computing with Web Services
	* Plenty of APIs exist
	* A Web Service is a service on the web/ internet
		* Any service/ API that is accessible over http is a web service
	* Mash-Up is taking one or more APIs and combining the data output into one product
* Distributed Computing
	* How two systems are communicating with one another in the hope of producing a better output
	* Services are any software function that carries out a:
		* Business task or process such as rder placing, shipping, payment
		* Any system operations such as accessing files, authentication, authorization, etc.
		* Any useful functionality exposed by a system
	* Services can be used to share functions across different applications and to enable software that runs on disparate computing platforms to collaborate
		* Implies that there are a client instance of the service and a server instance of the service
			* The service processes may be located on the same machine as the client's process but is usually found on a server
	* Closed Distributed Computing
		* Anything between the client and server are proprietary 
			* Language dependent payload
				* One computer looking for a Java output from another
			* Non-standard protocol
				* Communicating over file I/O
* Service Oriented Architecture (SOA)
	* SOA is a style of design that guides all aspects of creating and using business services throughout their life cycle
		* A paradigm for organizing and utilizing distributed capabilities that mayy be under control of different ownership domains
		* Underlying structure supporting communications between services
			* Defines how two computing entities interact in such a way as to enable one entity to perform a unit of work on behalf of the other
	* Does not have to be ran on the web for it to be SOA
* Web Services
	* Refers to software functions that can be invoked by leveraging HTTP as a simple transport protocol over which data is carried or by using HTTP as a complete application protocol that defines the semantics for service behavior
		* Client/ Requester/ Service Consumer is something that triggers events
		* Server/ Provider/ Service Producer is a component that responds or reacts to these requests and events
	* Provide the means to integrate disparate systems and expose reusable business functions over HTTP
		* Leverage HTTP as:
			* A simple transport over which data is carried
			* Use it as a complete application protocol that defines the semantics for service behavior
	* Rely on open and interoperable standards independent of the underlying technology
		* Non proprietary protocol
		* Language independent
	* use HTTP and leverage data interchange standards like XML and JSON and common media types
		* Open standards payloads
		* Standard serialization/ deserialization
	* Allows the facilitation and creation of complex buisiness processes through service composition
		* Mash-Ups
		* Multiple services from different providers
	* Makes it relatively easy to reuse and share services with mobile, desktop, and web applications
* Web Services Architecture View
	* Top level: Client applications
	* Below: Service Layer
	* Below: Domain Layer
	* Below: Data Sources
* Basic Web Services Standards
	* JSON
		* Based on a subset of the JavaScript
		* Text format that is completely language independent
		* 
	* XML
		* Markup language
		* Textual data that uses Unicode
		* Widely used for the representation of data types
	* XSD
		* XML Schema Definition Language
	* WSDL
		* Web Services Description Language
	* XPath
		* XML Path Language
	* XSLT
		* Extensible Stylesheet Language Transformation
	* TCP/ IP
		* TCP is used for transmission of data from an application to the network
			* Responsibility for breaking data down into IP packets before they are sent and for assembling the packets when they arrive
			* Assembles data as well
		* IP takes care of the communication with other computers
			* Responsible for sending and recieving data as well
	* HTTP/ Web
		* HTTP takes care of the communication between a web server and a web browser
		* Used for sending requests from a web client to a web server
			* Also for returning web content from the server back to the client
		* Verbs
			* Methods
				* GET, POST, PUT, DELETE
			* URI/ URL
				* Uniform Response Identifier
				* Has in order:
					* Protocol identifies the transport scheme that will be used to process and respond to the request
						* HTTP, FTP, etc.
					* Host name identifies the server address of the resource
						* Converted to an IP
sweb					* Path is used to identify the accessed resource
					* Query String is used to customize the accessed resource
					* EVERY URI/ URL IS UNIQUE
			* Request and Response Headers
			* Internet Media Types
			* HTTP Request and Response Codes
* Web Service API Styles
	* API is a set of unctions that one computer program makes available to other programs so they can talk to it directly
		* OS APIs
		* Application APIs
		* Toolkit APIs
		* Web Site APIs
			* Types:
				* RPC API
					* Remote Procedure Call
						* How clients execute remote procedures over HTTP
						* A message to tell a machine what to do 
				* Resource API
					* How a client manipulate data managed by a remote system and avoid direct coupling to remote procedures and minimizes the need for the domain specific API
						* Assign all procedures, domain data, and files a URI


## Week 2

### Lecture 1
* Object Oriented Models have:
	* Association
	* Cardinality
	* Navigation
	* Composition
	* Generalization
* Database Model
	* A type of data model that determines the logical structure of a database and fundamentally determines in which manner data can be stored, organize, and manipulation
		* Most popular example of a database model is the relational model
			* Has keys and columns
* CRUD
	* Create, Read, Update, Delete
		* Four basic function to be performed on relational databases
		* Almost all CRUD SQL statements are similar in different DB implementations
* Persisting Object Models into Relational Database
	* Single Class to a Table
		* Easy conversion
	* Classes with Relationship
		* Needs direction
			* To do this export the Primary Key from the main class into the secondary class
	* Many to Many Relationship
		* Create a second table that holds the primary keys of both tables
	* Inheritance
		* One table per concrete class
			* Either create one table with all of the information or multiple sub classes that are 1 to 1 with the root class
	* Object/ Relational Mappers (ORM)
		* A technique for converting data between objects developed in OO and relational database tables
			* Creates a virtual object databases that can be used from within programming language
* Layering
	* Layered system is organized hierarchically
		* Each layer providing service to the layer above it
		* Serves as a client to the layer below
	* Principles
		* The higher layer uses various services defined by the lower layer
		* Lower layer is unaware of the higher layer
			* Each layer usually hides its lower layers from layers above
	* Benefits
		* Understand  single layer as a coherent whole
		* Substitute layers with alternative implementations of the same basic services
		* Minimize dependencies between layers
		* Every layer things typically need to be transformed from one representation to another
	* Layers vs Tiers
		* Tier as implying a physical separation
		* Client/ Server systems are often described as two tier systems and the separation is physical
		* Use layer to stress that they don't have to run on the layers on different machines
* Three Principal Layers
	* Presentation/ View/ Service
		* How to handle the interactin between the user and the software
		* Two types:
			* Graphics UI
			* HTML-Based Browser UI
		* Responsible for displaying information to the user and interpret commands from the user into actions upon the domain and data source layers
	* Domain/ Business
		* Functionality of the system 
	* Data Source/ Data Access
		* Data source logic is about communicating iwth other systems that carry out tasks on behalf of the application
			* Biggest piece of logic is a database that is primarily responsible for storing and persistent data
* Organizing Domain Logic (Domain Modeling)
	* Domain Model is a conceptual model of all the topics related to a specific problem
		* Describes:
			* Various entities
			* Attributes
			* Roles
			* Relationships
			* Constraints
		* Created in order to represent the vocabulary and key concepts of the problem domain
		* Identifies the relationships among all enetities within the problem and their common attributes
		* Provides a structural view of the domain
		* Used to verify and validate the understanding of the problem among various stakeholders
		* Adds precision and focus to discussion among the business and technical teams

## Week 3

### Lecture 1

## Week 4

### Lecture 1
* Resource Web Service/ API (Resource API
	* How can a client:
		* Manipulate data managed by a remote system
		* Avoid direct coupling to remote procedures
		* Minimize the need for domain specific APIs
	* CRUD Services
		* Create
		* Read
		* Update
		* Delete
	* Assigns all procedures and files in a Uniform Resource Identifier
	* Leverages HTTP as a complete application protocol to define standard service behaviors
	* Exchange information by taking advantage of standardized media types and status codes
	* Clients invoke a request via a distinct URL designated for each resource
	* Use HTTP as a complete application protocol
	* Each request may carry a standardized or proprietary media type
* Representational State Transfer (REST)
	* High level architecture style that could be implemented using many different technologies
		* Includes the concepts of resources and a uniform interface
			* Uniform interface is the idea that every resource should respond to the same methods
			* HTTP is a REST style
		* Constraints
			* Identification of resources
			* Manipulation of resources through representations
			* Self-descriptive messages
		* Hypermedia as the engine of application state
* Rest Verbs Description
	* GET
		* Retrieves a representation of a resource
		* Safe operation
			* Can be repeated with no conequences
	* POST
		* Appends to an existing resource or Creates a new resource
	* PUT
		* Creates a resource or updates it if the resource already exists on the server
	* DELETE
		* Deletes a resource

## Week 5

### Lecture 1
* HTTP & REST
	* HTTP Vocab
		* verbs/ methods
		* URis
		* Request and Response Headers
		* Internet Media Type
		* HTTP Request and Response codes
	* REST over HTTP works with and leverages these features and allows to perform additional functions on the network such as HTTP caching and security enforcement
* RPC contrast to REST
	* SOAP/ RPC over HTTP encourages each application designer to define a new and arbitrary vocabulary of verbs
		* Methods are overlaid onto the HTTP methods
		* Disregards many of HTTp's existing capabilities in favor of the developers own methods
* Constraints of a REST Architecture
	* Identification of resources
		* Individual resources are identified in requests using URIs
		* Resources are conceptually separate from the responses sent to clients
			* Server does not send a database back to the user, sends a JSON file instead
	* Manipulation of resources through representations
		* When a client has a representation of a resource it has the ability to modify our delete the resource on the server
	* Self-descriptive messages
		* Each message includes enough ionformation to describe how to process the message
			* MIME types
		* From the media type alone, the client must know how to process its contest
			* If the client needs to look into the media type it is not self-descriptive
		* Server is stateless
	* Hypermedia as the engine of application state
		* HATEOAS
			* At any particular time a client can either be transitioning between application states or at rest
				* Rest state is able to interact with its user but creates no load and consumes no per-cline storage on the set of servers or on the network
				* The client sending requests when it is ready to transition to a new state
					* While one or more requests are outstanding, the client is considered to be transitioning states
			* Server is stateless
		* It is likely that the client will want to access related resources
			* Should be identified in the representation returned
* HTTP vs HTTPS
	* HTTPS is to create a secure channel over an insecure network
		* Provides reasonable protection from eavesdroppers and MITM attacks
		* Encrypts an HTTP message prior to transmission and decrypts the message upon arrival
		* HTTPS is not a seperate protocol but refers to use of ordinary HTTP over SSL
*  HTTP REST Basics
	* Accept and Content Type
		* The client's responsibility to use the Accept request header to identify the expected content type of the returned resource
		* Server describes what it is sending with Content-Type
	* Idempotent and Safe
		* Idempotent means that multiple identical requests should have the same effect as a single request
		* GET, HEAD, OPTIONS, and TRACE are defined as safe which means they are intended only for information retrieval and should not change the state of the server
			* Safe == Idempotent
	* REST URI
		* Use nouns (resource locations/ arguments) in a REST URI
			* GET is the only noun that does not modify the resource
		* The Query String needs to have an ID implicitly or explicitly called to access the proper data
* Content Negotiation/ Media Types
	* Content Negotiation refers to the practice of making available representations via the same URI
		* Negotiation between the requesting agent and the server determines which representation is served
	* A resource can be represented in different ways
	* A client doesn't know what a server is going to send to it
		* It is better for the client to decide what the Media Type is
	* A server doesn't know what a client can handle
	* Content types are negotiated using headers
		* Client describes what it wants with Accept header (request)
			* User agent informs the server what media types it understands
				* User agent provides an Accept HTTP header that lists acceptable media types
					* Server uses that list to supply the version of the resource that best fits the user agent's needs
		* Server describes what it is sending with Content-Type header (response)
			* POST and PUT also using the Content-Type header as well
			*  USER proves an Accept HTTP header that lists acceptable media types
* Rest Frameworks
	* REST service in Java web application can be implemented in serval ways
		* A plain Java Servlet
			* For very simple REST services
			* Requires boiler plate code
		* Using a REST frameworks removes the boiler plate code
			* Java provides the JAX-RS framework
				* Java API for RESTful Services
					* Removes the boiler plate code
				* CXF web Services Framework
					* Provides robust support for several web service patterns and specifications
					* Works on top of existing Java code
						* Supports for JAX-RS annotations
* CXF and JAX_RS Basics
	* JAX-RS applications consit of a hierarchy of resources
		* Resources are served up by a CXF controller servlet
		* Each REST resource is mapped to a request URL that is relative to the CXF servlet path
		* Methods that return a resource are annotated
* HATEOAS
	* Hypermedia As the Engine of Application State
	* Client doesn't have a built in knowledge of how to navigate and manipulate the model
		* Server provides that information dynamically to the user
		* Implemented using media types and link relations

## WEEK 6

### Lecture 1
* JAX-RS uses Java annotations
	* Applied to a Java method to bind it to an HTTP method
		* Annotations
			* @Path annotations customize the request URI of resource
				* Defines the base relative path foir all resources supplied by that class
				* Defines the relative path for the resource bound to that method
				* Relative to an @Path on the class
				* Absence of @Path on the class or method the resource is defined to reside at the root of the service
			* @QueryParam maps to a query string parameter
			* @PathParam maps to a path segment
			* @FormParam maps to a form POST statement
			* @DefaultValue supplies a default parameter value
			* @Produces the content type
			* @Consumes requires that content type
		* Multiple methods can have the same annotation as long as they point to different resources
	* They customize many parts of the REST service
		* Identify the HTTP method for accessing a resource
		* Identify the relative path for accessing a resource
		* Identify how to query and form parameters, headers, cookies, and other HTTP request message parts
		* Identify the available content type
* REST Layer Applications
	* Top to bottom
		* HTTP and Endpoints
			* Programmatic binding to the underlying web server
		* Representations
			* Representation of the resource
		* Resource
			* Acts a controllers for workflow activities passing through business information extracted from the representaion and marshaling results into HTTP responses
		* Activity/ Workflow
			* Implement the individual activities in terms of resource life cycles
				* CRUD
			* Responsible for state
		* Domain/ Business Logic Layer
		* Data Access Layer
* More on Service Architecture and JAX-RS/ CXF features
	* Resource Class
		* Exposes the service implementation
		* A resource class is a java class annotated with JAX-RS annotations to represent a Web Resource
		* Two types of resource classes
			* Root resource classes
				* Annotated with at least a @Path
			* Sub resource classes
				* Typically have no annotations
	* Representations Class
		* Looks like the underlying domain object
			* If the domain object has 20 fields and the user only needs 5, a representation object can do that
		* Will be sent over the wire after being converted to XML, JSON, etc.
		* Marked with JAXB annotation to support XML serialization
		* Contain links
			* HATEOAS
	* Workflow Activity Class
		* Units of work
			* Linker between the URI and the Business logic
		* Delegated to work with the domain objects on behalf of the Resource class
		* Executes some business interactions with the domain model
		* Each activity knows about the valid activities that follow and is able to map those activities to the URIs
	* Client API
		* CXF JAX-RS provides a comprehensive support for developing RESTful clients by introducing 3 flavors of the Client API
		* Usually taken care of by the browser
			* Use PostMan for testing
	* JAX-RS: XML and JSON Providers
		* CXF automatically provides support for reading and writing XML to and from JAXB annotated classes
		* Provides built in reading and writing JSON to and from JAXB annotated classes
		* 