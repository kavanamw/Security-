PKI components 

* PKI (Public Key Infrastucture)
	* policies, procedures, hardware, software, poeple 
		* digital certs, create, distribute, manage, store, revoke 
	* this is a big big thing 
		* lots of planning 
	* also referes to the binding of public keys to people or devices 
		* the cert authority 
		* it's all about trust 
* the key management lifecycle 
	* key generation 
		* create a key with the reuqested strength using the proper cipher 
	* cert generaotr 
		* allocate a key to a user
	* distribution 
		* make the key available to the user 
	* storage 
		* securly store and protect using unauthorized use 
	* revocation 
		* manage keys that may have been compromised
	* expiration 
		* a cert may only have a certian "shelf life"
* digital certs 
	* a public key cert 
		* binds a public key with a digital signature 
		* and other detials about he key holder 
	* a digital signature adds trust 
		* PKI uses cert authority for additional trust 
		* Web oof trust adds other users for additional trust 
	* certificate creation can be built into the OS 
		* part of windows 
* what's in a digital cert 
	* the digital cert format has a format called the X.509 
	* ![8c2e6f2e46c66e2c73be6da790b54558.png](../../_resources/2c6b118cb8ce493f9e0168f2f0678e85.png)
* certificate extensions 
	* add more information to a digital cert 
		* extends the functionality and use of the cert 
	* standard extensions 
	* ![5854ab12995f2f29591bc45c85f39fdc.png](../../_resources/078b977c689242898fdf956e12f5a986.png)
* commercial certificate authorities 
	* built-in to your browser 
	* purchase your web site certificate 
		* it will be trusted by everyone's browser 
	* create a key pair, send the public key to the CA to be signed 
		* a certificate signing request (CSR)
	* may provide different levels of trust and additional features 
		* add a new "tag" to your web site 
* private certificate authorities 
	* you are your own CA 
		* built in-house 
		* your devices must trust the internal CA
	* needed for medium-to-large orgs 
		* many web servers and priacy requirements 
	* implemeneted as part of your overall computing strategy 
		* built into windows or OpenCA
* PKI trust relationship 
	* single CA 
		* everyone receives their certificates from one authority 
	* hierarchical 
		* single CA issues certs to interdediate CAs 
		* distribute the certificate management load 
		* easier to deal with the revocation of an intermediate CA than the root CA 
		* ![480d9214ae666d94e4c01a31c3b05c0b.png](../../_resources/fe57c0e9a1f142fc8c05d171aa325287.png)
* key revocation 
	* Certificate Revocation List (CRL)
		* maintained by the certificate authority 
	* many different reasons 
	* april 2014 
		* heartbleed 
		* OpenSSL flaw put the private key of affected web servers at risk 
		* OpenSSL was patched, every web server certificate was replaced
		* older certs were moved to the CRL
* Getting revocation detials to the browser 
	* OCSP (Online Certificate Status Protocol)
		* the browser uses to check the status of a cert 
	* messages usually sent to an OCSP responder via HTTP
	* not all broswers/apps support OCSP
		* early internet explorer didnt support 
		* some support OSCP, but don't bother checking for a revoked cert