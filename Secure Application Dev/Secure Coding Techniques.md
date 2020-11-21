Secure Coding Techniques

* Secure Coding Techniques
	* a balance between time and quality
	* test in the QA process
	* vuln will be found 
		* secure coding conecpts to minimize this
* error and exception handling 
	* what happens when an error occurs
	* network connetion fails, database unaviable 
	* mishandled exceptions can allow execution of code
	* don't use default errors 
		* defaults will leak more info than needed
* input validiation 
	* what is the expected input
	* document all input methods 
		* forms, fields, etc
	* normalization - check and correct all input 
		* a zip code should be only numbers and a set length
		* fix any data with inproper inputs before storing 
	* fuzzer 
		* send random input to test app input handling 
* Stored procedures
	* SQL databases
		* client sends detialed requests for data
		* ex. 'SELECT * from wp_options WHERE option-id = 1'
	* client requets can be complex and sometiems modified by the user
	* stored procedures - limit the client interaction 
		* ex. 'CALL get_options'
			* CALL stored procedure 
		* that's it, no modifications to the query are possible
		* no SQL calls across the network
* Code signing 
	* an app is deployed 
	* security questions 
		* has the app been modified?
		* can you confirm that the app was written by a specific dev?
	* app signing - code can be digitally signed by the dev
		* asymmetric encryption
		* a trusted CA signs the dev's public key
		* dev signs the code with their private key
		* for internal apps, use your own CA
* encryption
	* if you can see the source code, you can look for security holes
		* source code well guarded
	* if you're sending data over the network it should be encrypted
	* data at rest should be encrypted
		* either from the os or from the app
* obfuscation/camo
	* obfuscate - make something normally understandable very difficult to understand
	* takes readable code and turns it into nonsense 
		* dev keeps readable code and gives you unreadable
	* helps prevent the search for security holes 
	* ![51f0d3c951b7b39473eae84430019891.png](../../_resources/80c657bf7bc5445b876a0f6e057cc9cd.png)
* code reuse/dead code
	* code reuse - old code to build new apps
	* if the old code has security problems than yours does too
	* dead code - running an exe, results are tallied 
		* results are not used
	* any code is a securty problem, remove dead code to tighted security
* validation points
	* server side validation 
		* all checks occur on the server 
	* client side validation
		* the end user side 
		* can filter legitimate inputs from genuine users
		* may speed up validation process
		* bad for security 
	* use both 
* memory management 
	* never trust data input 
		* malicious users can attempt to circumvent your code
	* buffer overflows are a a huge security risk 
		* make sure that your data matches you buffer size
	* some built in functions are insecure 
* third party libraries and SDK's
	* extend the functionality of a programming lang
	* security risk
		* app code written by someone else 
		* might be secure, might not 
		* extensive testing is required
	* balancing act
		* speed vs security
* Data exposure
	* how is the app handling the data
		* no encryption when sotres
		* no encryption on the network 
		* dispaying info on screen
	* all input and output proceses are important 