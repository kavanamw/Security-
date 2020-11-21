Network Segmentation 

* Segmenting the network
	* physical, logical, or virtual segmentation
	* preformance 
		* high bandwidth apps on their own network for more efficency 
	* security 
		* apps that can only talk to the database 
		* users are segmentated away from the core of a network 
	* compliance 
		* mandated segmentation (PCI compliance)
		* makes control easier, alter some network not all
* physical segmentation
	* devices are seperate 
	* must be connected to provide comm
	* web servers in one rack, database on another 
	* customer A on one and customer B on anther 
* logical segmentation with VLANS
	* sepearated logically instead of physically 
	* cannot comm between VLANS without a layer 3 device/router 
	* ![181511b58f33d01a0f50d73e28e94058.png](../../_resources/6a1f20b4da9b478b9f9e639e2a162a7d.png)
* Virtualization 
	* servers, switches, routers, firewalls, load balancers are all virtual
	* instant and complete control
		* build a new network quickly 
		* route between IP subnets 
		* drop a firewall between 
		* drag and drop between networks
* air gaps
	* one step up from physical 
	* remove any connectivity between components 
	* network separation
		* secure networks
		* industral systems (SCADA, manufacturing)
		* jump the gap
			* removable media 