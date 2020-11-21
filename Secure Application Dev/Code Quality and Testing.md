Code Quality and Testing  

* Static application security testing (SAST)
	* helps find security vulns
	* not everything can be found through anaylsis
		* don't relay on automation 
	* still have to verify every finding 
* dynamic anaylsis (fuzzing)
	* send random input to an application 
		* fault-injecting, robostness testing, syntax testing, negative testing
	* looking for something out of the ordinary
		* crashse, server exceptions 
* fuzzing engines and frameworks 
	* platform specific, language specific, etc
	* very time and processor heavy
		* many fuzzing engines use high-probility tests
* CERT basic fuzzing framework
* Stres testing 
	* the software works with one user 
		* what about 1,000?
	* inadvertent results can occur at load
		* unintended error messages
		* app detials and version leaked
		* kernel and mem dump
	* auotmate indivudial workstations 
	* simulate large workstation loads
	* extensive reporting at the end 
* sandboxing 
	* test enviroment look and works exactly like prod
		* no prod systems are used
		* no prod data is used
	* QA can fuzz, overload and break but not hurt prod users
* model verification 
	* verification and validation (V&V)
	* verification 
		* does the software work right
		* bugs to address
		* building the product right
	* validation 
		* did you meet the requirments
		* did we build the right product 
* compiled vs. runtime code
	* compiled code
		* don't see the source code
		* app is exe compiled from the source
		* the compiled code is specific to an os and CPU
		* logical bugs can be id at compiled time 
		* C. C++, Java
	* runtime 
		* source code is viewable
		* the code instructions execute when the app is run
		* python 