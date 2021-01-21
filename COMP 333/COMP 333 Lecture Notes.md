# COMP 333 Lecture Notes

## Week 1

### Lecture 1
* Mash-Up is when two API's are put together to create new data/ options for users
* Distributed Computing
	* Services is any software function that carries out a business task or process, system operations, and/or any useful functionality exposed by a system
		* Can be used to share functions across different applications and enable software to run on disparate computing platforms that collaborate
			* Implies that there is a client and server
		* Service processes may be located on the same machine as the client's process but is usually found on another machine
* Service Oriented Architecture
	* A design style that guides all aspects of creating and using business services throughout their life cycle
	* A paradigm for organizing and utilizing distributed capabilities that may be under control of different ownership domains
	* Defines how two computing entities interact in such a way as to enable one entity to perform a task
* Web Services Overview
	* Web Services refer to software functions that can be invoked by leveraging HTTP as a simple transport protocol over which data is carried or could use HTTP as a complete application protocol
		* Service requester or the one that triggers events is the client, requester or service consumer
		* Software component that responds or reacts to these requests and events is the server, provider, or service producer
	* Provide  the means to integrate disparate systems and expose reusable business functions over HTTP
		* Leverage HTTP as a simple transport over which data is carried
		* A complete application protocol
	* Rely on open and interoperable standards independent of the underlying technology
		* No proprietary protocol
		* Language independent
	* Use HTTP and leverage data interchange standards like XML and JSON and common media types
		* Open standards payload
		* Standard serialization and deserialization
	* Multiple services can create complex business processes through service composition
		* Mash-Ups
	* Make it easy to reuse and share services with mobile, desktop, and web applications
* Frameworks and Standards for Web Services Programming
	* NEED TO KNOW THESE
		* Client Applications rely on the Service Layer which relies on the Domain Layer which relies on the Data Sources Layer
		* Basic elements of Web Service solutions
			* JSON
				* Based on a subset of JavaScript
				* 
			* XML
				* Markup language
				* Produced by W3C
				* 
			* XSD
			* WSDL/ SOAP/ POX Frameworks
				* The java API for xml; web services
				* Apache CXF
				* Microsofts windows communication foundation
			* REST Frameworks
				* Java API for RESTful Web Services
				* Apache CXF
				* Microsoft WCF
				* Spring 
			* XPath
			* XSLT
			* TCP/IP
				* Transmission Control Protocol
					* Gets packets from one end to another
						* Breaks them down to be sent and error checked
				* Internet Protocol
					* Communication with other computers
					* Sends and receives packets
			* HTTP/Web
				* Hyper Text Transfer Protocol
					* Takes care of the communication between a web server and a web browser
					* Used for sending requests from a web client to a wweb server and returning web content from the server back to the client
					* Vocab
						* Verbs or methods
						* URI
							* Unique
							* Has a protocol, host name, path and query string
						* Request and response headers
						* Internet Media Types
						* HTTP Request and Response Codes
			* Application Programming Interface
				* A set of functions that one computer program makes available to other programs so they can talk to it directly
				* Types:
					* RPC API
						* How clients execute remote procedures over HTTP
						* Send a message to execute some code on a server
					* Resource API
						* How clients manipulate data managed by a remote system and avoid direct coupling to remote procedures as well as minimizing the need for the domain specific API 