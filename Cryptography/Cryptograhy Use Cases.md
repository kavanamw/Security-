Cryptograhy Use Cases

* finding the balance 
	* low power devices
		* mobile devices, portable systems 
		* smaller symmetric key sizes 
		* use elliptic curve crypto for asymmetric encryption 
	* low latency 
		* fast computation time 
		* symmetric encryption, smaller key sizes 
	* high resiliency 
		* larger key sizes 
		* encryption algo quality 
		* hashing provides data integrity 
* use cases 
	* configentiality 
		* secrecy and privacy 
		* encryption (file, drive, email)
	* integrity 
		* prevent modifications of data 
		* validate the contents with hashes 
		* file downlaods, password storage 
	* obfuscation 
		* modern malware 
		* encrypted data hide the active malware code 
		* decryption occurs during execution 
	* authentication 
		* password hashing 
		* protect the original password 
		* add salts to randomize the stored password hash 
	* non-repudiation 
		* confirm the authenticity of data 
		* digital signautres provides both integrity and non-repudiation 
	* resource vs. security constraints 
		* an ongoing battle 
		* browser support vs supported encryption 
		* VPN software support vs supported algos 