Perpheral Security 

* wireless keyboards and mice
	* many comm in the clear
		* use proprietary protocol 
		* over 2.4 GHz frequencies
	* easy to capture with a receiver 
		* inject keystrokes and mouse movement 
		* control the computer remotly
		* vuln called "Keysniffer"
	* some keyboard manufafctures are using AES
* electromagnetic radiation 
	* view info on a screen by eavesdropping the EM signals 
	* internal signals of a laptop or external cable
* firmware hacks
	* many displays have no security for firware updates
	* log info on the screen
	* ransomeware with an LCD display
	* make a man in the middle firmware with a backdoor
* wifi enabled microSD cards
	* combination of SD flash storage device and 802.11 wifi transfers 
	* SD card auth vuln
		* predictable access, easy to read files over wifi
	* API access to the SD card
		* not a well secured SD card
* printers/multi-functional devices
	* printers, scanners, fax, network connectivity, local storage
	* reconnaissance 
		* log files for all activity, address books
	* unauth access
		* prints without auth
	* gather info
		* capture spool files 
* external storage devices 
	* storage outside the computer and often removable 
	* limited auth
		* anyone can read and connect
		* always use file/volume encryption 
	* often used for exfiltration of data
		* manage the use of removal storage 
* digital camera 
	* devices operates as an external storage 
	* camera firmware can be compromised 
		* security camera are also vuln