Provisioning and Deprovisioning 

* provisioning - make something aviable 
	* deploy app
		* web server, database server, middleware server, user workstation configs, cert updates, etc
	* app sotware security
		* os, app
	* network security 
		* secure VLAN, internal access, external access,
	* software deployed to workstations 
		* check exe for malicious code, verify security posture of the workstation 
* orchestration - push button, deploy cloud via automation
	* automate is the key to cloud computing 
	* entire app instances can be instantly provisioned 
	* instances can move around the world as needed
		* follow the sun
		* wake up servers local to the daytime 
	* security policy should be part of the orchestration 
		* proper security is automatically included
* deprovisioning 
	* dismantling and removeing an app instance 
	* securit deprovising is import 
		* don't leave open holes, don't close important ones 
	* firewall policied must be reverted 
		* app gone, so is access
	* what happens to the data?
		* don't leave data public