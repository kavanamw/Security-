Driver Manipulation

* **a manipulation of the driver software beacuse it is a trusted software from the OS POV**
* drivers control the interaction between the hardware and software of a system, easy to implant malicious software there
* hardware interactoins have senstive data
* shimming
	* windows shim, the windows compatibility layer 
	* malware authors write their own shims 
* refactoring 
	* metamorphic malware, a slight change to the malware so that anti-virus does not catch it
		* changes every time it downloads the executable
	* address NOP, loops, pointless code 
	* 