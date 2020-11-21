Cryptographic Attacks

* attacks
	* known plaintext attack
		* attacker has encrypted info and some of the plaintext 
		* may be able to break down the crypt based on the known plaintext
		* plaintext called the crib 
	* password hash
		* if given the password hard you can brute force guess until the hash matches 
	* rainbow tables
		* an optimized pre-built set of hashes 
		* great speed increase 
		* won't work with salted hashes 
	* Dictionary attacks
		* people use common words as passwords, use the common words first 
		* equal to a wordlist 
		* catch low handing fruit 
	* brute force 
		* online 
			* keep trying the login screen
			* very slow
			* most account will lock after a number of failed attempts
		* offline 
			* obtain the list of users and hashes 
			* calculate a password hash, compare it to a stored hash
			* large resource requirment 
	* Birthday attack
		* in a class of 23 chance of same birthday?
		* 50%
		* for a class of 30 is 70%
		* in the digital work is known as a hash collusion 
	* Downgrade attack
		* instead of using good encryption use someting that not as good
		* force the system to downgrade their security 
	* Replay attack
		* some more susceptible than others
		* hash with no salt, no id tracking, no encryption
		* replay countermeasure may be part of the cryptography 
			* Kerberos includes times stamps 
			* anything after the time to live (TTL) is discarded 