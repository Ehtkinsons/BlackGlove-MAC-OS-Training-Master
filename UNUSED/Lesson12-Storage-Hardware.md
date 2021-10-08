## Storage Hardware 

### Objectives:

At the end of this episode, I will be able to:

1. Describe the storage hardware supported by macOS. 
2. List the hardware detected by macOS. 
3. Locate the mount points automatically created by macOS. 


>Additional resources used during the episode can be obtained using the download link on the overview episode.

-----------------------------------------------------------

* Internal media is always present
	+ HDD
	+ SSD
	+ Will typically use Apple proprietary file systems
* Removable media is transient
	+ CD
	+ DVD
	+ USB
	+ Thunderbolt
	+ Fire Wire
	+ Will typically use non-proprietary file systems for compatibility
* System Information
	+ `Macintosh HD -> Applications -> Utilities -> System Information`
	+ Under `Hardware` you will find: 
		- SAS
		- SATA/SATA Express
		- Storage (Shows logical volumes/partitions)
		- Thunderbolt
		- USB
* Disk Utility
	+ `Macintosh HD -> Applications -> Utilities -> Disk Utility`
* *Hard Disks*
	+ Physical disks
* *Partitions*
	+ Logical boundaries created on the physical disk
	+ A disk must contain at least 1 partition to be used by the system
	+ macOS supports up to 16 partitions per disk
* *Volumes*
	+ A partition that has been formatted for use by the system
	+ A partition is not visible to the user until it is formatted into a volume
	+ macOS mounts volumes to `/Volumes` by default
* GUID
	+ Globally Unique Identifiers
	+ GUID Partition Table (GPT)
	+ Default partition scheme for modern Macs
	+ Supported by Windows and Linux also
* APM
	+ Apple Partition Map
	+ Legacy partition map scheme
	+ Used on PPC-based Macs
* MBR 
	+ Master Boot Record
	+ Legacy partition map scheme
	+ Most widely supported
* NOTE: System disks under macOS Mojave need to be GPT

