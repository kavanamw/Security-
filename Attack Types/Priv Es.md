Priv Es

* **gain higher level access to a system via a vuln**
* often released as a critical bug
* horizontal - gaining no more access, just different user access
* prevention
	* path 
	* update anti-virus/anti-malware
	* data execution prevention
		* only data in executable areas can run
		* stops the vuln from running in a part of memory
	* address space layout randomization
		* apps run in a random part of memory to prevent attackers from exploiting an application at a known location of memroy 