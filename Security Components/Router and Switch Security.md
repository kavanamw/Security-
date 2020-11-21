Router and Switch Security 

# Routers 
* Routers traffic between IP subnets 
	* OSI Layer 3 devices 
	* routers inside switches sometimes called layer 3 switches 
* layer 2 = Switch
* layer 3 = router 
* often connect diverse network types
	* LAN, WAN, copper, fiber, etc.
* Acess Control List (ACLs)
	* used to allow or deny traffic 
		* also used for NAT, Qos, etc
	* defined on the ingress or egress of an interface 
	* ACLs evauilate certain criteris 
		* source ip, dest ip, tcp port number, udp port number, icmp
	* Like a firewall but for the internal network 
* ![1b5cba75ce665cd64bc60e080e24db1c.png](../../_resources/0c8e942a30b7493e931b0f71d472f488.png)
* anti spoofing 
	* prevents a bad guy from spoofing 
	* filter reserved IP addresses to protect them from the internet 
	* enable reverse path forwarding (RPF)
		* the response to an inbound packet should return the same way
		* if it doesn't then drop the packet right now
# Switches 
	* bridging done in hardware 
		* application specific inegrated circuit (ASIC)
	* OSI layer 2 device 
		* forwards traffic based on data link addresses
	* many many ports 
	* high bandwidth 
* switch port security 
	* the inside of the network is far less secure than the connection to the outside 
	* often easy to connect to the network 
		* open ports in conference rooms
* Network access control (NAC)
	* IEEE 802.1x Port based access control 
		* no access to the network without first authenticating 
		* makes use of EAP (Extensible Authentication Protocol) and RADIUS (Remote Authentication Dail In User Service)
		* ports here means physical connection ports not numbered ones 
	* must be enabled or disabled by an admin 
	* check for duplicate MAC addresses 
* Loop prevention
	* connect two switches to each other 
		* theyll send traffic back and forth forever 
		* no counting at the MAC layer
	* kinda dos yourself
	* spanning tree protocol 
		* IEEE 802.1D to prevent loops in bridged (switched networks)
		* ![37337a5e69d337d7147d783cf8f01142.png](../../_resources/38ce5c6c1a794a19adbf45e862c937d3.png)
		* BP nodes prevent the loops from happening 
		* smart enough to watch the network and make changes if they are needed 
			* could happen if a network becomes unavailable 
* Flood guard
	* configure a max number of source MAC addresses on an interface 
	* adds some dos prevention per interface 
	* the switch monitors the number of unique MAC addresses 
	* once the max is hit port security kicks in 
* Layer 3 switches 
	* a switch (layer 2) and a router (layer 3) in one device