Access Control Models 

* Access control
	* authorization 
		* policy encofrment 
			* the process of ensuring only authorized rights are exercised
		* policy definition 
			* the process of determining rights 
	* users recieve rights based on access control models 
		* different businesss needs or mission requirments 
* mandatory access control (MAC)
	* the os limits the operation on an object 
		* based on security clearence levels 
	* every object gets a label
		* confidential, secret, top secret, etc
	* labeling of objects uses predefined rules 
		* the admin deides who gets access to what security level 
		* users cannot change these settings 
* discretionary access control (DAC)
	* used in most os 
	* you create a spreadsheet
		* as the owner, you control who has access
		* modify access at any time 
	* very flexable access control 
		* weak security 
			* relies on the owner to set the proper sefcurity based on object
* role baseed access control (RBAC)
	* you have a role in you org
	* admins provide access based on the role of the user 
		* rights are gained implicitrly instead of explicityly
	* in Windows, use groups 
		* you are in shipping 
			* you can use shipping software
* attribute-based access control (ABAC)
	* users can have complex relationships to app and data 
		* access may be based on many different criteria 
	* ABAC can consider many parameters 
		* a "next generation" auth model 
		* aware of context 
	* combine and eval multiple parms 
		* resource info, IP, time of day, desired action, relationship to the data, etc
* rule based access control 
	* generic term for following rules 
		* conditions other than who you are 
	* access is deremined through system enfoced rules 
		* system admins not users
	* rule is associated with the object 
		* system checks the ACLs for that object
	* rule ex
		* lab network access only available between 9AM and 5PM
		* only chrome browsers may complete this web form 
* file system security 
	* accessing info
		* access control list 
		* groups/users rights and permissions 
		* can be centerally administratored and/or users can manage files they own
	* encryption can be built in 
		* the file system handles encryption and decryption
* database security 
	* databases have their own access control
		* username, password, permission 
	* encryption may be an option 
	* data integrity 
		* no data is lost because of a fault 
	* apps can provide a secure front end 
		* no SQL attacks 