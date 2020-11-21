Security Technologies Placment 

* sensors and collectors 
	* gather information from network devices 
		* built in or seperate
		* integrated into switches, routers, servers, firewalls, etc
	* sensors 
		* IPS, firewall logs, auth logs, web server logs, database transation lgos, email logs
	* collectors 
		* propreitarty consoles (IPS< firewall), SIEM consoles, syslog servers 
		* many SIEMs include a correlation engine to compare diverse sensor data
* filters and firewalls
	* packet filters 
		* simple data blocks - ignore state
		* linux iptables - filter packets in the kernel
		* usually placed on a device or server 
	* firewalls
		* state based
		* advancced filtering based on IP address, port, application, content 
		* usually located on the ingress/egress of the network
		* some organizations place them between internal networks 
* proxy servers
	* an intermediate server 
		* client makes the request to the proxy
		* the proxy preforms the request 
		* proxy provides result after looking at it to make sure it is safe 
	* features 
		* access control, URL filtering, etc. 
* forward proxy
	* protects users from the internet 
	* user -> proxy -> internet 
* VPN concentrators 
	* VPN appliancs are ususally located on the edge of the network 
* SSL accelerators 
	* does the SSL handshake and offloads it from the webserver 
	* often integrated into a load balancer 
* load balancers 
	* manage the load across multiple devices 
	* placed between the users and the device 
	* servers can be added or removed 
	* makes health checks 
* DDoS mitigation
	* resist a DDoS
	* cloud based
		* internet provider or reverse proxy to filter bad traffic 
	* on site 
		* DDoS filtering in a firewall or IPS
	* between you and the internet 
* aggregation switches 
	* ![2947203ceaff4379e9f55a72921e9565.png](../../_resources/744660e818f24fd9ae8935a471a5e509.png)
	* core 
		* the main core of the internet 
	* distrubution and aggregation
		* larger switches to connect between the core and the users 
	* access
		* the end users 
* taps and port mirrors 
	* intercept network traffic 
	* physical taps 
		* disconnect a link, put the tap in the middle 
		* can be active or passive 
	* port mirror 
		* port redirection, SPAN (Switches Port aNalyzer)
		* software based tap
		* limited functionality, but can work well in a pintch
	* ![8254ac5205677d9682262de0cd02304e.png](../../_resources/3f200c216ee54b46a94eb78d340f3bef.png) 