Denial of Service

* **force a service to fail via an overload of the serice**
* take advantage of a design failure or vuln
	* keep systems patched
* sometimes an overload
* create a smokescreen for some other exploit
	* percusror to a DNS spoofing attack
* could be as simple as a power outage 
* a friendly dos
	* unintentional DoSing 
	* netowkr DoS
		* layer 2 loop without STP
	* bandwidth Dos
		* downloading large files over a DSL line
	* water line break
		* knocks out servers
* ddos
	* an attack from many places at the same time 
	* use all the bandwidth or resources 
	* why the bad guys have botnets 
	* asymmetric threat
		* the attacks has fewer resources than the victum 
* ddos amplicaion
	* turns a small attack into a big one via a service 
		* often reflected off another device 
		* uses protocols with little auth 
			* NTP, DNS, ICMP
	* ask for little on the inbound that amps to a large on the outbound
	* a bunch of requests into resolvers before sending that onto a server, small in, large out and massive in for the end server