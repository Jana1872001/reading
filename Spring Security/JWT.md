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


