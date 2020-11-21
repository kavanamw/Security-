Virtualization Overview

* virtualization 
	* one computer, many os 
	* seperate os, independent CPU. mem, network, etc
		* but really one physical computer
	* host baded virt
		* normal desktop plus others 
	* standalone server that hosts virt machines 
		* enterprise level
* the hypervisor
	* virt machine mananger 
		* manages the cirt platform and guest os 
	* many require a CPU that supports virt
	* hardware management 
		* CPU
		* networking 
		* security 
	* type II
		* runs on top of the os 
	* type I
		* bare metal, embedded, native 
		* runs directly with hardware, no os needed
	* app containerization 
		* runs an app without launching an entire vm
		* use just the needed resources to run the app
		* all dependencies are contained withing the container install 