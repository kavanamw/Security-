Cross Site Request Forgery - XSRF, CSRF (sea surf)

* takes advantage of the trust between a browser and a website 
	* the website trusts your browser
* dev oversite 
	* should have anti-0forgery techniques added 
		* often a cryptographic token to prevent forgery
* ex.
	* bad guys creates a funds transfer request from someone elses account 
		* needs someone else to do the transfer for him
	* sends a bad url to a victum 
	* sends the reuqest to the bank to make the bank transfer to the bad guy
* prevention
	* you need to make sure the requests actually come from the user you think they do 