# Access Control (ACL)

## When is Basic Authorization used vs. Bearer Authorization?

The Basic authentication schemes are dedicated to the authentication using a username and a secret (see RFC7616 and RFC7617). The Bearer authentication scheme is dedicated to the authentication using a token and is described by the RFC6750. Even if this scheme comes from an OAuth2 specification, you can still use it in any other context where tokens are exchange between a client and a server. Concerning the JWT authentication and as it is a token, the best choice is the Bearer authentication scheme.

## What does the JSON Web Token package do?
(for creating access tokens.)
it defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed.

When the user logs in, we generate a JWT on the server and return it to the client. We store this token on the client and send it to the server every time we need to call an API endpoint that is only accessible to authenticated users.

## What considerations should we make when creating and storing a SECRET?
should be kept protected, best kept in a .env file that is not uploaded with the rest of your code .

# Term

|    |  |
| ----------- | ----------- |
| encryption | attempting to hide information/data        |
| token      | used in bearer authentication, a token is a cryptic string that is generated by the server in response to a login request.        |
| Bearer      | is a service that allows transmission of information signals between network interfaces. These services give the subscriber the capacity required to transmit appropriate signals between certain access points, i.e. user network interfaces.  "give access to the bearer of this token"        |
| Secret      |  this is what is paired with a token, a secret string stored on the server used to sign and encode the token .       |
| JSON Web Token      | is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed.        |


### role-based access control (RBAC)

Its the idea of assigning system access to users based on their role within an organization .

### Benefits of RBAC

it can in reality be easy to implement, and will make the ongoing management of access rights much easier and more secure.


- Access control lists (ACL): defining access rights by a given user or user group, to a specific object such as a document
- Attribute-based access control (ABAC): sometimes known as policy-based access control, can use a variety of attributes including user department, time of day, location of access, type of access required

