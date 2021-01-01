# Top REST API Security Threats

[Top 7 REST API Security Threats](https://blog.restcase.com/top-7-rest-api-security-threats)


#### Man in the Middle Attack with WIFI Pineapples

* [Silicon Valley Wi-Fi Pineapple MiM Attack](https://www.thesslstore.com/blog/silicon-valley-wi-fi-pineapple/#:~:text=The%20next%20step%20is%20to,server%20and%20the%20user's%20device)


#### API Security Mechanisms

* mTLS

* x509

[**OAuth2 - Authorization**](https://www.youtube.com/watch?v=t4-416mg6iU)

* OAuth 2 is an authorization framework that enables applications to obtain limited access to user accounts on an HTTP service, such as Facebook, GitHub, and DigitalOcean. It works by delegating user authentication to the service that hosts the user account, and authorizing third-party applications to access the user account. 

[**OpenID Connect - Authentication**](https://auth0.com/docs/protocols/openid-connect-protocol):

* OpenID Connect (OIDC) is an identity layer built on top of the OAuth 2.0 framework. It allows third-party applications to verify the identity of the end-user and to obtain basic user profile information. OIDC uses JSON web tokens (JWTs), which you can obtain using flows conforming to the OAuth 2.0 specifications. See our OIDC Handbook for more details.
* While OAuth 2.0 is about resource access and sharing, OIDC is about user authentication. Its purpose is to give you one login for multiple sites. Each time you need to log in to a website using OIDC, you are redirected to your OpenID site where you log in, and then taken back to the website. For example, if you chose to sign in to Auth0 using your Google account then you used OIDC. Once you successfully authenticate with Google and authorize Auth0 to access your information, Google sends information back to Auth0 about the user and the authentication performed. This information is returned in a JWT. You'll receive an access token and if requested, an ID token.

[**SAML**]

* You’ve more likely experienced SAML authentication in action in the work environment. For example, it enables you to log into your corporate intranet or IdP and then access numerous additional services, such as Salesforce, Box, or Workday, without having to re-enter your credentials. SAML is an XML-based standard for exchanging authentication and authorization data between IdPs and service providers to verify the user’s identity and permissions, then grant or deny their access to services.

[**JWT/JWE**](https://jwt.io/introduction)

* JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.
* Although JWTs can be encrypted to also provide secrecy between parties, we will focus on signed tokens. Signed tokens can verify the integrity of the claims contained within it, while encrypted tokens hide those claims from other parties. When tokens are signed using public/private key pairs, the signature also certifies that only the party holding the private key is the one that signed it.

* PEP/PDP

* WS-Security

**Basic Auth**

* Basic authentication is a simple authentication scheme built into the HTTP protocol. The client sends HTTP requests with the Authorization header that contains the word Basic word followed by a space and a base64-encoded string username:password. 
```Authorization: Basic ZGVtbzpwQDU1dzByZA==```
Note: Because base64 is easily decoded, Basic authentication should only be used together with other security mechanisms such as HTTPS/SSL.

* ABAC/RBAC based policies

[**Tokens**](https://auth0.com/docs/tokens)



* [Difference between Oauth, OpenID Connect and SAML](https://www.okta.com/identity-101/whats-the-difference-between-oauth-openid-connect-and-saml/)
