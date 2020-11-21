Access Control Technologies

* proximity cards
	* close range cards 
	* passsive device 
		* powered from the reader
	* no a large data storage device 
		* often used as an identifier
		* keycard door access, library card, payment systems 
		* the identifire is linked to data stored elsewhere
* smart cards
	* integrated circiut card 
		* contact or contactless
	* common on Credit Cards
		* also used for access control
	* must have physical card to provide digital access
		* a digital cert
	* multi factor 
		* use the card with a pin or fingerprint 
* biometric factors
	* fingerprint scanners 
	* retinal scanners 
		* inquie capillary structre in the back of the eye
	* iris scanner 
	* voice recog
	* facial recog
* biometric acceptance rates 
	* false aceptace rate (FAR)
		* likelihood that an unauth user will be accepted 
		* this would be bad 
	* false rejection rate (FRR)
		* likelihood that an authorized user will be rejected 
	* crossover error rate (CER)
		* the rate at which FAR and FRR are equal
		* adjust sensitivity to equal both values 
		* used to quantitatively compare biometric systems 
* token generators 
	* pseudo-random token generators 
	* carry around a physical hardware token gen
	* software based on a phone 
* HOTP - HMAC-based one time password algo
	* one time passwords
	* token based auth 
		* the hash is different every time 
	* hardware and software tokens available 
* TOTP - time based one time password algo
	* use the secret key and time of day 
	* no incremential counter 
	* secure key is configured ahread of time 
		* timestamps are synced via NTP
	* timestamp usually increments every 30 seconds 
	* one of the more common OTP methods 
* Certificate based auth 
	* smart cards
		* private key on the card is the cert 
	* PIV (Personal Identity Verification) card
		* US Federal Goverment smart card
		* picture and id info
	* CAC (Common Access Card)
		* US Department of Defense smart card 
		* picture and id
	* IEEE 802.1X
		* gain access to the network useing a cert 
		* on device storage or separate physica device
* 