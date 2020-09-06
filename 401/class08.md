# Express Routing & Connected

1. **Name 3 real world use cases where you’d want to change the request with custom middleware**

To insert code errors in the request.
To have a response in json.
To make timestamp logs. 

2. **True or false: The route handler is middleware?**

True

3. **In what ways can a middleware function end the process and send data to the browser?**

When not calling the next() argument.

4. **At what point in the request lifecycle can you “inject” middleware?**

Before the routes.

5. **What can cause express to error with “Request headers sent twice, cannot start a second response”**

When is more than one .send functions in one route


## Vocabulary Terms
### [Middleware](https://expressjs.com/en/guide/using-middleware.html)
Functions that have access to the request/response objects, and the next middleware function in the req/res cycle. Middleware must be placed before the routes!
### [Request](https://expressjs.com/en/4x/api.html#req) Object
Represents the http request and has properties for query strings, parameters, body, http headers.
### [Response](https://expressjs.com/en/4x/api.html#res) Object
The res object represents the HTTP response that an Express app sends when it gets an HTTP request.
### Application Middleware
Middleware that takes place in all routes of the application
### [Routing](https://scotch.io/tutorials/learn-to-use-the-new-router-in-expressjs-4) Middleware
In Express is a way to do something before a request is processed.