# API Server

1. **How does [route prefixing](https://medium.com/@zahiruldu/nodejs-route-prefixing-in-expressjs-65196adb3167) work with an external routing module?**

Routing is a getway to receive request from various sources into your application and responding to that request with required data.

2. **When routing, what’s the difference between `app.get('/data/:id')` and `app.get('/data/:name')`?**

/:Id will get the ID number from the object, and /:name will get the name from the object.

3. **Explain how Express handles routing conflicts?**

Throwing a 404 error.

4. **What are the ways that a browser can send “data” or request variables to an HTTP server**
GET, PUT, POST.

## Vocabulary Terms
### [Routing](https://medium.com/@fro_g/routing-in-javascript-d552ff4d2921)
A Javascript router is a key component in most frontend frameworks. It is the piece of software in charge to organize the states of the application, switching between different views.
### [Route Prefixing](https://medium.com/@zahiruldu/nodejs-route-prefixing-in-expressjs-65196adb3167)
Used to set a common prefix for an entire controller.
### Request “Body”
json() function that returns an Express middleware function that parses JSON HTTP request bodies into JavaScript objects. 
### Request “Query”
Here Request is a object that retrieves the values that the client browser passed to the server during an HTTP request and QueryString is a collection is used to retrieve the variable values in the HTTP query string
### Request “Params”
Request.Params is a combination of the keys/values you'll find in Request.Querystring , Request.Form , Request.Cookies , Request.ServerVariables (in that order).