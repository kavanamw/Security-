Securing the Network Topologies 

* Demilitarized zone (DMZ)
	* an additional layer of security between the internet and you
	* public access to the public resources 
	* ![99380a5720e0d2b78a58276707830510.png](../../_resources/c47f86d8cf374a1fa5c2e7bba073af5a.png)
* extranet
	* a private DMZ
	* usually requires aditional auth 
	* ![4af402bd2dec4efb813f76fdb1809c07.png](../../_resources/5e5d98636baa4917905d70b152a62a7c.png)
* intranet
	* private netowrk 
		* only available internally
	* company announcements, important internal documents 
	* no external access
		* interal or VPN access only
	* ![0d9b85296a0cb049116c7c0e17a8ad55.png](../../_resources/8a31207cf37d4491abd39caf364fd3d2.png)
* Wireless networking
	* the convience of wireless vs the security of it
	* interal use with seperate guest access
	* auth for the internal login
		* using the normal network login 802.1x standard 
		* integrates into the existing name services
		* no shared wireless passphrase
			* individual login
* guest network
	* an optional network
	* no access to the internal network but access to the internet
	* integrate with a captive portal 
		* auth guest creds
* Ad hoc
	* wireless without the access point 
	* common on mobile devices
	* difficult to control on unmanaged devices 
		* configured through the MDM
	* implemend network control 
		* use ad hoc but only with the right cred
		* limit app use for ad hoc
* honeypots and honeynets
	* attrack the bad guys
	* often bad guys are a machine 
	* honeypot - single use/single system traps
	* honeynets - more than one honeypot on a network, more than one source of information 
* NAT - Network Address Translation
	* IPv4 only has 4.29 addresses
	* NAT allows more 
	* not the only thing that NAT can do
* NAT and security 
	* NAT is not security 
	* only is security through obscurity 
	* the bad guys can circumvent an unprotected NAT 
	* a stateful firewall and NAT can be good
	* 