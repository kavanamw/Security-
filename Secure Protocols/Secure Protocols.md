Secure Protocols 

* Voice and video
	* SRTP (secure real-time transport protocol)
		* the secure verions of RTP
		* encryption using AES
		* auth integrity and replay protection 
		* HMAC-SHA1 hash based message auth
* Time 
	* NTP has no security 
		* exploit as amps in DDoS attacjs
	* NTPsec
		* secure network time protocol
		* began development in 2015
		* cleaned up the code base 
		* fixed vulns 
* email
	* S/MIME (Secure multipurpose internet mail extensions)
		* public key encryption and digital signing of mail content 
		* required PKI or similar organization of keys
	* secure POP and Secure IMAP
		* usees a STARTLS encryption to encrpyt POP3 with SSL or IMAP SSL
	* SSL/TLS
		* if the mail is browser based, always encrypt with SSL
* web
	* SSL/TLS (secure sockets layer/Transport Layer secuity)
		* usually implemented as HTTPS
			* HTTP over TLS/ HTTP over SSL/HTTP secure 
	* uses public key encryption 
	* private key on the server 
	* symmetric session key is transfered using asymmetric encryption
	* secureity and speed 
	* lock in the upper right hand correr
* file transfer
	* FTPS 9FTP over SSL
	* not SFTP
		* SSH file transfer protocol
		* also transferes files over network, but different protocol
* LDAP (lightweight Directort Access Protocl)
	* protocol for reading and writing directories over IP network
	* x.500 specification was written by the ITU
	* DAP ran on the OSI p[rotocol stack
	* LDAP used to query and update an x.500 direcetory 
		* used in windows, apple opendirectory, openLDAP, etc.
* Directory servies
	* LDAPs (LDAP Secure)
	* SASL (simple authenticaion and security layer)
		* provides authentication using many different methods i.e., kerberos or client certificate 
* remote access
	* SSH (secure shell)
		* encrypted terminal communication 
		* replaces telnet (unemcrypted)
* DNS
	* dns had no security in the original design
	* DNSSEC (domain name system security extensions)
	* validates DNS responses using public key crypto
		* origin auth
		* data integrity
	* signed DNS records are published in DNS
* routing and switching 
	* SSH 
	* SNMPv3 - simple network management protocol version 3
		* confidentiality - encrypted data
		* integrity - no tampering of data
		* auth - verifies the source 
	* HTTPS
		* browser based
		* encrypted communication 
* Network address allocation 
	* securing DHCP
		* DHCP does not include any security 
		* no secure version
	* rouge DHCP servers 
		* in AD, DHCP servers must be authorized, some form of security 
	* some switches can be configured with trusted interfaces 
	* DHCP distro is only allowed from trusted interfaces 
	* DHCP client Dos - starvation attack
		* using spofofed MAC addresses to exhause the DHCP pool
	* switches can limit the number of MAC addresses per interface 
* subscription services 
	* constant updates 
	* check for encryption and integrity checks 
		* may required an additional public key config
		* set a trusted relationship so no bad updates come in