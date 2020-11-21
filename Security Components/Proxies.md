Proxies 

* **sits between the users and the external network**
* receives the user request and sends the request on their behalf
* useful for caching information, access controll, URL filtering, content scanning 
* explicit 
	* applications may need to known how to use the proxy
* transparent 
	* the uses in the middle do not know it is being used
* application proxies 
	* one of the simplest proxies is NAT 
	* app proxies 
		* understands the wayt the application works 
	* the proxy may only know one application 
		* HTTP
	* most proxies are multipurpose
* forward proxy
	* an internal proxy 
		* commonly used to pretect and control user access to the internet 
		* ![fd7443e5c01edbb09c51e1fdbab72bb2.png](../../_resources/1a10c69ff6c4482ebb5ad08850c66f78.png)
		* URL Filtering 
* reverse proxy
	* inbound traffic from the internet to your internal service 
	* ![dd9dbe1657e16833a41bb017ba85246b.png](../../_resources/92e6e7e4ae9c44229ecb14e64b1c8bf5.png)
	* like self hosted stuff 
* open prixy 
	* a third party, uncontrolled proxy 
	* can be a significant security concern 
		* they are a man in the middle 
	* used to circumvent existing security controls 
	* ![a5a5901411ede93a21574f3ea604d47e.png](../../_resources/d4091f6e36814a78b369ba5188effaec.png)