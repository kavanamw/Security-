Asymmetric Algorithms 

* diffie-hellman key exchange 
	* a key exchange method over an insecure comm channel 
	* publish in 1976
	* DH does not itself encrypt or auth 
		* it's anonymous key-agreement protocol
	* used for PF security 
		* ephemerical DH (EDH or DHE)
		* combine with elliptic curve cryptography for ECDHE
	* use asymmetric cryptography to create a symetric key 
	* ![d209ffcd74208452d57e660e4d79ebc7.png](../../_resources/1ad83f5d659147db8ed83923c4d1fb61.png)
		* the symmetric key is the same
* RSA (Ron Rivest, Adi Shamir, and Leonard Adelman)
	* published in 1977
	* the first practical public-key cryptography system 
		* encrypt, decrypt, digital signatures 
	* based on the product of two large prime numbers 
		* you must know the factors to decode 
	* now released into the public domain 
		* used extensivly for web site encryption and digital rights management 
* DSA (Digital Signature Algorithm)
	* a standard for digital signatures 
		* modified DH for use in digital signatures 
	* a Federal information processing standard for digital signatures 
		* initally added in 1993 and updated through the years 
	* combine with elliptic curve cryptography 
		* fast and efficient digital signatures 
		* ECDSA - Elliptic Curve Digital Signature Algorithm
*  Elliptic curve cryptography (ECC)
	* used for crypto, digital signauters, pseudo-random generators, and more 
	* asymmetric encryption 
		* traditonally need large integers composed of two or more large prime factors 
	* instead of numbers, use curves 
		* just as infeasible to find the discrete logarithm of a random elliptic curve element 
		* uses smaller keys than non-ECE encryption 
		* ellptic cuve digital signature algorithm (ECDSA)
* PGP (Pretty Good Privacy)
	* popular asymmetric encryption 
		* created by Phil Zimmerman in 1991 
		* commerial software 
		* owned by Symantec 
	* open standard OpenPGP 
		* implemented as software- GNU Privacy Guard (GPG)
			* linux, mac, windows and others 
			* very compatible with commerical PGP