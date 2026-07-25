# REST Architecture

## Introduction

REST (Representational State Transfer) is a software architectural style used for designing web services and APIs. It was introduced by Roy Fielding in his doctoral dissertation in 2000. REST is not a protocol or a standard. Instead, it is a set of architectural principles that helps developers build scalable, reliable, and maintainable web applications. REST APIs allow different software systems to communicate over the internet using standard HTTP methods.

## How REST Architecture Works

REST architecture follows a client-server model where the client sends a request to the server, and the server processes the request and returns a response. The client and server remain independent, allowing each to evolve without affecting the other.

Each resource in a REST API is identified using a Uniform Resource Identifier (URI). Clients interact with these resources using standard HTTP methods.

### Common HTTP Methods

* **GET** – Retrieves data from the server.
* **POST** – Creates a new resource.
* **PUT** – Updates an existing resource.
* **PATCH** – Partially updates an existing resource.
* **DELETE** – Removes a resource from the server.

## REST Architectural Constraints

REST is based on six architectural constraints that improve performance and scalability.

### 1. Client-Server Architecture

The client is responsible for the user interface, while the server manages data and business logic. This separation allows independent development and maintenance.

### 2. Stateless Communication

Each client request must contain all the information required to process it. The server does not store information about previous requests, making REST APIs easier to scale.

### 3. Cacheable Responses

Server responses can be marked as cacheable. Cached responses reduce the number of requests sent to the server and improve application performance.

### 4. Uniform Interface

REST defines a consistent interface for communication between clients and servers. Resources are accessed using URIs, and standard HTTP methods are used to perform operations.

### 5. Layered System

A REST application may contain multiple layers, such as security, caching, and load balancing. Clients do not need to know whether they are communicating directly with the server or through intermediate layers.

### 6. Code on Demand (Optional)

A server can send executable code, such as JavaScript, to extend the functionality of the client. This constraint is optional and is not commonly used in most REST APIs.

## Resource Representation

Resources can be represented in different formats. The most commonly used formats are:

* JSON (JavaScript Object Notation)
* XML (Extensible Markup Language)
* HTML
* Plain Text

Today, JSON is the preferred format because it is lightweight, easy to read, and supported by most programming languages.

## Example REST API

The following example shows a simple REST API for managing users.

| HTTP Method | Endpoint | Description |
|-------------|----------|-------------|
| GET | `/users` | Retrieve all users |
| GET | `/users/1` | Retrieve user with ID 1 |
| POST | `/users` | Create a new user |
| PUT | `/users/1` | Update user with ID 1 |
| DELETE | `/users/1` | Delete user with ID 1 |

### Example JSON Response

```json
{
  "id": 1,
  "name": "Ankit",
  "email": "ankit@example.com"
}
```

## Advantages of REST Architecture

* Simple and easy to understand.
* Uses standard HTTP methods.
* Supports multiple data formats.
* Highly scalable because it is stateless.
* Easy to integrate with web, mobile, and cloud applications.
* Better performance through caching.
* Independent development of clients and servers.

## Limitations of REST Architecture

* Stateless communication may increase request size because each request must include all required information.
* Multiple requests may be needed to retrieve complex data.
* There is no fixed standard for API design, so implementations can differ across organizations.

## Applications of REST APIs

REST architecture is widely used in modern software development, including:

* Web applications
* Mobile applications
* Cloud services
* E-commerce platforms
* Social media applications
* Banking and financial systems
* Internet of Things (IoT) applications

## Conclusion

REST architecture is one of the most widely used approaches for building modern web services. Its client-server model, stateless communication, and use of standard HTTP methods make applications scalable, flexible, and easy to maintain. REST APIs enable different systems to exchange data efficiently and are supported by almost every programming language and framework. Understanding REST architecture is an essential skill for software developers because it forms the foundation of many web and mobile applications used today.

## References

* https://restfulapi.net/
* https://www.redhat.com/en/topics/api/what-is-a-rest-api
* https://aws.amazon.com/what-is/restful-api/
* https://developer.mozilla.org/en-US/docs/Web/HTTP
* https://roy.gbiv.com/pubs/dissertation/rest_arch_style.htm
