## File System Maintenance 

### Objectives:

At the end of this episode, I will be able to:

1. Describe techniques you can use to prevent file system corruption.
2. Properly prepare a disk for safe removal from a system.
3. Use the Disk Utility to repair damage caused by improper drive removal.

>Additional resources used during the episode can be obtained using the download link on the overview episode.

-----------------------------------------------------------

* Maintenance Tasks
	+ Reactive
		- Error is detected
		- Must be corrected
	+ Proactive
		- Preventative maintenance
		- Performed to prevent an error
* Proper ejecting
	1. Drag the disk icon to the Trash
	2. Click the eject icon next to the disk in the finder navigation tree
	3. Highlight the disk in Finder and click `File -> Eject`
* Force ejecting
	+ Disks should be properly unmounted before being removed
	+ Failing to do so can result in corrupted files
	+ Especially with FAT32/ExFAT disks
	+ Sometimes a disk is "stuck"
	+ Normally the result of an open application
	+ If so, you have a few options:
		1. Logout and log back in again, then try to eject. 
		2. Shutdown and unplug the disk.
		3. Unmount the disk using the Disk Utility
* Identifying rogue disk access
	+ Not easily
	+ Spindump will list all processes and their related disk activity
		1. Launch Activity Monitor
		2. `Gear -> Spindump`
	+ You may also find information in the Console logs
* Disk Utility can help if disk corruption occurs
	+ Not fool-proof
	+ `Disk Utility -> Select Disk -> First Aid`
		1. Verify Disk
		2. Repair Disk
		3. Fix Permissions
	+ Use Recovery if it is the system disk
* Target Mode
	+ Allows turning your Mac into an external disk
	+ Attach it to another Mac, as if it were a peripheral
	+ Steps
		1. Shutdown Mac
		2. Boot while holding "T" 
		3. Connect to another Mac using Thunderbolt or Fire Wire
	+ Once connected, you can use Disk Utility on the second Mac.

