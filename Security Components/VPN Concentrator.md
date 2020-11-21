VPN Concentrator

* VPN - an encrypted private data traversing a public network 
* concentrator
	* encryption/decrytion access device
	* often integrated into a firewall
	* sometimes hardware or software 
	* used with a web client or built into the os 
* remote access VPN
* ![e6b34c94d826221e3270a7f705a43068.png](../../_resources/6228a621436c4e4c888adb5fa57878c7.png)
	* on demand access from a remote device 
	* can be configured as always on
* SSL VPN
	* uses 443 
	* amost no firewall issues because of the port
	* mostly in browsers 
	* sign in with your normal auth
* full tunnel
	* all traffic sent to the VPN first 
	* like PIA
* split vpn tunnel
	* Traffic going to the corprate network goes to them, all public traffic goes like normal 
* site to site 
	* always on 
	* ![e62cc5fe88bbfbe3d517263ce9e1e66d.png](../../_resources/b5438504ed55463f892fdcc87173b3a9.png)
* IPSec (Internet Protocol security)
	* OSI Layer 3
	* confidentiality and integrity/anti-replay 
	* very standardized
	* two core protocols
		* AH (Authention Header)
		* ESP (Encapsulation Security Payload)
	* Transport mode and tunnel mode
		* ![0d112b3fc5e9f830403ab700fab0bacf.png](../../_resources/36e93e9666414cbb80503006bb979f4a.png)
		* transport - data is encypted 
		* tunnel - data and IP header are encrypted so they don't know where the data is going from the encrypted info
	* AH
		* hash of the packet and a shared key 
		* ![29022c9e626bcaaf5b639dc352093149.png](../../_resources/3c2457f129ac4089983d31b9ae144778.png)
	* ESP
		* encrypts the packet 
		* ![ffcf3e17e98e2ac6b1194983f071ed9a.png](../../_resources/d18c3d4ef0cf44eda99e50bcbf1771fb.png)
		* 