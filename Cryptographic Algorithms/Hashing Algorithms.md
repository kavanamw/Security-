Hashing Algorithms 

* MD5 message digest algorithm 
	* designed by Ronald Rivest 
	* first published 1992 
		* replaced MD4
		* 128 bit hash value 
	* 1996, vuln found 
		* not collision resistant 
	* 2008, research create CA cert that appeared legit when MD5 checked 
		* built other certs that appeared to be legit 
* SHA (Secure Hashing Algoirhtm)
	* Developed by the NSA
	* SHA-1
		* widely used 
		* 160 bit digest 
		* 2005 - collision attacks published
	* SHA-2 
		* the preferred SHA variant 
		* up to 512 bit digest 
		* SHA-1 is now retired for most US Goverment use 
* HMAC (Hash-based Message Authentication Code)
	* combine a hash with a secret key 
	* e.g. HMAC-MD5, HMAC-SHA1
	* verify data and authenticity 
		* no fancy asymmetric encryption required 
	* used in network encryption protocols 
		* IPsec, TLS
* RIPEMD (RACE Integrity Primatives Evaluation Message Digest)
	* a family of message digest algorithms 
	* RIPE (Reasech and Development in Advanced Communication Technologies)
		* from Europe 
		* created to help with integreated broadband communicatoin in Europe
		* centralized cryptographic standards and management 
	* orininal RIPEMD was found to have collision issues (2004)
		* effectively replaced with RIPEMD-160 
		* based on MD4 design but performs similar to SHA-1
		* RIPEMD-128, RIPEMD-256, RIPEMD-320
		* 