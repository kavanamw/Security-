States of Data

* data in-transit 
	* data transmitted over the network 
		* also called data-in-motion 
	* not much protection as it travles 
	* network-based protection 
		* firewall, IPS
	* provide transport encryption is best 
		* TLS (Transport Layer Security)
		* IPsec (Internet Protocol Security)
* data at-rest
	* the data is on a storage device 
		* herd drive, SSD, flash drive
	* encrypt the data
		* whole disk encryption 
		* databse encryption
		* file or folder level encryption 
	* apply permissions 
		* access control lists 
		* only auth users can access the data 
* data in-use 
	* the data in memory 
		* system RAM, CPU registers and cache 
	* the is almost always decrypted 
	* the bad guys can pick the decrypted info out of RAM
		* good attack option
	* ex. Target breach
		* Data at rest encryption and data in transit encryption
		* malware went on the POS system to get the data in use 