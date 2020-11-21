Business Impact Anaylsis

* recovery 
	* mean time to restore (MTTR)
		* average time to restore a system after it fails 
	* mean time to failure (MTTF)
		* the expected lifetime of a non-repairable product or system
	* mean time betweeen failures (MTBF)
		* predict the time between failures 
	* recovery time objectives (RTO)
		* get up and running quickly 
		* get back to a particular service level
	* recovery point objective (RPO)
		* how much data is loss is acceptable  
		* bring the system back online, how far back does data go?
		* provide limited availability to a certian group of poeple 
* calculating uptime and availability 
	* expressed as a percent over time 
		* 99.999% availability 
		* 5 9's
	* availbility is a negoatied def 
		* is downtime for maitenence part of the metric
			* is it planned
		* could be part of a bonus 
	* ![f3b51ec7933abbd647dcfc60cf4ce59a.png](../../_resources/acd8e61259694818b9d83188d084f72a.png)
* mission-essential functions 
	* if a hurricane blew through, what functions would be ssential to the org
			* thats where you start you analysis
			* these are the broad business requirements 
		* what computing sytstems are required for these mission-essential business functions
			* id the critical systems 
* removing single point of failure 
	* a single event can ruin your day
	* remove a single point of failure, redudency 
	* netowork config 
		* multiple devices (the "Noah's Ark" of networking)
	* facility/utilities 
		* backup power, multiple cooling devices 
	* people/locations
		* a good hurricae can disrupt personel travel 
	* no practical way to remove all points of failure 
		* money drives redudaancy 
	* ![b878323e9b0e3691516975b822ff8d40.png](../../_resources/fda9b59ecd804257be918dc098539851.png)
* imopact 
	* life 
		* everyone working at the org is safe 
	* property 
		* the risk to buildings and assets 
	* safety 
		* some enviroments are too dangerous to work 
	* finance 
		* the resulting fininchal cost 
	* reputation 
		* an event can  cause status or character problems 
* privacy compliance 
	* some compliance requires a public privacy statement 
	* privacy threshold (PTA)
		* the first step in the compliance process 
		* id business processes that are privacy senstive 
		* determine if a privacy impact assessment is required 
	* privacy impact assessment (PIA)
		* ensures compliance with privacy laws and regulationis 
		* what PII is collected and why
		* how the PII data will be collected, used, sold