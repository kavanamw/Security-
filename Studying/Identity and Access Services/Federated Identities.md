Federated Identities 

* Server based auth
	* HTTP/web browser comm is stateless
		* each request is unique and has no relationship to the previous request 
	* traditially the server has kept track of logins 
		* you are assigned a session id when you login
		* server checks each time you send a request 
	* adds overhead to the server
		* hard to scale 
		* hard with redudency and cloud 
		* hard across different devices 
	* ![2ccc90d2f070f01c83c06d350f8ede15.png](../../../_resources/6d7ec97b25054fb2b848a426ad864be6.png)
* token based auth 
	* no session info stored on the server 
	* after user auth, the application sends a token to the client 
		* client stores token locally 
	* the token is provided with each request to the server 
		* server validates the token and the app continues to work noramlly 
	* ![cd85438ddd002f25cd25402a6e2909d5.png](../../../_resources/617cb8b42b7347a9a445cb17279205ed.png)
	* token can expire after a time 
	* auth process can be seperate to the app itself 
		* third party token generateion
* federation  
	* provide netowrk access to others
	* login with your google account 
* SAML (Security Assertion Markup Language)
	* open standard for auth and authorization 
		* you can auth through a third party to gain access
		* one standard does it all, sort of 
	* Shibboleth is open-source software that implements SAML to provide feferated SSO
		* SAML defines the standard that Shibboleth uses
	* no originally desined for mobile apps 
* OAuth
	* auth framework
		* determines what resources a user will be able to access
	* created by Twitter, Google, and many others 
	* not an auth protocol 
		* OpenID Connect handles the single sign-on auth
		* OAuth provides auth between applications 
	* popular, good industry support 