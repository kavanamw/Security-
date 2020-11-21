Firewalls

* the universal security control
* **controls the flow of traffic to prevent the bad traffic from getting in or sometimes out**
	* control of senstive material
* control of inapproprate content 
* filters by port number 
	* OSI layer 4
	* some firewalls can filter through osi layer 7
	* can ecrypt traffic into/out of the network 
	* can proxy trafic
	* most can be router
* stateless firewall
	* does not keep track of traffic flows
	* each packet is indivudailly examined, regardless of history
	* traffic sent outside of an active session will traverse a stateless firewall
* stateful firewall
	* remeber the state of the sesion
	* when a packet hits the firewall the session is given a number, a source IP, a destination IP
	* is traffic comes in that is destinied to a known reciever but it is not part of the session table the traffic will be dropped 
* Application  aware security devices
	* OSI appliciation layer 
	* names
		* application layer gateway
		* stateful multilayer inspection
		* deep packet inspection
	* every packet must be analyzed and categorized before a security decision  
	* network based firewall
		* control traffic flows based on the application
		* intrusion prevention system
			* id the application
			* apply app specific vuln signatrues 
			* host based firewall
				* works with the os the determine the app
* firewall rules
	* Access control lists (ACLs)
	* rules for the traffic being allowed or not 
	* a logical path, usually top to bottom
	* can be very general or very specific 
		* specific rules are usually on top
	* implicit deny
		* most firewalls include a deny at the bottom
		* if it matches no rules then most will default to deny the traffic
	* 