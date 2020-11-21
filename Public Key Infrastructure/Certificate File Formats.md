Certificate File Formats 

* X.509 digital certs 
	* the structure of the cert is standarized 
	* the format of the actual cert file can take many different forms 
	* there are many cert file formats 
		* you can convert between many of the formats 
		* use OpenSSL or a similar app to view the cert contents 
* DER (Distinguished Encoding Rules)
	* format designed to transfer syntax for data structures 
		* a very specific encoding format 
		* perfect for X.509 cert 
	* binary format 
		* not human readable 
	* a common format 
		* used across many different platforms 
		* often used with java certs 
* PEM (Privacy-Enhanced Mail)
	* a very common format 
		* generally the format provided by CAs 
		* supported on many differnt platoforms 
	* ASCII format 
		* letters and numbers 
		* easy to email
	* readable 
* PKCS #12
	* Public key Cryptography standards # 12 
	* personal information exchange syntax standard 
		* developed by RSA Security, now an RFC standard
	* container format for many certificates 
		* store many X.509 certificates in a single .p12 file 
		* often used to transfer a private and public key pair 
		* the container can be password protected
	* exteneded from Microsft .pfx format 
		* the two standards are very similar 
		* often referenced interchangeable 
* CER (certificate file)
	* primarlly a windows x.509 file extension 
		* can be encoded as binary DER format or as the ASCII PEM format 
	* usually contains a public key 
		* private keys would be transferred in the .pfx file format 
		* common format for windows certs 
			* look for the .cer extension 
* PKCS #7
	* pulic key cryptography standards #7
	* cryptographic message syntax standard 
		* associated with the .p7b file
	* stored in ASCII format 
		* human readable 
	* contains certs and chain certs 
		* private keys are not included in a .p7b
	* wide platform support 
		* windows
		* java tomcat 