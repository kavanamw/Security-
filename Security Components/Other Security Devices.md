Other Security Devices 

* SSL Accelerators 
	* used because asymmetric encryption is hard 
	* moves the encryption process to a seperate server from the web server 
	* the SSL handshake uses asymmetric encryption 
		* transfers the symmetric key using the asymmetric encryption 
	* offload the handshake process to hardware 
		* SSL offload, SSL termination 
	* may not encrypt between the Accelerator and the web server 
* SSL/TLS decryption
	* commonly used to examine outgoing SSL
	* decrypt it, look for malicious stuff, reencrypt it 
	* possible with the trust relationship between your browser and the website
* browser contains list of trusted Certificate Authorities 
	* will only trust a website if it is in a known Certificate Authoritie
	* pay to be added to the cert auth
	* the CA has preformed some security checks 
* SSL Proxy 
	* user comm to third part website 
	* inside the firewall is an internal CA certificate 
	* laptop has the internal as trusted
	* firewall duplicates the whole process allowing it to decrypt and reincrypt stuff 
	* certificate listed as "internal" then you have a SSL proxy somewhere
* Hardware Security Module (HSM)
	* high end cryptographic hardware 
		* plugin card or seperate hardware device 
	* key backup
	* cryptographic accelerators 
		* offload that VCPU overhead
	* used in large environments 
		* clusterless, redundent power
* Media Gateway
	* converts beween PSTN (public switched telephone network) and VoIP
		* ISDN trunk on one side, eithernet with VoIP on the other 
		* SIP on one side, H.323 on the other 
	* security is a conver
		* disable all voice comm
		* make outbound calls 