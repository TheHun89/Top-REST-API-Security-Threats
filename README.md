# Top REST API Security Threats

[Top 7 REST API Security Threats](https://blog.restcase.com/top-7-rest-api-security-threats)


#### Man in the Middle Attack with WIFI Pineapples

* [Silicon Valley Wi-Fi Pineapple MiM Attack](https://www.thesslstore.com/blog/silicon-valley-wi-fi-pineapple/#:~:text=The%20next%20step%20is%20to,server%20and%20the%20user's%20device)


#### API Security Mechanisms

* mTLS

* x509

[**OpenID Connect**](https://auth0.com/docs/protocols/openid-connect-protocol):

* OpenID Connect (OIDC) is an identity layer built on top of the OAuth 2.0 framework. It allows third-party applications to verify the identity of the end-user and to obtain basic user profile information. OIDC uses JSON web tokens (JWTs), which you can obtain using flows conforming to the OAuth 2.0 specifications. See our OIDC Handbook for more details.
While OAuth 2.0 is about resource access and sharing, OIDC is about user authentication. Its purpose is to give you one login for multiple sites. Each time you need to log in to a website using OIDC, you are redirected to your OpenID site where you log in, and then taken back to the website. For example, if you chose to sign in to Auth0 using your Google account then you used OIDC. Once you successfully authenticate with Google and authorize Auth0 to access your information, Google sends information back to Auth0 about the user and the authentication performed. This information is returned in a JWT. You'll receive an access token and if requested, an ID token.

[**JWT/JWE**](https://jwt.io/introduction)

* JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.
Although JWTs can be encrypted to also provide secrecy between parties, we will focus on signed tokens. Signed tokens can verify the integrity of the claims contained within it, while encrypted tokens hide those claims from other parties. When tokens are signed using public/private key pairs, the signature also certifies that only the party holding the private key is the one that signed it.

* OAuth2

* PEP/PDP

* SAML

* WS-Security

* Basic Auth

* ABAC/RBAC based policies

[**Tokens**](https://auth0.com/docs/tokens)
