Mobile Device Management 

* MDM (mobile device management)
	* BYOD or company owned 
	* certralized management of the mobile drives 
	* set policies on apps, data, camera, etc. 
	* manage access control 
		* force screen lock, pins to unlock device
* application management 
	* it's a challenge 
	* no all apps are written with security in mind 
		* malware is a growing concern
	* manage apps with a whitelist 
		* adds hours to setup and manangement over time
* content management 
	* MCM (Mobil Content Management)
		* secure access to data 
		* protect from outsiders
	* file sharing and viewing 
		* on site content (microsfot sharepoint, file servers)
		* cloud based (box, office )
		* DLP
			* prevent copy paste
			* ensure encryption is enabled
* remote wipe
	* remove all data from your mobile device in case of stolen or missing 
	* need a plan for this 
	* always have a backup 
		* your data can be removed at any time 
		* could happen as you're walking out the door
* geolocation 
	* percise tracking of the devices location 
	* can be used for good or bad
		* find you or find your phone 
	* modt phones provide an option to disable 
	* may be managed by the MDM
* geofencing 
	* some mdms allow for geofencing 
		* restrict or allow featurs when the device is in a particular area
	* camera only works when outside the office 
	* auth
		* only allow logins when the device is located in a perticular area 
* screen lock
	* all mobile devices can be locked
	* simple passcode or strong passcode depending on what is forced
	* fail too many times? erase the device 
	* define a lockout policy 
* push notification services 
	* information appears on the lock screen
	* can be managed from the MDM
* passwords and pins 
	* the universal help desk call, forgot password
	* mobile devices use multiple auth methods 
	* recovery process can be initialed from the MDM
		* security question to regain access to the device 
* biometrics 
	* you are the authentication factor 
	* may not be the most secure 
	* available to enable or disable in the MDM
	* can be managed per app 
* context aware auth
	* combine several context
		* normal IP
		* normal location 
		* normal bluetooth devices around?
	* an emerging technology 
* containeraization 
	* difficult to seperate business from personal
	* separate enterprise mobile apps and data
		* create a virt container for company data
		* limited data sharing 
		* storage segmentation keeps data serperate 
	* easier to wipe just the container not the entire phone 
* full device encryption 
	* even if lost all the data is safer
	* devices handle this in different ways 
		* android - strong/stronger/strongest 
	* encryption isn't easy but it's worth it
	* don't forget the password or it's gone forever 
		* backup the keys 