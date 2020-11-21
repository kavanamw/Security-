Resillency and Automation 

* automation and scripting 
	* plan for change 
	* automated courses of action 
		* many problems can be predected 
		* have a set of auto responses
	* continous monitoring 
		* check for event then react
	* configuration validation
		* cloud based tech allow for constant change
		* automatically validate a config before going lvie 
		* preform ongoing checks
* templates
	* basic structure of an app instance 
	* the blueprint of online services
	* requires a web server, database server
		* what version, PHP version, SSL certs, firwall, brute force monitoring 
	* template is just a start 
		* scritps and APIs to do the changes 
* master image
	* instead of builgin the server each time create a custom image 
	* still need to make changes when deploying 
	* keep the master image updated 
		* securty patches 
		* os updates
		* service updates 
		* can be challenging and take a lot of time 
* non-persistence 
	* the cloud is always in motion 
	* snapshots can capture the current config and data 
		* state of device or just config 
	* revert to a known state 
	* rollback config but don't modify data
	* live boot media 
		* very portable 
* elasticity and scalability
	* elasticity  
		* provide resources when demand 
		* scale down when slow
	* host availbility 
		* new server deployed in a few clicks
	* virt integrates a layer of orchestration 
		* automate the deployment and movement of virt hosts 
	* servers can be added or moved to other data centers 
		* all of the mangement systems follow the servers 