Redundancy, Fault Tolerance, and High Availability 

* distrubutive allocation 
	* bad guys looking for you data 
	* web servers, database serversm middleware 
	* don't keep everything in one place 
		* critical assets, data and other system should be in differenet places 
		* easier to add secuirty between layers 
		* more difficult to target
* redudancy and fault tolerance 
	* maintain uptime 
	* no hardware failure should stop a service 
	* no software failure should stop a service 
	* no system failure so network works around the problem 
	* redudant hardware 
		* multiple devices, load balacncing power supplies 
		* RAID - redudent array os independent disks 
			* one drive fails, the rest take over
		* UPS
			* power supply 
		* clustering 
			* a logical collective of server 
			* any servers fail the rest of the cluster takes the load 
		* load balancing 
			* if a server fails it balances the load on the remaining servers 
* RAID
	* 0 - striping without parity 
		* high preformance but no fault tolerance 
	* 1 - mirroring 
		* duplicates data for fault tolerance 
		* lower performance and higher data cost 
	* 5 striuping with parity 
		* fault tolerant
		* only requires and additional disk for redudency 
	* 0+1,1+0,5+1, etc
		* multiple raid types 
		* combine raid methods to increase redudency 
* high availability 
	* redudency doesn't alway mean always available 
		* may need to be enabled manually
	* HA (high availabity)
		* alway on, always available 
	* many include many different componsents working together 
		* watch for single points of failure 