Common Security Issues 

* Unencrypted creds
	* auth is a critical process
	* some protocols aren't encrypted 
		* telnet, ftp, smtp, imap
	* verify with a packet capture software to know if it is encrypted 
* lops and event anomalies 
	* gather as much information as possible 
	* switches, routers, firewalls, servers
	* SIEM (Security information and event management) will hold all that information 
* permission issues
	* a simple oversite, but a big vuln
	* database left on the open internet with little to no auth to get in
	* confirm permissions on initial config
* asscess violations
	* seg fault
	* os should prevent this from happening 
	* could just be a programming problem 
	* could be a security issue 
		* restricted memory area
* certificate issues
	* trust 
		* a cert should be signed by someone you trust 
		* either internal or external CA
	* certs should be renewed every couple months or years 
* Data exfiltration
	* data is your most valuable asset 
	* you've aready built a high speed network 
* misconfigured devices
	* another example of leaving the door open
	* default username and passwords 
	* outdated software 
	* running maitenance code in the public
		* leaks more info than you should
* misconfigured devices
	* firewalls 
		* rules provide too muich access
	* content filters
		* URLs are not specific enough
		* some protocols are not filtered
	* access points
		* no encryption mechanisms 
		* open configs from the wireless side
* weak security configs
	* digital security works great until it doesn't 
	* too old - DES (Data encryption standard) encryption 
		* easy to break today 
	* encryption vulns - WEP (Wired equivalent privacy)
	* hash collisions - SHA-1 (secure hashing algoritm 1)
* personel issues 
	* people are the weakest link
	* policy violations 
	* insider threats 
		* auth users have more free reign than non authed
		* important to assign the correct rights and permissions 
		* give just the right amount of permissions 
	* social engineering 
		* so willing to help other 
	* social media
		* posting of internal info
		* public companies must not disclose meaningful info 
	* personal emails
		* emails sent from work imply endorsement by organization 
* unauthorized software
	* you don't know where the software comes from 
	* conflicts 
		* may conflict with internal software
	* licensing
		* you may need to pay for the business version 
	* ongoing support
		* who's going to upgrade the software
* baseline deviation 
	* everything should be well documented 
	* any chances need a history 
	* no remote access until everything matches a baseline '
		* like a health check from before
* license compliance violation
	* integrity 
		* data and apps must be accurate and complete 
		* a missing/bad license may cause problems with data integrity
* asset management 
	* id and track computer assets 
	* respond faster if there is a security issue 
	* keep track on most valuable assets 
	* track licenses and updates 
	* verify that all devices are up to date
* auth issues 
	* determine if someone is really who they say they are 
	* factors 
		* the more the better 
		* the more, the more chance of problems 
	* a lapse of any auth can open an entire network 