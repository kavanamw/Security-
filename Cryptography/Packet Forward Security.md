Packet Forward Security 

* traditional web server encryption 
	* SSL/TLS uses encryption keys to protect web server comm
		* traditionally this is based on the web server's RSA key pair 
		* one key that encrypts all symmetric keys 
	* this server's private key can rebuild everything 
		* if you capture all of the traffic, you can decrypt all of the data 
	* one point of failure for all of your web site encryption 
* perfect forward secrecy (PFS)
	* change the method of key exchange 
		* don't use the server's private RSA key 
	* elliptic curve Diffie-Hellman ephemeral 
		* the session keys aren't kept around 
	* can't decrypt with the private server key 
		* every session uses a different private key for the exchange 
	* PFS requires mor computing power 
		* not all servers choose to use PFS
	* the browser must support PFS