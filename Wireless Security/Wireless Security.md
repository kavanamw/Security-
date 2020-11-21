Wireless Security 

* wirless security modes 
	* config the authenticaor on your wireless access point/router 
	* open system 
		* no auth password is needed
	* WPA-Personal/WPA-PSK
		* WPA2 with a pre-shared key 
		* everyone uses the same 256-bit key 
	* WPA-Enterprise/WPA-802.1X
		* authenticated users individually with an auth server (i.e. RADIUS)
* captive portal 
	* auth on the network 
		* common on wireless networks 
	* access table recognizes a lack of authentication 
		* redirects your web access to a captive portal page 
	* username/password 
		* add additional auth factos 
			* random key generators 
	* once proper auth is provided the web session continues 
		* until the captive portal removes your access
* using WPS
	* Wi-Fi protected setup 
		* originally called Wi-Fi simple config 
	* allows "easy" setup of a mobile device 
		* a passphrase can be complicated 
	* different ways to auth
		* PIN configured on access point must be entered on the mobile device 
		* push a button on the access point 
		* NFC 
		* USB method - no longer used 
	* the WPS hack 
		* December 2011 design flaw 
		* PIN is an 8 digit number 
			* really a 7 digits and a checksum
			* 7 digits, 10,000,000 possible combos 
			* the WPS process validates each half seperatly 
				* 4 digits, 3 digits and a checksum
				* only really needed 11,000 possibilities 
				* brute force lockout features are now the norm 
	* best practice is to disable WPA entierly 