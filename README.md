# Top REST API Security Threats

[Top 7 REST API Security Threats](https://blog.restcase.com/top-7-rest-api-security-threats)


#### Man in the Middle Attack with WIFI Pineapples

* [Silicon Valley Wi-Fi Pineapple MiM Attack](https://www.thesslstore.com/blog/silicon-valley-wi-fi-pineapple/#:~:text=The%20next%20step%20is%20to,server%20and%20the%20user's%20device)


### API Security Mechanisms


[**mTLS**](https://wott.io/blog/tutorials/2019/09/09/what-is-mtls)

* mTLS is just an extension of TLS (Transport Layer Security). This is commonly found in verifying endpoints and for encrypting communications and for TLS specifically, browsers. The ‘HTTPS’ in a URL is the evidence for this. This part of the URL verifies the identity of the server (the website you’re accessing), to you the client. Unlike a password which is manually entered by a single user, TLS is typically managed by cryptographic certificates. Most TLS protocols usually verify this with an x509 certificate; and it’s typically the client requesting a valid certificate from the server (DNS name on server must match that of the certificate). Secure Sockets Layer (SSL) security is also based off this principle and HTTPS is its successor.
* The main thing that makes mTLS different (and arguably more secure) is that it requires both the server and client to verify each other: a handshake. This is particularly useful in a scenario where you are the server and not the client.


**x509**

* X.509 is a standard format for public key certificates, digital documents that securely associate cryptographic key pairs with identities such as websites, individuals, or organizations.  Many of the certificates that people refer to as Secure Sockets Layer (SSL) certificates are in fact X.509 certificates.


[**OAuth2 - Authorization**](https://www.youtube.com/watch?v=t4-416mg6iU)

* OAuth 2 is an authorization framework that enables applications to obtain limited access to user accounts on an HTTP service, such as Facebook, GitHub, and DigitalOcean. It works by delegating user authentication to the service that hosts the user account, and authorizing third-party applications to access the user account. 


[**OpenID Connect - Authentication**](https://auth0.com/docs/protocols/openid-connect-protocol):

* OpenID Connect (OIDC) is an identity layer built on top of the OAuth 2.0 framework. It allows third-party applications to verify the identity of the end-user and to obtain basic user profile information. OIDC uses JSON web tokens (JWTs), which you can obtain using flows conforming to the OAuth 2.0 specifications. See our OIDC Handbook for more details.
* While OAuth 2.0 is about resource access and sharing, OIDC is about user authentication. Its purpose is to give you one login for multiple sites. Each time you need to log in to a website using OIDC, you are redirected to your OpenID site where you log in, and then taken back to the website. For example, if you chose to sign in to Auth0 using your Google account then you used OIDC. Once you successfully authenticate with Google and authorize Auth0 to access your information, Google sends information back to Auth0 about the user and the authentication performed. This information is returned in a JWT. You'll receive an access token and if requested, an ID token.


**SAML**

* You’ve more likely experienced SAML authentication in action in the work environment. For example, it enables you to log into your corporate intranet or IdP and then access numerous additional services, such as Salesforce, Box, or Workday, without having to re-enter your credentials. SAML is an XML-based standard for exchanging authentication and authorization data between IdPs and service providers to verify the user’s identity and permissions, then grant or deny their access to services.


[**JWT/JWE**](https://jwt.io/introduction)

* JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.
* Although JWTs can be encrypted to also provide secrecy between parties, we will focus on signed tokens. Signed tokens can verify the integrity of the claims contained within it, while encrypted tokens hide those claims from other parties. When tokens are signed using public/private key pairs, the signature also certifies that only the party holding the private key is the one that signed it.


[**Policy: PAP, PDP, PEP, PIP**](https://www.yenlo.com/blog/api-policies-pap-pdp-pep-and-pip.-oh-my)


[**WS-Security**](https://www.soapui.org/docs/soapui-projects/ws-security/)

* Web Services Security (WS Security) is a specification that defines how security measures are implemented in web services to protect them from external attacks. It is a set of protocols that ensure security for SOAP-based messages by implementing the principles of confidentiality, integrity and authentication.


**Basic Auth**

* Basic authentication is a simple authentication scheme built into the HTTP protocol. The client sends HTTP requests with the Authorization header that contains the word Basic word followed by a space and a base64-encoded string username:password. 
```
Authorization: Basic ZGVtbzpwQDU1dzByZA==
```
Note: Because base64 is easily decoded, Basic authentication should only be used together with other security mechanisms such as HTTPS/SSL.


[**Attribute and Role Based Access Control**](https://www.okta.com/identity-101/role-based-access-control-vs-attribute-based-access-control/)


[**Tokens**](https://auth0.com/docs/tokens)
