Acess Points (WAP)

* not a wireless router
	* a router has a WAP and a router in one device 
* WAP is a bridge 
	* extends the wired network onto the wireless network 
	* WAP is layer 2
* SSID management 
	* Service Set Identifier 
	* a name of a wireless network 
	* change the ssid to something not too obvious 
	* name should match the type of network you're connection to 
* MAC filtering 
	* limit access through the physical hardware address 
	* keeps neighbors out 
	* limits who can get on your network
	* MAC addresses can be spoofed by watching the network traffic 
	* security through obscurity 
* Power level controls 
	* best to set as low as you can 
	* covers less area 
	* test to know how low is low enough 
	* consider the receiver 
		* high gain can hear a lot 
* Band selection bandwidths 
	* throughput 
		* max theoretical throughputs 
		* actually can varry widely 
	* frequence 
		* 2.4 and 5 GHz 
	* channels 
		* difference in geographical location 
		* non-overlapping channes are best 
* band selection and bandwidth 
	* ![e6bd9ee0719431e15da039a3b6f98c52.png](../../_resources/0ca6676b9d0f4000926e840f118bba77.png)
* omnidirection antennas 
	* most common 
	* siginal is evenly distrubuted on all sides 
	* good choice for most enviroments 
	* no way to focus the signal 
* antenna placement 
	* ![5dbc4f27b4f1ee91efab78269aa76237.png](../../_resources/a86a0d097b8d4682a3c81c42e98649df.png)
* directional placement 
	* focus the signal, increase distance 
	* preformacne is measured in dB 
		* double power every 3dB of gain 
* wireless LAN controllers 
	* centralized management of WAPs 
		* a single pain of glass 
	* deploy new access points 
	* preformance and security monitoring 
	* configure and deploy changes to all sites 
	* report on access point use 
	* normally proiperty 
		* controlelr paried with the access point 
* LWAPP
	* lightwight access point protocol 
	* CAPWAP is an RFC standard based on LWAPP
	* manage multiple access points at the same time
	* thick/fat access points 
		* handles most wireless tasks 
		* switch is not wireless-aware 
	* thin access points 
		* just enough to be 802.11 wireless 
		* the intelligence is in the switch 
		* less expensive 