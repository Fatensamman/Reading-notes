##  Bearer Authorization
- Write the following steps in the correct order:

a. Register your application to get a client_id and client_secret 
b. Make a request to a third-party API endpoint 
c. Redirect to a third-party authentication endpoint 
d. Receive authorization code 
e. Ask the client if they want to sign in via a third part
f. Make a request to the access token endpoint

- What can you do with an authorization code?

process of determining if the user has permission to perform a given operation.

- What can you do with an access token?

Any time we need to call an API endpoint that is only available to authorized users, we store this token on the client and send it to the server.

What’s a benefit of using OAuth instead of your own basic authentication?

They help us recognise users. It looks like a visa or a driver's license. Its payload incorporates a few public properties regarding a consumer. Since tampering with these properties will necessitate re-generating the digital signature, it is not possible.

## Term :

* Client ID

The client id is an app's public identifier. Even though it's public, it's better that third parties can't figure it out, because many implementations use a 32-character hex series. It also has to be unique across all of the authorization server's clients. It is marginally easier to craft phishing attacks against random programs if the client ID is guessable.

* Client Secret

The client_secret is a secret known only to the application and the authorization server. It must be sufficiently random to not be guessable. A great way to generate a secure

* Authentication API enables you to manage all aspects of user identity when you use Auth0

* Access Token Endpoint

Auth0 produces JSON web token (JWT) format access tokens for API authorization scenarios. Scopes are the rights represented by the access token in OAuth terminology. When a program uses Auth0 to authenticate, it defines the scopes it needs to use. If the user has given permission for those scopes, the access token would reflect those permissions.

* API Endpoint

An API endpoint is a location where an application program interface (API) – the code that enables two software programs to interact – links to the software program. APIs function by submitting and receiving requests for information from a software application or web server.

* Code of Authorization The authorization code is a one-time use code that the customer can use to obtain an access key. The code is accessed from the authorization server, which allows the administrator to view the details requested by the client and accept or reject the request.

* Token of Access Token-based authentication uses authorization tokens to authorize an application to access an API. When a user successfully authenticates and authorizes entry, the program collects an access token, which it uses as a credential when calling the goal API. The passed token tells the API that the bearer of the token has been given access to the API and has been allowed to perform unique acts specified by the scope granted during authorization.

## A JSON Web Token (JWT) 

is a JSON object encoded as a long string. We use 
them to identify users. It’s similar to a passport or driver’s license. It includes a few public properties about a user in its payload. These properties cannot be tampered because doing so requires re-generating the digital signature. 

- When the user logs in, we generate a JWT on the server and return it to the 
client. We store this token on the client and send it to the server every time we need to call an API endpoint that is only accessible to authenticated users.

- To generate JSON Web Tokens in an Express app use jsonwebtoken package. 
// Generating a JWT 
const jwt = require(‘jsonwebtoken’);
const token = jwt.sign({ _id: user._id}, ‘privateKey’);

- Never store private keys and other secrets in your codebase. Store them in 
environment variables. Use the config package to read application settings 
stored in environment variables. 
- When appropriate, encapsulate logic in Mongoose models.


 [JSON Web Token](https://en.wikipedia.org/wiki/JSON_Web_Token)
