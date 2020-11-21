Command Line Security Tools

* ping
	* deterime if a host is up
	* determine round trip
	* uses ICMP (internet control message protocol)
	* first troubleshoot tool
	* written in 1983
	* sound used by sonar 
* netstat
	* give network statistics 
	* netstat -a 
		* shows all active connections 
	* netstat -b
		* shows binaries that make the connection (windows)
	* netstat -n 
		* do not resolve names 
* traceroute
	* tracert (windows)
	* determine the route a packet takes to a destination 
	* maps the path 
	* takes advantage of ICMP time to live (TTL, TTL of 1 + number of devices hit, in this case) excedded error message so it fails at every device 
	* not all devices will reply with ICMP time excedded messages 
	* not always the same path
* nslookup and dig
	* lookup information from dns servers 
	* nslookup is deprecated, use dig
	* dig - Domain Information Groper
		* more advanced
* address resolution protocol
	* determine the MAC address based on an IP address
	* arp -a
		* view local arp table 
* ifconfig and ipconfig
	* most of your troubleshooting starts with IP addresses 
	* determine the TCP/IP and network adapter information
	* use ip -a on linux 
* tcpdump
	* capture packets from the command line 
	* available in linux/mac, download WinDump for windows
	* apply filters, view in real time 
	* save the data, use in another application 
	* can be an overwhelming amount of data 
* nmap
	* netowrk mapper
	* port scans to find services on a device 
	* os scan 
	* service scan
		* name, version, detials
	* aditional scripts 
* netcat
	* read or write to the network 
	* open a port and send or recieve some information 
	* different functions
		* kisten on a port
		* transfer data
		* scan ports and send data
	* become a backdoor 
	* alturnative - ncat 