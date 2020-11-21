Embedded Systems

* SCADA (Supervisory Control and Data Aquisition Systems)
	* large scale, multi-site insustral control system (ICS)
	* PC manages equipment 
		* power generation, regining, manufacturing 
	* distrucbuted control systems 
		* real time info
		* system control
	* requires extensive segmentation
		* no access from the outside 
		* like in a power plant
* Smart device and IOT
	* weakable technology 
		* track location 
		* where is that info stored and who has access
	* home automation
		* video doorbells
		* door openers
		* HVAC
		* knows when you're home and when you're not
* HVAC (Heating Ventilation and Air conditioning)
	* a complex science 
		* no something to desin yourself
		* must be integrated into the fire system
	* PC manages equipment 
		* makes decisions 
	* traditionally not built with security in mind 
		* difficult to recover from a DDoS
* SoC (System on a chip)
	* multipole components running on a single chip
	* small form factor
		* external interfact support
		* cache mem, flash mem
		* usually low powered
	* secuirty considerations are important 
		* dificult to upgrade hardware 
* RTOS (Real Time Operating System)
	* an os with a deterministic processing schudel
		* no time wait for other processes 
		* industral quipment, cars
		* military equipment 
		* brakes on a car, you don't want to wait on other processes to finish first 
	* extremely senstive to security issues 
		* non-triucial systems 
		* needs to be available all the time
		* difficult to know what type of security is in place
* Printers, Scanners, and fax machines
	* All in one multifunction device (MFD)
		* everything in one device
	* no longer a simple printer, sophisticated firmware 
	* some images are stored locally on the device
		* can be retreived externally
	* logs are stored on the device 
* camera systems 
	* vidos records are IP devices 
		* auth using a specialized app
	* camera are IP devices
	* privacy concerns 
		* know when you are home
		* know what security you have
* special purposes
	* medical devices
		* heart monitors, insulin pumps
		* often older oses
	* vehicles 
		* internal networks is often accessible from mobile network 
		* control internal electronics 
		* disable the engine 
	* aircraft/UAV
		* DoS could damage the aircraft or people on the ground 