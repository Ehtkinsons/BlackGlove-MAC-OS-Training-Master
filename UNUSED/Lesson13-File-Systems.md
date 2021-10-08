## File Systems 

### Objectives:

At the end of this episode, I will be able to:

1. Describe the file systems available in macOS including APFS, Mac OS Extended, exFAT and NTFS. 
2. Differentiate between the file systems and identify their benefits and drawbacks. 


>Additional resources used during the episode can be obtained using the download link on the overview episode.

-----------------------------------------------------------

* Apple File System (APFS)
	+ Introduced in macOS High Sierra
	+ Designed for all Apple platforms (iOS, macOS, tvOS and watchOS)
	+ Better encryption
		- Single key and multi-key
	+ Supports more files and larger partitions
	+ Case sensitive
	+ Initially only supported on SSD
		- Now supported on Fusion as well
		- Not supported on spinning disk (HDD)
* Mac OS Extended
	+ Most basic Apple format
	+ Unicode filenames
	+ File permissions
	+ Links and aliases
* Mac OS Extended (Journaled)
	+ Same as above, but with journaling support
	+ Journaling protects from unexpected failures
		- Power outage
		- Improper drive removal
	+ Write operations are committed to a protected area
	+ Writes are not committed until they are 100% received
	+ Write failure results in a roll-back of the change
	+ Leaves the original file intact 
* Mac OS Extended (Journaled, Case-Sensitive)
	+ Same as above, but obeys UNIX/POSIX case rules
	+ These are different files: 
		- `/Users/dpezet/Documents/FileName.txt`
		- `/Users/dpezet/Documents/filename.txt`
		- `/Users/dpezet/Documents/FILENAME.txt`
* Mac OS Extended (Journaled, Encrypted)
	+ Same as above, but with full disk encryption applied
	+ FileVault
* FAT32
	+ File Allocation Table (32-bit)
	+ Developed for DOS/Windows systems
	+ Considered the most compatible file system for removable media
	+ Not supported for boot volumes under macOS
	+ Very fragile with improper removal
* NTFS
	+ New Technology File System
	+ Developed for Windows NT systems
		- Windows XP, Vista, 7, 8, 10
	+ Microsoft Proprietary
	+ macOS can read NTFS, but not write
* ExFAT
	+ Extended File Allocation Table
	+ Replacement for FAT32
	+ Large disk support
	+ High degree of compatibility
	+ Useful for removable disks that go between Macs and PCs
	+ Fragile with improper removal
	+ Supported in macOS since v10.6
* UFS
	+ UNIX File System
	+ Supported up through v10.5
	+ Could still be read by v10.13
	+ Support removed
	+ DiskUtility cannot format UFS anymore
