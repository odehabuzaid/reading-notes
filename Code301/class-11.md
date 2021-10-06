Code401# What is OAuth

1. What is OAuth?

> `is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential`

2. Give an example of what using OAuth would look like.

> `login/signup with google account on canvas`

3. How does OAuth work? What are the steps that it takes to authenticate the user?

* The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
  
* The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
  
* The first site gives this token and secret to the initiating user’s client software.
  
* The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).

* If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.

* The user approves (or their software silently approves) a particular transaction type at the first website.

* The user is given an approved access token (notice it’s no longer a request token).

* The user gives the approved access token to the first website.

* The first website gives the access token to the second website as proof of authentication on behalf of the user.

* The second website lets the first website access their site on behalf of the user.

* The user sees a successfully completed transaction occurring.

* OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).

1. What is OpenID?

`human verification / to check for bots `


## Authorization and Authentication flows

1. What is the difference between authorization and authentication?
![authorization and authentication](https://i.imgur.com/LAcjYuX.png)


2. What is Authorization Code Flow?

![authorization](https://images.ctfassets.net/cdy7uua7fh8z/2nbNztohyR7uMcZmnUt0VU/2c017d2a2a2cdd80f097554d33ff72dd/auth-sequence-auth-code.png)


3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

![Auth with proof](https://images.ctfassets.net/cdy7uua7fh8z/3pstjSYx3YNSiJQnwKZvm5/33c941faf2e0c434a9ab1f0f3a06e13a/auth-sequence-auth-code-pkce.png)

4. What is Implicit Flow with Form Post?
![Implicit](https://images.ctfassets.net/cdy7uua7fh8z/6m0uE4E7Hpzbdhyh9dEuYK/e36c910ff47a7540bf27e23c02822624/auth-sequence-implicit-form-post.png)

5. What is Client Credentials Flow?

With machine-to-machine (M2M) applications, such as CLIs, daemons, or services running on your back-end, the system authenticates and authorizes the app rather than a user. For this scenario, typical authentication schemes like username + password or social logins don't make sense. Instead, M2M apps use the Client Credentials Flow, in which they pass along their Client ID and Client Secret to authenticate themselves and get a token.


6. What is Device Authorization Flow?

With input-constrained devices that connect to the internet, rather than authenticate the user directly, the device asks the user to go to a link on their computer or smartphone and authorize the device. This avoids a poor user experience for devices that do not have an easy way to enter text.

![device](https://images.ctfassets.net/cdy7uua7fh8z/1A6jpG3W1H6SC9ZK92NyKd/40af53209f90a7c392f621f329fb4424/auth-sequence-device-auth.png)

7. What is Resource Owner Password Flow?
   
   Though we do not recommend it, highly-trusted applications can use the Resource Owner Password Flow , which requests that users provide credentials (username and password), typically using an interactive form. Because credentials are sent to the backend and can be stored for future use before being exchanged for an Access Token, it is imperative that the application is absolutely trusted with this information

![password](https://images.ctfassets.net/cdy7uua7fh8z/4EeYNcnVX1RFcTy5z4lP4v/c3e4d22e6f8bf558caf07338a7388097/ROP_Grant.png)
