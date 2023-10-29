# JWT
JSON Web Token (JWT) is a popular user authentication standard, used to securely exchange information online. 
JWTs can be used to authorize access to resources and services.

This token is made up of three components:
1. A header that specifies the algorithm used to encrypt the contents of the token.
2. A payload that contains “claims” (information the token securely transmits).
3. A signature that can be used to verify the authenticity of the information.



## How JWT Works ?
<p>When customer and clint send HTTP request to our backend sysytem which is running on spring boot container running on apache tomcat server.

> [!IMPORTANT]
>The first thing that get executed in spring application is **fillter**.And this is once only per request filter and has role to validate and check everything regarding the token or JWT token we have.

The first thing that will happen , we will have an internal cheack to cheak if we have JWT token or not.

IF the JWT token is missing we send 403 responce to clinet.
### First call(Request)
1. IF we have JWT token , we will start validation process.(Filter like internal execution will first make a call with user details to try to fetch user information from the database and this will base on user email that we will set as claim or token subject that will extract within this JWT authentication filter).

 JWT Authentication filed will cheak the JWT token extract the username or email or we call it the subject when we talk about JWT tokens and it will use that email to fetch the user deatils information from our database.

### Secound call(Responce)
 2. Once user is fetched , we have responce from our database and the responce can be either way can be existing user or not existing user.

> [!NOTE]
> @Data annotation equelitive getter&setter , constructor and toString method.
> @Builder annotation help me to build my object in easy way.


# How Does JWT Authorization Work? 
 by encoding information into a JSON web token (JWT),then passed between the client and server.

 The steps involved in a typical JWT authorization flow are as follows:
 1. Authentication: The client sends the user’s credentials to the server.which authenticates the user and generates a JWT containing information about the user.
 2. Issuing the Token: The server sends the JWT back to the client, which stores it for future use.
 3. Sending the Token: When the client wants to access a protected resource on the server, it sends the JWT in the Authorization header of the HTTP request.
 4. Verifying the Token: The server receives the request and verifies the JWT by checking its signature using the secret key that was used to sign it.
  If the JWT is valid, the server extracts the information contained in it and uses it to determine what actions the user is authorized to perform.
  5. Authorizing the Request:  If the user is authorized to access the resource, the server returns the requested data. If the user is not authorized, the server returns an error message.