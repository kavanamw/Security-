Gathering Forensic Data

* forensic procedures 
	* collect and protect info 
		* many different data sources and protection mechanisms 
	* RFC 3227 - Guidelines for ecidence collection and archiving 
		* a good set of best practicies 
	* standard ditial forensic process 
		* acquisition, anaylsis, and reporting 
	* must be detialed oriented 
* order of colatility 
	* how long does data stick around 
		* some media is much more volatile than others 
		* gather data in order from the most volatile to the least volitale 
		* ![7b4faffeaaf329c9668b66f453302769.png](../../_resources/e3285ebb816b48af8253223f4262221d.png)
* chain of custody 
	* control evidence, maintain integrity 
	* everyone who contacts the evidence 
		* avoids tampering 
			* use hashes 
	* label and catelog everything 
		* sealed and stored 
* legal hold 
	* a legal technique to preserve relvent info 
		* prepare for impending litigation 
		* initiated by legal consel 
	* hold notification 
		* records custodians are instructed to preserve data
	* separate repo for electronically stored info (ESI)
		* many different data sources and types 
		* unique workflow and retention requirements 
	* ongoing preservation 
		* once notified, there's an ongoing obligation to preserve data 
* capture system image 
	* copy the contents of a disk 
		* bit for bit, byte for byte
		* get every morsel of info 
	* software imaging tools 
		* use a bootable device 
	* remove the physical drive 
		* use a hardware write blocker 
	* get backup tapes 
		* some of this work may have been done for you 
* network traffic and logs 
	* traffic logs 
		* very common
		* firewall logs a lot of info 
		* switches and routers don't usually log user-level info 
	* intrusion detection/prevention sytstems 
		* log usual traffic patterns 
	* raw network traffic data 
		* stream-to-disk 
		* an exact recording of network comm
			* rebuild images, email messages, browser sessions, file transfers 
* capturing video 
	* captures the status of the screen and other volatile info 
	* don't forget security camera and your phone 
	* the video must be archived 
* recording time offsets 
	* the time zone determines how the time is displayed 
		* document the local device settings 
	* different file systems store timestamps differently 
		* FAT: local time 
		* NTFS: time is stored in GMT
	* record the time offset from the OS
		* the windows registry 
		* many different values (daylight savings, time change info, etc)
* take hashes 
	* ensure no tampering 
	* MD5 (Message Digeste 5)
		* 128 bit hash 
		* displayed as hex
		* chance of duplication is 2^128
	* CRC (Cyclical Redundancy Check)
		* 32 bit, displayed as hex
		* chance of duplication is 2^32
	* create an MD5 hash for an image, file, or groups of files 
* Screenshots 
	* external capture 
		* digital camera or phone
	* internal capture 
		* from the OS
* witness 
	* who saw it 
	* interview and document 
	* do so quickly 
	* not all witness statements are 100% accurate 