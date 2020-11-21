NIDS and NIPS

* Network Intrustion Detection System
* Network Intrustion Prevention System
	* both watch internet traffic 
	* one tells you, one prevents as it happens 
* intrusions 
	* exploits 
* passive monitoring 
	* examine a copy of the traffic 
		* copy sent, not in the middle 
	* no way to prevent traffic (NIDS)
	* out of band response 
		* when bad traffic is id, IPS sends TCP reset frame to the dest and source effectivly cutting the traffic flow 
		* stops the communication before much data is lost 
		* does not work well with things other than TCP (such as UDP)
	* Inline monoriting 
		* all traffic passes through the IPS
			* is a man in the middle
		* drop packet at the IPS if it's bad 
		* signature based
			* looks for a perfect match to bad traffic 
		* anomaly based
			* builds a baseline for normal then blocks weird stuff
		* behavior based 
			* observe and report based on the user actions 
		* Heuristics 
			* things that look like an attack 
	* IPS rules
		* you determine what happens when unwanted traffic appears 
			* block, allow, send an alert 
		* customized by group
		* can take a lot of time to find the balance
	* false postives 
		* a report that is not true
		* IDS/IPS info
			* only as good as the signatures 
			* some legitimate traffic could be marked as bad 
	* false negative
		* a report missed id something bad 
		* bad traffic gets through your defenses 
		* get catch/miss rates with testing 