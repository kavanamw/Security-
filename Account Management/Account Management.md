Account Management 

* least priviledge 
	* rights and permissions should be set to the bare min
	* you get exactly what needed
	* all user accounts must be limited
	* don't allow users to run with admin privileges 
		* limmits the scope of malicious behavior 
* on boarding 
	* bring a new person into the org
	* it agremments need to be signed 
		* may be in the employee handbook
	* create accounts 
		* associate the user with the proper groups and priv
	* provide hardware
* off boarding 
	* the process should be pre planned
	* what happens to the hardware?
	* what happens to the data?
	* account info is usually deactited 
		* but not always deleted
* preform reoutine audits 
	* is everyone following policy?
	* make sure it's scheduled 
	* certain actions can be automatically id
		* consider a tool for log analisis
* auditing 
	* permission auditing 
		* does everyone have the correct premissions?
		* some admins don't need to be admin
		* scheduled recert 
	* usage auditing 
		* how are resources being used?
		* are you systems and apps secure?
		* time of day restrictions 
			* nobody needs lab access at 3AM
* standard naming convertions 
	* unique 
		* same username across multiple systems 
	* consistent 
		* usernames shouldn't describe a role or status 
	* persistent 
		* use the same username for the duration of employment 
	* memorable 
		* shouldn't be difficult 
		* doesn't mean recognizable 
* account maintence 
	* account creation 
		* intial provisioning 
		* password management 
		* group and persmission assignments 
	* peridiocit updates 
		* password resets/forced updates 
		* permission audits
	* deprovisioning 
		* disable account 
		* archive users docs and encryption keys 
* group based access control
	* set privileges based on what you do 
		* put many users in a single group
		* set privileges on the group
		* add/remove users from the group to assign privileges
	* users can be members of multiple groups 
		* group permissions can overlap
		* how do you determine the effective premissions?
			* not as straightforward as you think
			* don't run into problems with implicit premission 
				* one group denies, another allows
* location based policies 
	* user access is based on location 
		* GPS, mobile devices, very accurate
		* 802.11 wireless, less accurate
		* IP address, not very accurate 
	* restrict app use 
		* don't allow this app to run unless you're near the office 
	* apply securty rules 
		* your IP address is associated with an IP block in China
		* we don't have an office in China
		* permission not granted