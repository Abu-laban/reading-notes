# Access Control (ACL)

### When is Basic Authorization used vs. Bearer Authorization?

- The Basic authentication schemes are dedicated to the authentication using a username and a secret
- The Bearer authentication scheme is dedicated to the authentication using a token

> `Basic` authorization used when in sign-in process, after signing-up.

> `Bearer` authorization used after basic auth done. for every request will use a bearer auth to verfiy if token match user token or not.

### What does the JSON Web Token package do?

- Defines a compact and self-contained way for securely transmitting information between parties as a JSON object.

> Generates a token that we can use with authorization and information exchange.


### What considerations should we make when creating and storing a SECRET?

- Use encryption to store secrets within .git repositories
- Use environment variables
- Use “Secrets as a service” solutions

> don’t create a weak secret.

> don’t store it in a plain text.

> don’t share your secret with anyone.

> don’t use same secret for different accounts.


## Document the following Vocabulary Terms.

- encryption :

is the process of taking plain text, like a text message or email, and scrambling it into an unreadable format — called “cipher text.” This helps protect the confidentiality of digital data either stored on computer systems or transmitted through a network like the internet.

> it is a process that convert our passwords to hashed ones, with characters representation. to make our passwords secured. we use the bcrybt library to do this.

- token :

 is a piece of a two-factor authentication security device that may be used to authorize the use of computer services.

> it an encoded json, that we use in beare authorization to ensure if the user is authorized or not.

- bearer :

(also called token authentication) is an HTTP authentication scheme that involves security , Bearer authentication is a security scheme with type: http and scheme: bearer .

> it is an authorization process, that use the header, and create and compare the token for the users, to allow them to reach a certain endpionts or not.

- secret :

These non-human privileged credentials are often called “secrets” and refer to a private piece of information that acts as a key to unlock protected resources or sensitive information in tools, applications, containers, DevOps and cloud-native environments.

> it is a signiture for the developper that make his token secure and no one can access his data when his secret is exists.

- JSON Web Token :

 is a proposed Internet standard for creating data with optional signature and/or optional encryption whose payload holds JSON that asserts some number of claims. The tokens are signed either using a private secret or a public/private key
