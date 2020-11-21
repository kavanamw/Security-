Cross Site Scripting - XSS

* often occurs on a single site 
* created from error in the developent taking advantage of the trust a user has for the site 
* types
	* non-persistent (reflected) XSS Attack
		* web site allows scripts to run in user input boxes
		* bad guys email a link that takes advantage of the vuln, runs a scriipt that send creds to the bad guy
		* script embedded in the bad URL and sends creds back to the attacker 
		* like an SQL Injection but scripts instead of just data returned 
	* persistent (stored) XSS Attack
		* is now persistent and everyone gets the payload 
		* no specific target, anyone on the page will run the script 
		* ex. blog post where anyone who read or shares the post will be infected 
* prevention
	* be careful when  clicking links in a message 
	* consider disabling javascipt, really annoying though
	* keep browser and apps up to date 
	* validate input, don't let users store scripts from an input