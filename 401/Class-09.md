# Authorization/Authentication

### What header(s) are used in authentication and authorization

- The WWW-Authenticate and Proxy-Authenticate response headers define the authentication method that should be used to gain access to a resource. They must specify which authentication scheme is used, so that the client that wishes to authorize knows how to provide the credentials.

### What is safe to put into a JWT

- add "secret" that is used to generate the JWT. If someone modifies the data contained in the JWT, the server will fail to decode it. So the server can trust any JWT that it can decode.


### How are JWTs validated

- Header

The contents of the Header describe the cryptographic operations to the JWT data.

- Payload

*The payload is the central part of the JWT which contains verifiable security statements*

Registered Claim Names

Public Claim Names

Private Claim Names

- Signature

HS256 algorithm, which is short for HMAC-SHA256

RS256 signing algorithm, which is short for RSA-SHA256


## Document the following Vocabulary Terms.

- RBAC :

Role-based access control is a method of restricting network access based on the roles of individual users within an enterprise.

- User Roles :

 it is what the user is supposed to do in an organization, what are his/her duties.

- JWT Token :

(JSON Web Token (JWT) access tokens conform to the JWT standard and contain information about an entity in the form of claims. They are self-contained therefore it is not necessary for the recipient to call a server to validate the token.