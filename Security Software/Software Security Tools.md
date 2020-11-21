Software Security Tools

* Passive tools
	* watch the packets go by 
* Active tool
	* send traffic to a device, watch the results 
	* try exploits 
	* query pages
* Protocol Analyzers 
	* solve complex app
	* gathers packets on the network
	* id unknown traffic 
	* vcerify packet filtering and security tools
	* store the data for later
* Network scanner
	* active - scan for IP addresses and open ports 
		* operating system
	* pick a range of IP addresses 
	* visually map the network 
		* zenmap 
			* shows IP, services, OS
		* nmap
		* angry IP scanner
	* rouge system detection 
* Wireless scanners and crackers
	* wireless monitoring 
		* packet capturing 
	* wireless attacks 
		* check your own access points for vulns
	* cracking 
		* try to crack your own password
* Password crackers
	* hash - on way function 
	* passwords often stored as hashes 
	* use wordlists or rainbow tables 
* vuln scanners 
	* did you miss a security patch?
	* minimally invasive, still active 
	* check for bad configs 
* exploitation framework 
	* use anything they can
	* exploits can be written with a framework to make exploit development easier 
		* BeEf
		* RouterSploit
		* Metasploit
* data sanitization tools
	* when upgrading drive makes sure the old drive is wiped throughly 
	* overwrite data one or more times to make sure data is gone 
	* Darik's boot and nuke (dban)
	* Microsoft's SDelete (for single files or folders)
	* don't forget cache or temp files 
* Steganography tools
	* concelied writing hidden in an image 
	* network based
		* embeded messages in TCP packets 
	* image basesed
		* embedded in the message itself
	* invisuble watermarks
		* yellow dots to make what printer printed that document 
* Honeypot
	* attract the bad guys 
	* the bad guys are often machiens, easy for them to make a mistake
	* could be as complicated as an entire company 
	* projecthoneypot.org
	* honeyd
* backup tools
	* protect from unexpected downtime
	* real-time file sync 
		* rsync
	* regaular partial backups
	* sometimes do full backups 
* Banner grabbing
	* applications can tell you a lot more about the server than you would expect 
	* nmap grabs these 