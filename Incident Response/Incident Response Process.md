Incident Response Process 

* NIST SP 800-61
	* National institute of standards of technology
		* computer security incident handling guide
	* the incident reponse lifecycle 
		* prep
		* detection and anaylsis
		* containment, eradication, and recovery 
	* post-incident activity 
* prep for an incident 
	* comm methods 
		* phones and contact info
	* incident handling hardware and softwware 
		* laptops, removable media, forensic software, digital cam, etc
	* incident analysis resources 
		* doc, network diagrams, baselines, critical file hash values 
	* incident mitigation software 
		* clear OS and app images
	* policies needed for incident handling 
* the challenge of detection 
	* many different detection sources 
		* different levels of detials 
	* a large amount of "volume"
	* incidents are almost always complex
		* need advanced knowledge 
* incident percusors 
	* an incidnet might occur in the future 
	* web server log 
		* vuln scanner in use 
	* exploit announcements 
		* monthly Microsoft patch release, Adobe flash update 
	* direct threats 
		* a hacking group doesn't like you 
* incident indicators 
	* an attack is underway 
	* buffer overflow attempts 
	* anti-virus software id malware 
	* host-based monitor detects a config change 
		* monitors system files 
	* network traffic is different from norm 
* isolation and containment 
	* generally a bad idea to let things run their course 
		* incident can spread 
	* sandboxes 
		* the attacker things they're on a real system 
	*  isolation can be problematic 
		* malware can monitor connectivity 
		* when connectivity is lost, everything could be deleted, encrypted, damaged 
* recovery after an indident 
	* get things back to normal
	* eradicate the bug 
		* remove malware 
		* diable breached user acounts
		* fix vulns 
	* recover the system 
		* restore from backups 
		* rebuild from scratch 
		* replace files 
		* tighten down the perimeter 
* reconstitution 
	* a phased approach 
	* recovery may take months 
		* large-scale incidents require a lot of work
	* the plan should be efficient 
		* start with a quick, high-value security changes 
			* patches, firewall
		* later phases involve must "heavier lifting"
* lessons learned 
	* learn and improve 
		* no system is perfect
	* post-incident meeting 
	* don't wait too long 
		* memories fade
	* answer the tough questions 
		* what happened, timestamps 
		* how did the incident plan work?
		* what would you do differently next time 
		* which indicators would you watch next time 
			* different precursors may give you better alerts 