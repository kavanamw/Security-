Network Access control

* access control 
	* control from whereever you are 
		* inside or outside
	* access based on user, group, location, etc
	* access can be easily revoked or changed 
* Posture assessment (BYOD)
	* is the device safe?
	* running anti-virus
	* corporate apps installed
	* disk encrypted
	* must run on all OSes 
	* persistent agent
		* permanently installed onto a system
		* periodic updates may be required
	* dissolvable agents 
		* no installation is required
		* runs during the posture assessment 
		* terminates when no longer required
	* Agentless NAC
		* integrated withing AD
		* checks are made during login and logoff 
		* can't be scheduled
	* failing as assessment 
		* too dangerous to be allowed on the network
		* normally put on a quarentine network
			* enough access to install software and updates  
		* once resolved, try again 