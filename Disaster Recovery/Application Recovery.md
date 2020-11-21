Application Recovery 

* Order of restoration 
	* not all apps have the same priority 
	* this list should be defined well before it's needed
		* management sets it 
	* the order may change based on the time of year 
		* monthly, quarterly apps may take priority 
* backup strategies 
	* backup tech
		* tape, disk, optical 
	* database backups 
		* replication - online duplicates 
		* online backups - specialized backup processes for databases 
	* email database backups 
		* provide server, database, mailbox, or message backup and restore 
	* snapshots 
		* OS volume snapshots or hypervisor snapshots 
	* system backups 
		* bare metal backup using images 
* file backups 
	* the archive attribute 
		* set when a file is modified 
	* archive bit 
		* set when the file is modified 
		* indicated the file is ready for arciving 
		* when backup happens, the archive bit is cleared 
	* full backup
		* everything 
		* you'll want this one first 
	* incremental 
		* all files changed since the last incremental backup 
	* differential 
		* all files changed since the last full backup 
* backup types 
	| Type | Data Selection | Backup/Restore Time | Archive Attribute |
	|------|----------------|---------------------|-------------------|
	| Full | All selected Data | High/Low (one tape set) | Cleared |
	| Incremental | New files and files modified since the last backup | Low/High (Multiple Tape Sets) | Cleared |
	| Differential | All data modified since the last full backup | Moderate/Moderate (No more than 2 sets) | Cleared |