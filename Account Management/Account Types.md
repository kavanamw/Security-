Account Types

* User accounts 
	* an account on the computer that is associated with an individual 
	* storage and files can be private to that user 
		* even if another is using that computer 
	* no privileged access to the os 
		* specifically not allowed on a user account 
	* the type most people use
* shared account 
	* used by more than one person 
	* guest login 
	* very difficult to create an audit trail 
		* no way to know exactly who was working 
		* difficult to determine the proper priviegde 
	* pasword management becomes difficult 
		* password change requires telling everyone 
			* difficult to rememebr so many password changes 
			* write it down on a sticky note
			* insecure storage of passwords due to the changes 
* service accounts 
	* used exculusively by services running on a computer
		* no interactive/user access
		* web server, database server
	* access can be defined for a specific service 
		* web server rights and persmission 
	* scomonly use username and passwords
		* policy for changes
* privileged accounts 
	* evalated access to one or more systems 
		* admin, root
	* complete access to the system 
		* often sued to manage hardware, drivers, and software installs 
	* this account should not be used for normal admin 
		* user accounts show be used
	* needs to be highly secured 
		* strong passwords, 2FA
		* scheduled password changes 