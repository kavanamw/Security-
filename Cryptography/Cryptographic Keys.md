Cryptographic Keys

* cryptographic keys 
	* there's very little that isn't known about the cryptographic process
		* the algo is well known
		* the only thing you don't know is the key 
	* the key determines the output 
		* encrypted data 
		* hash value 
		* digital signature 
	* keep your key private 
		* it's the only think protecting your data 
* key strength 
	* larger keys tend to be more secure 
		* prevent brute-force attacks 
		* attackers can try every possible key combo 
	* symmetric encryption 
		* 128 bit or larger symmetric keys are common 
		* these numbers get larger as time goes on 
	* asymmetric encryption 
		* complex calculations of prime numbers 
		* larger keys than symmetric encryption 
		* common to see key lengths of 3,072 bits or larger 
* key exchange 
	* a logistical challenge 
		* how do you trasnfer keys across an inscure medium without having an encryption key 
	* out-of-band key exchange 
		* don't send the symmetric key over the 'net'
		* telephone, courier, in-person, etc
	* in-band key exchange 
		* it's on the network
		* protect the key with additional encryption 
		* use asymmetric encryption to deliver a symmetric key 
* real-time encryption/decryption 
	* there's a need for fast security 
		* without compromisisng the security part 
	* share a symmetric session key using asymmetric encryption 
		* client encrypts a random (symmetric) key with a server's public key 
		* the server decrypts this shared key and uses it to encrypt data 
		* this is the session key 
	* implement session keys carefully 
		* need to be changed often (ephemeral keys)
		* needs to be unpredictable
			* don't incriment by 1 for ex.