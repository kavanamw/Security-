Account Policy Enforcement 

* cred mangaement 
	* all that stands between the outside world and your data
	* passwords must not be embedded in the app
		* everything needs to reside on the server 
	* comm across the network should be encrypted
* configuring settings 
	* windows group policy management 
		* apply security admin settings across many computers 
		* thousands of settings 
	* different from NTFS or share permissions 
	* linked to AD admin bountires 
* group policy control
	* admin policies 
		* remove add or remove programs 
		* prohibit changing sounds 
		* allow font downloads
		* only allow approved domains to use ActiveX control without prompt
	* security policies 
		* specify minimul password length
		* require smart card
		* maximum security log size 
		* enforce user login restrictions
* password complexity and length
	* make your password strong 
		* no single words
		* no obvious passwords 
		* mix upper and lower case 
		* use special character 
	* a strong password is at least 8 characters 
	* prevent password reuse 
* password expiration and recovery
	* all passwords should expire 
	* critical systesm might change more frequently 
	* the recovery process should not be trivial 
* account lockout and disablement 
	* too many bad passwords will cause a lockout 
		* normal for most users 
		* can cause issues for service accounts 
	* diable accounts 
		* part of the normal change process
		* you don't want to delete accounts, at least not initially 