Hardware Security

* full disk encryption (FED)
	* protects all your data as well as OS
	* unencrypted with a password
	* data protected when moving drive to another drive 
	* often built in to the OS
* Trusted Platform Module (TPM)
	* a specific piece of hardware to do the encryption stuff
	* cryptographic processor
		* random num generator, key generator
	* persistent memory 
		* comes with unique keys burned in
	* versatil mem
		* stoarge keys, hardware config info
	* TMP is password protected 
* Hardware Secuirty Module (HSM)
	* a high end encryptic hardware
		* plug in card
	* good for key backup in one place
	* often is an SSL accelerator 
	* used in large enviroments with large scalable security 
		* cluster and redudent power
* hardware root of trust
	* security is based on trust 
	* the TPM and HSM are the root of that trust
		* trusted because it is hard to circumvent 
		* security won't work without the hardware
* UEFI Bios
	* Unified extensible fireware interface 
		* based on Intel's EFI (Extensible firmware interface)
	* defigned to replace the legacy BIOS
		* needed for modern computers
* Secure boot
	* malicious software can "own" your system at boot
	* secure boot is part of the UEFI specs
	* degitally sign known-good software 
		* crypto secure
		* software won't run without proper signature 
	* supports many different os
		* apple has their own
* remote attestation
	* nothing on the computer has been changed since the last boot
	* good for a large set of machines 
	* device provides an operational report to a verification server 
	* encrypts the digitally signs the report with the TPM
	* changes are IDed and managed before the OS is booted
	* if differences are found then it won't boot
* supply chain
	* adding a backdoor at the time of manufacturing 
	* use trusted vendors
	* critical devices should not be connected outside before being behind the firewall
	* verify that hardware is legit
* EMI/EMP
	* electromagnetic interference/electromagnetic pulse
	* EMI leakage
		* determine data streams based on EMI emmissions 
		* keyboards, hdd, network connections
	* modify the security by injecting EMI
	* shielding against EMI is important for important systems 