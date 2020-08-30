# Express

1. What’s the difference between `PUT` and `PATCH`?

The main difference between the PUT and PATCH method is that the PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource, whereas the PATCH method supplies a set of instructions to modify the resource.

2. Provide links to 3 services or tools that allow you to “mock” an API for development like `json-server`

[Insomnia](https://insomnia.rest)

[PostMan](https://www.postman.com/features/mock-api/)

[Swagger](https://swagger.io/docs/)

3. Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?

**Swagger:**
- 200: OK.
- 400: Bad request. User ID must be an integer and bigger than 0.
- 401: Authorization information is missing or invalid.
- 404: A user with the specific ID was not found.


4. Compare and contrast SOAP and ReST

**SOAP**
- Simple Access Protocol
- Is a protocol
- Only works with XML formats
- Cannot make us of rest 

**REST**
- Representational State Transfer
- Is an architectural pattern
- Works with plain text, XML, HTML and JSON
- Cna make use of soap

## Vocabulary Terms
### SOAP
SOAP is a messaging protocol specification for exchanging structured information in the implementation of web services in computer networks. Its purpose is to provide extensibility, neutrality, verbosity and independence.
### ReST Verbs
POST, GET, PUT, PATCH, and DELETE. These correspond to create, read, update, and delete (or CRUD) operations, respectively. There are a number of other verbs, too, but are utilized less frequently.
### CRUD Verbs
Read, Update/Replace, Update/Modify, Delete
### Swagger
Swagger is a set of rules (in other words, a specification) for a format describing REST APIs. ... As a result, it can be used to share documentation among product managers, testers and developers, but can also be used by various tools to automate API-related processes.

## Express Middleware
Middleware literally means anything you put in the middle of one layer of the software and another. Express middleware are functions that execute during the lifecycle of a request to the Express server. Each middleware has access to the HTTP request and response for each route (or path) it's attached to.

