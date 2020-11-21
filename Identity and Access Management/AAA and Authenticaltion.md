AAA and Authenticaltion 

* identification 
	* who you claim to be 
	* usually your username 
* authentication
	* prove you are who you say you are 
	* password and other auth factors 
* authorization 
	* based on your id and auth what access do you have
* accounting 
	* resources used, login time, data sent and recieved, logout time 
* multi-factor auth
	* something you are 
		* biometric auth
		* usually stores a mathematical model of your biometric
		* difficult to change 
		* used in specific situations
	* something you have 
		* smart card 
			* may require a pin
			* itegrates with devices 
		* USB token
			* cert is on the USB device 
		* hardware or software tokens 
			* generates pseudo-random auth codes
		* you phone 
			* sms a code to your phone 
	* something you know
		* one of the most common
		* password
		* pin 
			* personal id number 
			* not typically contaied anywhere on a smart card or atm card
		* pattern
			* only you know the right format
	* somewhere you are
		* provide a factor based on your location 
		* is this a good place to allow access
		* IP address
			* not perfect but can provide a lot of info
			* works with IPv4, not with IPv6
		* mobile device location 
			* geolocation to a very specific area 
			* must be in a location that can recieve GPS info
			* not a perfect id of location 
	* something you do 
		* a personal way of doing things
		* handwriting 
			* signature comparison 
		* typing techniques 
			* delays between keystrokes
		* very similr to biometrics 
	* can be expensive 
		* seperate hardware tokens 
		* scanning equipment 
	* can be inexpensive 
		* phone app
* federation 
	* provide network aceess to others 
	* third parties fcan establish a federated network 
		* auth between two organizations 
		* loging with your google account on another site
	* third parties must establish a trust relatonship
		* no pasing of passwords
* single sign on (sso)
	* auth one time, gain access to everything 
	* saves tiem 
		* seamlesss
		* end-user doesn't see any of the complexities under the surface 
	* methods
		* kerberos 
		* 3ed party options 
* transtive trust 
	* one way trust 
		* domain B trusts domain A but not in the other direction 
	* two way trust
		* equal trust 
	* non-transitive trust 
		* a trust is specifically created and applies only to that domain 
	* transtive trust 
		* domain A trusts domain B, domain B trust C, thereforce domain A trusts domain C
* 