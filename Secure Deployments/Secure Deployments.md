Secure Deployments 

* Development to production 
	* how will you deploy safely and reliability
	* how will you patch 
	* manage the process 
* sandboxing 
	* isolated testing enciroment 
	* no connectnion to the real world 
	* use during dev process
	* incremential development 
		* try code, break things 
* working enviroments 
	* secure enviroment 
	* writing code
	* test 
		* still in the dev stage
		* does it all work after putting it together 
		* QA testing 
		* if its working then its read for prod
	* staging 
		* almsot ready to deploy
		* works and feels like the prod env
		* working with a copy of prod data
		* preformance tests 
		* test usability and features 
	* production 
		* app is live 
		* rolled out to the user community 
* secure baseline 
	* the security of an application env should be well defined
	* firewall settings, patch levels, os file versions 
	* amy require constant updates 
	* integrity measurments checks for the baseline over time 