# REST API

----

- REST stands for REpresentational State Transfer and API stands for Application Programming Interface.
- Representational State Transfer (REST) is a software architecture that imposes conditions on how an API should work.
- REST was initially created as a guideline to manage communication on a complex network like the internet.
- APIs that follow the REST architectural style are called REST APIs.
- Web services that implement REST architecture are called RESTful web services.
- A REST API and RESTful API are same.
- Interaction in REST based systems happen through Internet’s Hypertext Transfer Protocol (HTTP) methods. 
- A Restful system consists of a:
 * client who requests for the resources.
 * server who has the resources.

## Working of REST API :

![Working Of REST APIs](https://fiverr-res.cloudinary.com/images/t_main1,q_auto,f_auto,q_auto,f_autogigs/260127571/original/81b1f622228ecf883ba5985e86aa52c395797482/create-api-rest-from-mysql-db-in-php.png)


- A request is sent from client to server in the form of a web URL as HTTP method that contain GET or POST or PUT or 
 DELETE request.
- After that, a response comes back from the server in the form of a resource which can be anything like HTML, XML, Image, or JSON. But now JSON is the most popular format being used in Web Services.  
- HTTP methods are used to identify the action.

**GET**

- The HTTP GET method is used to access resources that are located at the specified URL on the server. 
- It is used to read a representation of the resources.

**POST**

- The POST verb is most often utilized to create new resources.
- POST also uses to send the client data to the server.
- Sending the same POST request multiple times has the side effect of creating the same resource multiple times.

**PUT**

- Clients use PUT to update existing resources on the server. 

**DELETE**

- Clients use the DELETE request to remove the resource.
- If the user does not have appropriate authentication, the request fails.

![CRUD]("https://assets.website-files.com/5ff66329429d880392f6cba2/61c325278ba0dc1f5c550f27_CRUD%20acronym.png")

-----------------------------------------------

## **REST API Architectural Constraints**

![REST API Architectural Constraints](https://www.google.com/search?q=REST+API+Architectura+Constraints&sxsrf=ALiCzsbd9YuIcQP6EB3q1AXKPBawxribhA:1665567809408&source=lnms&tbm=isch&sa=Xved=2ahUKEwit8oPNs9r6AhWCcGwGHdvqDIEQ_AUoAXoECAEQAw&biw=1536&bih=750&dpr=1.25#imgrc=FdSLA0GzSGOWBM)

**Uniform Interface**

- The uniform interface is fundamental to the design of any RESTful webservice. 
- It indicates that the server transfers information in a standard format. 
- There are four guidelines principle of Uniform Interface are:
  * Resource-Based: Requests should identify resources. They do so by using a uniform resource identifier.
  * Manipulation of Resources Through Representations:Clients have enough information in the resource 
   representation to modify or delete the resource if they want to.
  * Self-descriptive Messages:Each message includes enough information to describe how to process the 
   message so that server can easily analyses the request.
   The server achieves this by sending self-descriptive messages that contain metadata 
  * Hypermedia as the Engine of Application State (HATEOAS): It need to include links for each response 
   so that client can discover other resources easily.
   The server achieves this by sending hyperlinks in the representation.

**Statelessness**

- Server do not store client context between requests.	
- It means that the necessary state to handle the request is contained within the request itself and 
 server would not store anything related to the session. 
- Clients can request resources in any order, and every request is stateless or isolated from other requests. 
- Improves performance  by reducing server load.

**Cacheability**

- RESTful web services support caching, which is the process of storing some responses on the client or on an intermediary to 
 improve server response time. 
- Every response should include whether the response is cacheable or not and for how much duration responses can be cached at the client side. 
- Client will return the data from its cache for any subsequent request and there would be no need to send the request again to the server. 

**Client-Server**

- REST application should have a client-server architecture.
- A Client is someone who is requesting resources and are not concerned with data storage, which remains internal to each server, and server 
 is someone who holds the resources and are not concerned with the user interface or user state. 
- They can evolve independently.

**Layered system**

- An application architecture needs to be composed of multiple layers.
- In a layered system architecture, the client can connect to other authorized intermediaries between the client and server, and it will still receive
 responses from the server.
- Servers can also pass on requests to other servers.
- You can design your RESTful web service to run on several servers with multiple layers such as security, application, and business logic, working 
 together to fulfill client requests. These layers remain invisible to the client.

**Code on demand**

- It is an optional feature.
- In REST architectural style, servers can temporarily extend or customize client functionality by transferring software programming code to the client. 
- For example, when you fill a registration form on any website, your browser immediately highlights any mistakes you make, such as incorrect phone numbers. 
- It can do this because of the code sent by the server.
- Client can download after deployment.

------------------------

- A RESTful web service must **authenticate** requests before it can send a response.
- Authentication is the process of verifying an identity. 
 
#### RESTful API has authentication methods:

**HTTP authentication**

- Here are HTTP authentication :-
  
   - **Basic authentication** :
      In basic authentication, the client sends the user name and password in the request header.
      It encodes them with base64, which is an encoding technique that converts the pair into a set of 64 characters for safe transmission.
   
   -**Bearer authentication**:
        In this,It gives Tokens Bearer.
        The bearer token is typically an encrypted string of characters that the server generates in response to a login request.
  		The client sends the token in the request headers to access resources.

**API Keys**

- The server assigns a unique generated value to a first-time client,that value is known as API Keys.
- Whenever the client tries to access resources, it uses the unique API key to verify itself. 
- API keys are less secure.

**OAuth**

- OAuth combines passwords and tokens for highly secure login access to any system. 
- The server first requests a password and then asks for an additional token to complete the authorization process.

-----------------------------















