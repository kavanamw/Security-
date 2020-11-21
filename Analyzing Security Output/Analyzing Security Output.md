Analyzing Security Output

* Host baded IDS/IPS
	* used to be a seperate application, now part of anti-virus
	* protects based on signatures 
	* protects based on activity
		* should that file have been changed?
* antivirus 
	* alert and log malicious software 
* file integrity check
	* are the core files in place?
	* sfc /scannow (windows)
* host based firewall
	* protect against other network
	* protect wherever you go
	* restricts by applicationb and network port number
	* log displays connection attempts
* application whitelist
	* only allow specific apps
	* application hash
	* certificate 
		* only from microsoft for example
	* path 
		* only run apps in these folders 
	* network zone
* remoable media
	* USB drives, portable hdd
	* malware infections 
		* drives brought from home
		* drives in parking lot
	* data going out via usb drive
* advanced malware tools
	* speciialized removal and recovery tools 
	* malware is pervasive, has backdoors 
* patch management tools
* UTM (unified thread management/ web security gateway)
	* URL filter, content inspection
	* malware inspection
	* spam filter
	* CSU/DSU
	* router switch
	* firewall
	* IDS/IPS
	* Banwidth shaper
	* VPN endpoint
* DLP (Data Loss Prevention)
	* private info going across the network
* DEP (Data Execution Prevention)
	* No-eXecute bit
		* intel calls it the XD bit (eXecute Disable)
		* designated sections of memory as executing code or data
			* code can't run from protected memory locations 
			* prevents malware and viruses from executing 
		* os must support this feature 
			* windows calls it Data Execution Prevention 
			* enabled by default
			* all logs are in event viewer 
* WAF (Web Application Firewall)
	* not a normal firewall
	* allow or deny based on expected input 
		* unexplected input common exploit
	* a major focus on CC industry 
	* 