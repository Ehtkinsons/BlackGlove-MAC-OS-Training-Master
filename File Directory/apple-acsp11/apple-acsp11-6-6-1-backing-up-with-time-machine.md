## Backing Up with Time Machine 

### Objectives:

At the end of this episode, I will be able to:

1. Configure Time Machine to backup a computer running macOS.
2. Verify a backup completed successfully.
3. Describe the supported destinations for a Time Machine backup. 

>Additional resources used during the episode can be obtained using the download link on the overview episode.

-----------------------------------------------------------

* Time Machine
	+ Easy to use backup system
	+ Provides ongoing backups to another disk
	+ By default backs up every hour
		- If a removable disk is used, it must be present
		- Changed files are tracked and backed up on schedule
		- Only changed files are copied
		- The entire file is copied
			+ That is a problem for large files, as each copy is maintained
	+ Backups are stored as a large series of hard links to unchanged files alongside the changed files
	+ When space runs out, oldest backups are deleted
	+ The larger the backup drive, the further back you can restore
* Hardware Requirements
	+ Can back up to any disk other than the system volume
	+ A secondary disk is recommended
* Time Machine Encryption
	+ Can be encrypted
	+ DEMO: Enabling Time Machine with Encryption
* Local Snapshots
	+ A local backup cache is kept
	+ Called a local snapshot
	+ Enabled by default
	+ Can be viewed in terminal
		- Terminal needs "Full Disk Access" permissions
		- `sudo tmutil listbackups`
		- `sudo tmutil listlocalsnapshots /Volumes/Macintosh\ HD`
* Network Backups
	+ Backup to a network share hosted on a macOS server or Time Capsule WAP
	+ DEMO: Network Backup

