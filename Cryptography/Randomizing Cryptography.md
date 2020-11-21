Randomizing Cryptography 

* crypto without randomization 
	* ![6e5502f5a3d7a63664e5040ee35ad99e.png](../../_resources/830a0f0c9a2e42699f9a1abafcaabab1.png)
	* since theirs not randomization, the encrypted picture gives away too much info
* cryptographic nonce 
	* arbitrary number 
		* used once 
		* "for the nonce" - for the time being 
	* a random or pseudo-random number 
		* something that can't be reasonable guessed 
		* can also be a counter
	* use a nonce during the login process 
		* server gives you a nonce 
		* calculate your password hash using the nonce 
		* each password hash sent to the host will be different, so a replay won't work
* initialization vector 
	* a type of nonce 
		* used for randomizaing an encrypted scheme 
		* the more random, the better 
	* used in encryption cipher, WEP, and older SSL implimentations 
	* ![339a48bb362a8bfeaf4178b1ef0ae767.png](../../_resources/b7aadf5265d4490eb29ea4c0f13280a8.png)
* salt
	* a nonce most commonly asociated with password randomization 
		* make the password hash unpredictable 
	* password storgae should alway be slated
		* each user gets a different salt 
	* if the passwrod databsae is breached, you can't correlate any passwords 
		* even users with the same password have different hashes stored 