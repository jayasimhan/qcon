#API Security and Federation Patterns

APIs deal with personla/sensitive information
* confidentiality
* 
* 
* 
OAuth
* Express consent
* limit scope
* turn on/off


API Security Logical components

USer
Identity provider
Application
Authorization server
token server
policyr enforcement point
Resource server 

###Oauth client - 

#### application grant type
An application presents its own credentials to get a token. There is no user identity here. It is an application using its credentials to get access to the api.
#### password grant type
Resource owner password credentials
- for trusted apps only (the twitter ios app connecting to the twitter api)
- for public or confidential cleints
- optimal use on mobile apps.

Redirection Based Authentication

TODO write this down from the slide screenshots in phone

#### Social Login
user tries lo login -> 

* pattern specified in Openid Connect 
  * extends Oauth 2.0
  * 
* better alternative to SAML Web Browser SSO
  
#### Nested Handshakes
Your app uses an api and the api server uses another authorization server

ex: Lets say you use a twitter client but twitter uses Google to login. This is a nested handshake.

#### Federated handshakes

##### SAML Bearer Grant
app sends a SAML to the api -> the api returns a token
##### JWT Bearer Grant
app sends a JWT to the api -> the api returns a token


#### Federated 



### Attacks

##### Fishing Attacks

- Risk associated with redirection based handshakes
  - malicious application, pretends to be legitimate
  - Inserts its own endpoint in callback address
  - Gets token

Mitigation
- Do not provide a redirect uri in the url. Instead register the uri 

Public vs confidential clients
*  dont try to hide a secret in a public app
Client confidentiality strenghten's security
when an app tries to get a loca

Bearer vs HMac tokens
Trend today is towards bearer tokens. HMac tokens are used mostly internally.
Bearer tokens are easy, but use them responsibly.
Mac 
pros: 
1. no problem if a secret is intercepted.
2. safe for man in the middle attacks.
Con:
You have to keep two secrets on your server side



