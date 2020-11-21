Wireless Cryptographic Protocols 

* wireless encryption 
	* all wireless computers are radio transmitters and receivers 
		* anyone can listen 
	* solution, encrypt the data 
		* everyone gets a password
	* only people with the pasword can transmit and listen 
* WPA (WIi-Fi Protected Access)
	* 2002: WPA was the replacement for serious cryptographic weaknesses in WEP (Wired Equivalent Privacy)
	* needed a short-term bridge between WEP and whatever would be the replacement 
		* needed to run on existing hardware 
	* WPA: RC4 ciphers with TKIP (Temporal Key Itegrity Protocol)
		* initialization vector is larger and an encrypted hash 
		* every packet gets a unique 128-bit encryption key 
* TKIP
	* mixed the keys
	* adds sequence counter 
		* prevents replay attacks 
	* implements a 64 bit message integrity check 
	* TKIP has it's own set of vulns 
		* deprecated in 802.11-2012 standard 
* WPA2 and CCPM
	* WPA2 cert began in 2004 
	* AES (Anvanced Encryption Standard)
	* CCPM (Counter mode with Cipher Block Chaining Message Authentication Code Protocol) replaced TKIP
	* CCPM block cipher mode 
		* uses AES for data confidentiality 
		* 128-bit key and a 128 bit block size 
		* requires additional computing resources 
	* CCMP Securiy Services 
		* data confidentiality (AES), authentication, and access control