Hashing and Digital Signatures 

* hashes 
	* rep data as a short string of text 
		* refered to as a message digest 
	* one-way trip 
		* impossible to recover the original message from the digest 
		* used to store passwords 
	* verify a downloaded document is the same as the og 
	* can be used as a digital signature 
	* two different messages will not have the same hash
		* called a hash collision when it happens 
* a hash example 
	* SHA256 
		* 256 bits/64 hex character 
* collision 
	* hash functions 
		* take an input of any size 
		* create a fixed size string 
		* message digest, checksum
	* the hash should be unique 
		* different inputs should never create the same hash 
		* if they do it's called a collision
* practical hashing 
	* verify a downloaded file 
		* hashes may be provided on a download site 
		* compare the downloaded file hash with the posted hash 
	* password storage 
		* instead of storing passwors, store the salted hash 
		* compare hashes during auth process
		* no one ever knows your actual password
* digital signatures 
	* prove a message was not changed 
	* prove the source of the message 
		* auth
	* make sure the signature isn't fake 
		* non-reputable 
	* sign with a private key 
		* the message doesn't need to be ecnrypted 
		* no one else can sign this 
	* verify with my public key 
	* ![8b976a6b223d729c33eda341976167ad.png](../../_resources/6540df8dc85c4a7a84f54706f79b7613.png)
	* ![413ceca8f2a2c11cc53a93180c737d1a.png](../../_resources/4bba9749c3cb44148da86bad3711410c.png)
* 