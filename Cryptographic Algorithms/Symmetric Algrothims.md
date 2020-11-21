Symmetric Algrothims 

* DES (Data Encryption Standard)
	* DES and Triple DES
	* Developed between 1972 and 1977 by IBM for the NSA
		* one of the Federal Information Processing Standards (FIPS)
		* 64 bit block cipher 
			* 56 bit key (very small in modern terms)
		* easy to brute force with today's technology
* 3DES
	* triple DES 
	* three different keys is the strongest 3DES encryption method 
		* two serperate keys is deprecated, a single key isn't allow 
	* use DES encryption/decryption three times
		* encrypt with the first key 
		* decrypt with the second key 
		* encrypt with the third key 
	* superseded by AES (Advanced Encryption Standard)
	* ![aef7a14bba62df2e296ff1fb746c2ca9.png](../../_resources/ccebcd10bd3b46848d10de704de407a8.png)
* RC4 
	* Rivest Cipher 4 
		* Ron Rivest
	* part of the ill-fated WEP standard 
		* also part of SSL, but removed from TLS
	* RC4 has a "biased output"
		* if the third byte of the og state is 0 and the second byte is not equal to 2, than the second output byte is always 0
	* not common to see RC4 these days 
		* WPA2 moved to AES
* AES (Advanced Encryption Standard)
	* US Federal Govement standard 
		* FIPS 197 in 2001
		* it took 5 years to standardize this 
		* developed by two Belgian cryptographers 
	* 128 bit block cipher 
		* 128, 192, and 256 bit keys
	* used in WPA2 
		* powerful wireless encryption 
* blowfish and twofish
	* blowfish
		* designed in 1993 by Bruce Schneier 
		* 64 bit block cipher, variable length key (1 to 448 bits)
		* no known way to break the full 16 rounds of encryption 
		* one of the frist secure ciphers not limited by patents 
	* twofish 
		* successor to blowfish 
		* 128 bit block size, key sizes up to 256
		* no patent, public domain 