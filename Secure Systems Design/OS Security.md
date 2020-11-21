OS Security

* types
	* network
		* connects devices over the network
	* server
		* web server, database server
	* workstation
		* optimized for user apps 
			* email, browsing, office
	* appliance 
		* purpose built
		* usually a minimal os unsean by the user 
	* kiosk
		* public device 
		* os is tightly locked down 
	* mobile
		* designed for touch screen 
		* optimized for mobile hardware (arm and apple)
* patch management 
	* very important 
	* service packs
		* a single large set of updates 
		* often from microsoft 
	* vs monthly incremental updates 
	* emergency out of band 
		* zero day exploits 
* update options
	* windows - Windows Updates 
	* Windows server updates Services (WSUS)
		* a centralized management for windows devices 
	* Mac os - software updates, app store 
	* linux 
		* many different options 
		* yum, apt-get, rpm, graphical front end 
* the patching process
	* not always seamless 
	* may introduce some planning 
	* pick and choose which patches
		* do get the security ones 
	* often centrally managed 
		* test then have the MDM distribute the patches
* disabling unnecessary services 
	* every service is a problem point
	* may require a lot of research to find what is needed and what can be disabled
	* trial and error may be necessary 
* least functionality 
	* limit the os to only what's needed
	* may be different depending on the use 
		* shipping and receiving will have different needs from IT/dev
	* extensive configs 
		* disable printer install
		* disable changing time
* sercure configs 
	* fine tuning of the os 
	* many of these will apply regardless of how the system is used
	* ex.
		* stay up to date with all patches 
		* compromised systems are reimaged, not cleaned
		* changes must be managed
		* preform integrity checks of the os files 
* eval assurance levels
	* common criteria for information technology evaluation 
		* also called common criteria (or CC)
		* international standard for computer security 
		* common reference for US Federal Goverment 
	* evaluation assurance level (EAL)
		* EAL1 - EAL7
	* trusted OS
		* the os is EAL compliant 
		* EAL$ is the most accepted minimul level
* app whitelisting and blacklisting 
	* any app can be dangerous 
	* security policy can allow or disallow app execution 
	* whitelisting 
		* nothing runs unless approved
	* blacklisting 
		* everything runs but some stuff 
* app whitelisting
	* application hash
	* certificate 
		* digitally signed apps from certian publishers 
	* paths 
		* only apps running from a protected path can execute 
	* network zone 
		* only apps can run on the corperate network, not public ones 
* disabling unncessary accounts 
	* all os include other accounts 
		* guest, root, mail, etc
	* disable interactive log ins
		* not all accounts need to login 