Mobile Device Enforcement 

* apps stores 
	* not all apps are secure
	* some have vulns and data leakage 
	* not all apps are approprate for business use 
	* MDM can allow or deny app store use 
* rooting/jailbreaking
	* most users don't interact directly with the os
	* android - rooting 
	* apple - jailbreaking
	* install custom firmware 
	* uncontrolled access
		* circumvent security features, sideload apps
		* the MDM becomes useless
* carrier unlocking
	* most phones are locked to a carrier 
	* the cost is subsitzed to the monthly plan cost
	* you can unlock your phone if your carrier allows it
	* security revolves around connectivity 
		* moving to another carrier can circumvent the MDM
		* preventing a sim unlock may not be possible on a personal device 
* firmware and OTA updates
	* over the air updates, no cable requred
	* may or may not be a good thing
		* the MDM can manage what OTA updates are allowed 
* camera use
	* not always good on a corperate device 
		* corporate espionage, innappropriate use 
	* almost impossible to control on the device 
	* cameras can be controlled by the MDM
		* always disabled
		* enabled outside of work
* SMS/MMS
	* control of data can be a concern 
	* outbound data leaks
	* inbound notifications, phising attempts 
	* MSM can enable or disable this feature 
* external media
	* when plugged in looks like a flash drive to the computer 
	* limit data written to removedable drives
	* can be disabled via the MDM
* USB OTG
	* usb on the go
	* connect mobile devices directly together 
	* no computer required
	* mobile device is both a host and a device 
	* a usb  standard 
	* extreamly convient 
	* can be disabled on the MDM
* microphone 
	* audio recordins 
	* useful for meetings and note taking 
	* a legal liability 
		* every state has different laws
	* enabled or disable in MDM
* geotaggin/gps tagging
	* your phone knows where you are 
	* adds your location to document metadata
	* every document may contain geotagged info
	* may be a securty concern 
		* photo Exif data
* wifi direct/ad hoc
	* connect devices to eachother
	* called ad hoc mode 
	* wifi direct
		* easily connect many devices together 
		* has some vulns 
* hotspot/tethering 
	* turn your phone into a wifi hotspot 
	* denendent on the phone and carrier 
	* may provide inadvertent access 
		* a rouge access point to the internal netwokr
	* can be enabled or disabled from the MDM
* Payment methods
	* send small amounts of data wirelessly over a limited area 
	* a few different standards
	* bypasses primary auth would allow payments 
		* use proper securirty or disable completly 
	* MDM