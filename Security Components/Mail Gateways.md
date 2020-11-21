Mail Gateways 

* stopping unsolicited emails 
	* stop it before it gets to the user 
	* on site or cloud based
* email filtering 
	* inbound or outbound 
	* unsolicited email ads 
	* control of phishing attempts 
	* anti-virus to block bad attachments 
	* DLP block confidential info at the gateway
* id spam
	* whitelist 
		* only receive email from trusted sender 
	* SMTP standard checking 
		* block anytthing that doesn't follow RFC standards
	* rDNS - reverse DNS
		* block email where the sender's domain doesn't match the IP address
	* Tarpitting 
		* intentionally slow down the server conversation 
		* slow spammers who want to go fast
	* recipient filtering 
		* block all email not addressed to a valid recipient 
* email encryption
	* useful for sensitive info
	* not always automatic 
	* encryption can be required on the gateway 
		* force the encryption, send a password to the sender 
		* send a text message to the recipient 
	* many email clients support encryption 