## API Integration

### Review, Research, and Discussion

**1. How do bearer tokens work?**

> Bearer Token A security token with the property that any party in possession of the token (a “bearer”) can use the token in any way that any other party in possession of it can. Using a bearer token does not require a bearer to prove possession of cryptographic key material (proof-of-possession).

> request to the Express server. Each middleware has access to the HTTP request and response for each route (or path) it’s attached to. … This “chaining” of middleware allows you to compartmentalize your code and create reusable middleware


**2. Describe express middleware**

> Express middleware are functions that execute during the lifecycle of a request to the Express server. Each middleware has access to the HTTP request and response for each route (or path) it's attached to. ... This “chaining” of middleware allows you to compartmentalize your code and create reusable middleware

**3. What is a JWT?**

> JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.

> Although JWTs can be encrypted to also provide secrecy between parties, we will focus on signed tokens. Signed tokens can verify the integrity of the claims contained within it, while encrypted tokens hide those claims from other parties. When tokens are signed using public/private key pairs, the signature also certifies that only the party holding the private key is the one that signed it.



**Term** | **Definition**
-----|-----
role based access control | Attribute-based access control, also known as policy-based access control for IAM, defines an access control paradigm whereby access rights are granted to users through the use of policies which combine attributes together. The policies can use any type of attributes
http cookies | HTTP cookies, or internet cookies, are built specifically for Internet web browsers to track, personalize, and save information about each user's session. A “session” just refers to the time you spend on a site. Cookies are created to identify you when you visit a new website.
