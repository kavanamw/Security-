Seucre DevOps

* DevOps - development and Operations 
	* ![cc1e202fbf6c4036bec2372455c2e71b.png](../../_resources/76f5676abb1e408b838f299effe6a984.png)
	* creating and deploying apps
		* speed, availablity, and security 
	* emphsis on automation and monitoring 
		* integration, testing, release, and manage
	* shrink deployment cyles 
		* and more deployments
* security automation
	* automation is relativly inexpensive 
	* functional security tests
		* login, logout, ensure a secure platform
	* test against known vulns 
		* misconfigs, weak SSL, ciphers
	* pen testing 
	* test the security of the app itself 
		* manipulate the app to get unexpected results 
* continuous integration
	* code is contantly written 
	* many chances for security problems 
	* basic set of security checks during the development process
	* large-scale security anaylsis
* immutable systems
	* update an app every week for a year
	* immutable systems - locked down and unable to change 
		* to update the app, the entire platform must be updated
		* test the entire system, not a small part of it 
	* much stronger security becasue no small update could introduce bugs
* infrasturture as code (IAC)
	* cloud computing 
	* automate the building and deployment of hardware and software in the cloud 
		* done fast
	* turn the infrasturcre devices into code
		* virt everything 
		* focus on what the app needs rather than building the app based on available infrastrue 
	* security is a known quantity 