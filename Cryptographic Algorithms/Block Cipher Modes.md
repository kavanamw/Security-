Block Cipher Modes 

* block ciphers modes of operation
	* encrypt one fixed length group of bits at a time 
		* a block
	* mode of operation 
		* defines the method of encrpyion 
		* may provide a method of auth
	* the block size if fixed
		* not all data matche sthe block size perfectly 
		* split your plaintext into smaller blocks 
		* some modes require padding before encrypting 
* ECB (Electronic Codebook)
	* the simpliest encryption mode 
		* too simple for most use casea
	* each block is encrypted with the same key 
		* identical plaintext blocks create identical ciphertext blocks 
		* ![1211a7134f3a67b4bcab1477b861c652.png](../../_resources/b27b2e1bab29494499a7a87182745368.png)
	* ECB without a salt 
	* ![96eb959c35e7162854b381b6763811c5.png](../../_resources/0a0dca1de3c445368cb9ca5bcff1cafc.png)
* CBC (Cipher Block Chaining)
	* a popular mode of operation 
		* relaititly easy to impliment 
	* each plaintext block is XORed with the previous ciphertext block
		* adds additonal randomization 
		* use an initialization vector for the first block 
		* ![d2d03055e8dfd08761b10464d5e35fe5.png](../../_resources/3e8591ca57fa454aa546ef0e10d743d0.png)
* CTR (Counter)
	* block cipher mode/acts like a stream cipher 
		* encrypts successive values of a "counter"
	* plaintext can be any size, since it's part of the XOR
		* i.e. 8 bits at a time (steaming) instead of a 128 bit block
		* ![80db59ae90c274201e6f96e21af832d5.png](../../_resources/1c3e90fe40494f048fe25a8cf82a2b33.png)
* GCM (Galois/Counter mode)
	* encryption with auth
		* auth is part of the block mode
		* combines counter mode with Galois auth
	* minimum amount of latency, minimum operation overhead 
		* very effieient encryption and auth
	* commonly used in packetized data 
		* network traffic security (wireless, IPsec)
		* SSH, TLS