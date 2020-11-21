Types of Certificates 

* root certificate 
	* the public key certificate that identifies the root CA 
		* everything starts here
	* the root certificate issues other certificates 
		* intermediate CA certififcates 
		* any other ones 
	* this is a very important cert
		* take all security precauctions 
		* access to the root certificate allows for the creation of any trusted certificate 
* web server SSL certs 
	* domain validation cert (DV)
		* owner of the certificate has some control over the DNS domain 
	* extened validation cert (EV)
		* additional checks have verified the certificate owner's identity 
		* greeen name on the address bar 
	* subject alternative name (SAN)
		* extension to an X509 cert 
		* lists additional id info 
		* allows a certificate to support many different domains 
	* wildcard domain 
		* certs are based on the name of the server 
		* a wildcard domain will apply to all server names in a domina 
		* *.professormesser.com
			* www, ftp, webserver...
	* self-signed certificates 
		* internal certificates don't need to be signed by a public CA 
			* your company is the only one going to use it 
			* no need to purchase trust for devices that already trust you
		* build your own CA 
			* issues your own certs signed by your own CA 
		* install the CA cert/trusted chain on all devices 
			* they'll now trust any certificates signed by your internal CA 
			* works exactly like a cert you purchased 
* machine and computer certificates 
	* you have to manage many devices 
		* often drvices that you'll never see
	* how can you truly auth a device?
		* put a certificate on the device that you signed 
	* other business processes rely on the cert
		* access to the remote access VPN from auth devices 
		* management software can validate the end device 
	* user certificate 
		* associate a cert wit ha user 
			* like an id card
		* use an additional auth factor 
			* limit access without the cert 
	* integrated onto smart cards 
		* use both a physical and digital access cards
* email certificates 
	* use cryptography in an email platform 
		* you'll need public key crypto 
	* encrypting emails 
		* use a recipient's public key to encrypt
	* receiving encrypted emails 
		* use your private key to decrypt
	* digital signatures 
		* use your private key to digitally sign an email
		* non-repudiation, integrity 
* code signing certifiate 
	* developers can provide a level of trust 
		* apps can be signed by the developer 
	* the user's os wlll examine the signature 
		* checks the dev signature 
		* validates that the softwware has not been modified 
	* is it from a trusted entity 
		* user sees a warning 