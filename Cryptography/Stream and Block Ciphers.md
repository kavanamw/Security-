Stream and Block Ciphers 

* steam ciphers
	* encryption is done one bit or byte at a time 
		* high speed, low hardware need
	* used with symmetric encryption 
		* not asymmetric because of the overhead 
	* the starting state should never be the same twice 
		* key is often combines with an Initalization vector (IV)
* block ciphers 
	* encrypted fixed-length groups 
		* often 64 bit or 128 block 
		* pad to added to fixed length 
		* each block is encrypted or decrypted indenpendently 
	* symmetric encryption 
		* simmilar to steam ciphers 
	* block ciphers modes of operations 
		* avoid patterns in encryption 
		* many different modes to choose from 
		* ![7b06893f4b690b450aadc82580834ae5.png](../../_resources/0bec834747734984a1de755aeb2457ff.png)
	