Load Balancers 

* distributes the load 
* invisible to the end user 
* large-scale implementations 
* fault tolerance 
	* server outages have no effect 
	* very fast convergence 
* ![af38a35ebf1d1a2fad9b2e9cacbeaef2.png](../../_resources/751efa33548c4eec88325fcd237afc45.png)
* scheduling 
	* round robin 
		* each server is selected in turn 
		* first to server a, then b, c, ...
		* weighted
			* priortizer the server use 
		* dynamic 
			* monitor the server load and distribute to the server with the lowest use
		* active/active load balancing 
			* use any active server at any time 
* affinity 
	* when an applicatoin requres communication to the same instance 
		* each user is stuck to the same server 
		* tracked through IP addresses or session IDs 
* active passive load balancing
	* some servers are active, others are on standby
	* if an active server fails the passive takes its place 