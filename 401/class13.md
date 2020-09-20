# Bearer Authorization

1. **Write the following steps in the correct order:**

  * Register your application to get a client_id and client_secret
  * Receive authorization code
  * Ask the client if they want to sign in via a third party
  * Make a request to a third-party API endpoint
  * Receive access token
  * Make a request to the access token endpoint
  * Redirect to a third party authentication endpoint.

2. **What can you do with an authorization code?**

The authorization code is a temporary code that the client will exchange for an access token. The code itself is obtained from the authorization server where the user gets a chance to see what the information the client is requesting, and approve or deny the request

3. **What can you do with an access token?**

Access tokens are the thing that applications use to make API requests on behalf of a user. The access token represents the authorization of a specific application to access specific parts of a user's data. Access tokens must be kept confidential in transit and in storage.

4. **What’s a benefit of using OAuth instead of your own basic authentication?**

OAuth works based on tokens and authorization. 

## Vocabulary Terms

### Client ID
Public Identifier for apps 
### Client Secret
A secret only is known to the application and authorization server.

### Authentication Endpoint
Endpoint authentication is an authentication mechanism used to verify the identity of a network's external or remote connecting device.
### Access Token Endpoint
Lets the client access the requested resource if a proper credential is provided.
### API Endpoint
The point of entry in a communication channel when two systems are interacting. 
### Authorization Code
The code obtained from the authorization endpoint which the server uses to look up the granted permission or consent.
### Access Token
Contains the security credentials for a login session and identifies the user, the user's groups, the user's privileges, and, in some cases, a particular application.