# How JWT Works ?
<p>When customer and clint send HTTP request to our backend sysytem which is running on spring boot container running on apache tomcat server.

> [!IMPORTANT]
>The first thing that get executed in spring application is **fillter**.And this is once only per request filter and has role to validate and check everything regarding the token or JWT token we have.

The first thing that will happen , we will have an internal cheack to cheak if we have JWT token or not.

IF the JWT token is missing we send 403 responce to clinet.

IF we have JWT token , we will start validation process.
