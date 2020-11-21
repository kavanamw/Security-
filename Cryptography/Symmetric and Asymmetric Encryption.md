Symmetric and Asymmetric Encryption 

 * symmetric encryption 
	 * a single shared key
		 * encrypt with the key 
		 * decrypt with the same key 
		 * if it get's out, you'll need another key 
	 * secret key algorithm 
		 * a secret shared key
	 * doesn't scale very well
		 * can be challenging to distribute 
	* very fast to use 
		* less overhead than asymmetric encryption 
		* often combined with asymmetric encoryption 
	* very common to encrypt an symetric encryption with asymettic encryption 
		* ![0932708dd998e6cc13e3a39f5bfdb3aa.png](../../_resources/bd24b65729a64d059b815f47aef90502.png)
			* the key combo creates an identical key pair and encrypt with that 
* asymmetric encryption 
	* public key crypto 
		* two or more mathematically related keys 
	* private key
		* keep this private 
	* public key 
		* anyone can see
		* give it away
	* the private key is the only key that can decrypt data encrypted with the public key 
		* you can't derive the private key from the public key 
	* ![7955cea8ff9f5d507021f931b77a0796.png](../../_resources/85438b00b6ff4956ada5caba3cdacdaa.png)
* the kay pair 
	* asymmetric encryption 
		* public key 
	* key generation 
		* buid both the public and private key at the same time 
		* lots of randomization 
		* large prime numbers 
		* lots of math
	* everyone can have the public key 
		* only allice has the private key 
 * elliptic curve crypto
	 * asymmetric encryption 
		 * need large integers composed on two or more large prime factors 
	 * instead of numbers, use curves 
		 * uses smaler keys than non-ECE asymmetric encryption 
		 * smaller storage and transmission requirements 
		 * perfect for mobile devices 