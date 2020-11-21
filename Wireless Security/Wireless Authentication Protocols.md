Wireless Authentication Protocols 

* EAP (Extensible Authentication Protocol)
	* an auth frameowkr 
	* many different ways to authenticate based on RFC standards
	* WPA and WPA2 use 5 different EAP types as authentication mechanims 
	* EAP types
		* EAP-FAST (EAP Flexable Authentication via Secure Tunneling)
			* cisco's proposal to replace LEAP (Lighweight EAP - previously used with WEP)
			* lightweight and secure 
		* EAP-TLS (EAP Transport Layer Security)
			* Strong security, wide adoption
			* support from most of the industry
		* EAP-TTLS (EAP Tunneled Transport Latered Security)
			* support other authentication protocols in a TLS tunnel
			* use any authentication you can support, maintain seucrity with TLS
* PEAP (Protected Extensible Authentication Protocol)
	* created by cisco, microsoft, and RSA security 
		* combined a secure channel and EAP
	* commonly implemented as PEAPv0/EAP-MSCHAPv2
		* auth to microsoft's MS-CHAPv2 databases  
* 802.1X
	* IEEE 802,1X port based 
		* you don't get access until you auth 
	* used in conjunction with an access database 
		* RADUS
		* LDAP
		* TACACS+
	* supplicant - us
	* authentiator 
	* authentication server - might also contain the authenticator 
		* supplicant communicats to the authenticator but allows no network access
		* asks if this is a new authentication as an EAP requrest
		* yes we need access to the network and here is our username 
		* checks with the auth server and asks to speak to the supplicant privatly 
		* authentictor ask the end user and the end user sends the auth stuff to the auth server 
		* if the access detials are good then it lets the device on the network 
* RADIUS Federation
	* use RADIUS with federation 
		* members of one org can auth to the network of another 
		* use their normal creds 
	* use 802.1X as the auth method 
		* and RADIUS on the backend 
		* EAP to auth
	* driven by eduroam (education roaming)
		* visiting professors signing in with their local accounts on a new network 