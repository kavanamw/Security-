Key Stretching Algorithms  

* give weak keys a workout 
	* a weak key is a weak key 
	* make a weak key stronger by performing multiple processes 
		* hash a password, hash the hash of the password etc
		* key stretching, key strengthening 
* key strecting libs 
	* already ready for you 
	* bcrypt 
		* generates hashes from passwords 
		* an extension to the UNIX cypt lib 
		* uses blowfish cipher to perform multiple rounds of hashing 
	* password-based key derivation function 2 (PBKDF2)
		* part of RSA public key crypto standards