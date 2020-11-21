PAP, CHAP, and MS-CHAP

* PPP auth 
	* point to point protocol
		* analog dialup, ISDN
	* and derivatives 
		* PPTP (point to point tunneling protocol)
		* PPPoE (Point to point protocol over ethernet) - DSL auth
	* need to auth through these non-ethernet networks
		* PAP, CHAP, and MS-CHAP
* PAP (Password Auth Protocol)
	* a basic auth method 
		* used in legacy os 
		* rare to see singuarly used
	* pap is in the clear
		* weak auth scheme
		* non-encrypted password exchange
		* we didn't require encryption on analog dial-up lines 
	* ![5450d181d44704e90d7107eb4660d324.png](../../../_resources/664cf67ce1814333b65d8fb50cab625d.png)
* CHAP (Challenge Handshake Auth Protocol)
	* encrypted challenge sent over the network  
	* three way handshake
		* after link is established, server sends a challenge message
		* client responde with a password hash calculated from the challenge and the password 
		* server comapres received hash with stored hash
	* challenge-reponse continues 
		* occurs periodically during the connection 
		* user never knowns it happens 
	* ![6127eea4dd6cf003fba4fdf0055815bf.png](../../../_resources/d0b7e09cd56f4571b4dab9b928e02127.png)
* MS-CHAP (Micrsoft Challenge Handshake Auth Protocol)
	* used coimmonly on Microsfot's point to point tunneling protocol (PPTP)
	* MS-CHAP v2 is the more resent version 
	* security issues related to the use of DES
		* relativly easy to brute force the 2^56 possible keys to decrypt the NTLM hash
		* don't use MS-CHAP
		* consider L2TP, IPsec or some other secure VPN tech