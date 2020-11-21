Weak Encryption

* the strength of encryption 
	* strong crypto vs. weak crypto 
		* it's all relative 
	* practically evrything can be brute forced 
		* try every possible key 
	* the goal is to use a key so long that it is impractical to brute force 
	* strong alogs have been around for awhile 
		* that's part of the reason they are strong 
		* Wired Equivalent Privacy (WEP) has design flaws 
	* strong algos 
		* PGP (Pretty Good Priacy), AES (Advanced Encryption Standard)
	* weak algos 
		* WEP (Design flaw), DES (Data Encryption Standard)
* give weak keys a workout 
	* a weak key is a weak key 
		* by itself, it's not very secure 
	* make a weak key stronger be preforming multiple processes
		* hash a password, hash the hash of the password, etc
		* key stretching, key strengthening 
	* brute force attacks would require reversing each of those hashes 
		* the attacker has to spend much more time, even if the key is small 