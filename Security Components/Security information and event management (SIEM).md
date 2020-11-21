Security information and event management (SIEM)

* **Loggin of security events and information**
* security alerts 
	* real time information 
* log aggregation and long term storage 
* data correlation
	* links diverse types of data
* forensiv analysis 
* time scnchronization 
	* swithces, router, firewall, servers, workstation has its own clock
	* becomes critical to know what is happening at different devices at the same time
	* NTP (Network Time Protocol)
		* very accurate 
		* flexable, you control how the clock are synced 
* syslog
	* standard for message loggin 
	* usually a central loggin receiver 
		* integrated into the SIEM
	* you're going to need a lot of disk space 
	* WORM drive technology 
		* Write Once Read Many - DVD-R
		* protects logs
* Event de-duplication
	* events sotrms 
	* filter out the noise 
	* flapping (down/up/down)
		* timers used to supress ongoing messages 
* automated alerting and triggers 
	* constant flow of information 
	* track inportant stats 
		* exceptions can be id
	* send alerts when problems are found 
	* create triggers to automate responses 
		* open a ticket, reboot a server 
* security reports 
	* reports generated at set intervals to show everyting in a graphical view 