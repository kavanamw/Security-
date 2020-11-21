Cryptography Concepts 

* crypto 
	* Greek for "kryptos"
		* hidden, secret 
	* confidentiality 
	* authentiacion and access control 
	* non-repudiation 
		* you said it, you can't deny it 
	* integrity 
		* tamper proof 
* crypto terms 
	* plaintext 
		* an unencrpyted message, in the clear 
	* ciphertext 
		* an encrypted message 
	* cipher 
		* the alogrithm used to encrypt and/or decrypt 
	* cryptanalysis 
		* the art of cracking encryption 
		* researchers are constantly trying to find weaknesses in ciphers 
			* a mathematically flawed cipher is bad for everyone 
* cryptograhic keys 
	* keys 
		* add the key to the cipher to encrypt 
		* larger keys are generally more secure 
	* some encryption methods only use one key 
		* some use more than one key 
		* every method is a bit different 
* confusion and diffusion 
	* encryption is based on confusion and diffusion 
	* confusion 
		* the encrypted data is drastically different than the plaintext 
		* the process is non-linear, no discernible patterns 
	* diffusion 
		* change one character of the input and many characters change of the output 
* security through obscurity 
	* security should exist, even if the attacke knows everything about the sytem 
		* security of the design shouldm't be the main method of security 
		* encryption key would be the only unknown 
	* substution cipher (Ceasear cipher)
		* ROT13 
	* if you know how the security is designed, you can circumvent it 
		* SSID broadcast supproession, MAC filters
* random numbers 
	* cryptoghraphy relies on randomness 
		* used to generate keys, salt hashes, and much mroe 
	* random number generator 
		* very hard to create true randomness with a program
		* usually includes some type of natural input 
		* mouse movements, atmospherics noise, lava lamp 
	* pseudo-randomness doesn't rely on the natural worl
		* aproximate true randomness 
		* based on a starting seedz 
			* you have the seed, you have the number 
* app dev and crypto 
	* devs don't need  to be cryptographers 
		* use an API
	* the API does the heavy lifing 
		* send plaintext into box, get ciphertext back 
	* Windows has Cryptographic Service Provider (CSP)
		* the microsoft CryptoAPI is the bridge between the app and the CSP 