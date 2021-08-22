# Bearer Authorization

### Write the following steps in the correct order:

- Receive access token
- Redirect to a third party authentication endpoint
- Register your application to get a client_id and client_secret
- Make a request to a third-party API endpoint
- Ask the client if they want to sign in via a third party
- Receive authorization code
- Make a request to the access token endpoint


1. Register your application to get a client_id and client_secret
2. Ask the client if they want to sign in via a third party
3. Make a request to a third-party API endpoint
4. Redirect to a third party authentication endpoint
5. Make a request to the access token endpoint
6. Receive access token
7. Receive authorization code

### What can you do with an authorization code?

> An authorization code is an alphanumeric password that authorizes its user to purchase, sell or transfer items, or to enter information into a security-protected space

### What can you do with an access token?

Access tokens are the thing that applications use to make API requests on behalf of a user. The access token represents the authorization of a specific application to access specific parts of a user's data.

### What’s a benefit of using OAuth instead of your own basic authentication?

> It enables apps to obtain limited access (scopes) to a user's data without giving away a user's password. It decouples authentication from authorization and supports multiple use cases addressing different device capabilities.

OAuth contains authorization requests, access tokens and refresh tokens and widely accepted as the standard for modern web applications. It is well documented and easy to implement.

## Document the following Vocabulary Terms.

- Client ID :

The client_id is a public identifier for apps. Is used to identify the application.
    - It must also be unique across all clients that the authorization server handles.
    -  it’s best that it isn’t guessable by third parties

- Client Secret :

The client_secret is a secret known only to the application and the authorization server.

- Authentication Endpoint :

 Endpoint authentication is a security mechanism designed to ensure that only authorized devices can connect to a given network, site or service.

> The approach is also known as device authentication.

- Access Token Endpoint :

The token endpoint is where apps make a request to get an access token for a user.

- API Endpoint :

 is a point at which an application program interface (API) -- the code that allows two software programs to communicate with each other -- connects with the software program.

- Authorization Code :

  **is essentially a unique password for the domain, made up of letters, numbers, and special characters.**

 The authorization code is a temporary code that the client will exchange for an access token It’s used to prove your ownership of the domain and authorize a domain transfer.

- Access Token : 

        Used for token-based authentication is an object encapsulating the security identity of a process or thread.

 > The information in a token includes the identity and privileges of the user account associated with the process or thread.
