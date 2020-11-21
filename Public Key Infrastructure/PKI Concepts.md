PKI Concepts

* online and offline CAs
	* a compromised certificate authority 
		* a very very bad thing 
		* no certificates issues by that CA can be trusted
	* distribute the load 
		* then take the root CA offline and protect it 
		* ![92b6955f2478247d0420100d0d3613fb.png](../../_resources/066f11017e8749c2a1f86ce5e2f6de8d.png)
* OCSP stapline 
	* online certificate status protocol 
		* providesscalability for OCSP checks 
	* the CA is responsible for responding to all client OCSP requests 
		* this does not scale well
	* instead, have the certificate holder verify their own status 
		* status info is stored on the certificate holder's server 
	* OCSP status is "Stapled" into the SSL/TLS handshake 
		* digitally signed by the CA 
* Pinnging 
	* you're communicating over TLS/SSL to a server 
		* how do you know its the right server
	* "pin" the expected certificate or public key to an application 
		* compiled in the app or added to it's first run 
	* if the expected certificate or public key doesn't match the app can decide what to do 
		* shut down, show a message
* PKI trust relationships 
	* single CA 
		* everyone recieves their certificate from one authority 
	* hierarchial 
		* single CA issues certs to intermediate CAs 
	* mesh 
		* cross-certifying CAs
		* doesn't scale well
		* ![18de4aee1a4564c6b91dbf1c29818358.png](../../_resources/dab74affb77b43e8ac6fc5f76220a3e0.png)
	* web of trust 
		* alternative to traditional PKI
		* a trust b, b trust c, a trust c
		* ![2f1fa9a31da17960c264afb3f309cf1a.png](../../_resources/09f5dec7b80240c19e95e0743263ed2a.png)
	* mutual authentication 
		* server authenticates to the client and the client authenticates to the server 
* key escrow 
	* someone else hold your decryption keys 
		* your private keys are in the hands of a 3rd party 
	* this can be a legitimate business arrangment 
		* a business might need access to employee information 
		* goverment agencies may need to decrypt partner data
	* it's all about the process
		* need clear processes and procedures 
			* keys are incredibly important pieces of info 
		* you must be able to trust your 3rd part 
		* carfully controlled confitionals 
			* legal stuff and courts 
* certificate chaining 
	* chain of trust 
		* list all of the certs between the server and the root CA
	* the chain starts with the SSL certificate 
		* ends with the root CA certififcate 
	* any certificate between the SSL certificate and the root certificate is a chain certificate 
	* the web server needs to be configured with the proper chain 
		* or the end user may get an error 