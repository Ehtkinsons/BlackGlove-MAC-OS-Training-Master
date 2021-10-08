## Introduction to macOS Recovery 

### Objectives:

At the end of this episode, I will be able to:

1. Describe the purpose and function of the macOS Recovery partition. 
2. Boot a system into recovery mode and access recovery tools. 
3. Describe the tools available within the Recovery environment.

>Additional resources used during the episode can be obtained using the download link on the overview episode.

-----------------------------------------------------------

* Potential sources of errors
	+ Failing RAM
	+ Bad sectors on HDD
	+ Bad memory blocks on SSD
	+ Accidental deletion
	+ Corrupt file system
	+ Malware/Ransomware
* Error Symptoms
	+ Freezing during boot
	+ Frequent spinning color wheels
	+ Applications failing to run
	+ Files becoming corrupt
	+ System fails to boot
	+ Operating system not found
* Time Machine
	+ Restore deleted/damaged files
	+ Restore entire disk
* Disk First Aid
	+ Recover from disk errors
	+ Reset file permissions
* Reinstall macOS
	+ Restore damage/missing OS files
	+ Repair disk boot files
* If it is a hardware issue, you have to fix the hardware first
* Recovery volume
	+ Stripped down version of macOS
	+ Allows access to recovery tools independent of the installed OS
	+ Allows re-installing macOS
	+ Used to be on the installation media
	+ Installation media is no longer included with a new Mac
	+ Recovery volume is on the local disk
		- Hidden partition
		- Allows you to boot to recovery without installation media
	+ Not particularly helpful if your HD fails
* Alternative Recovery Locations
	+ USB install media
		- Follow [these instructions](https://support.apple.com/en-us/HT201372) to create installation media
	+ Time Machine backup disks
	+ Internet Recovery
		- Added in OS X 10.9
* Boot-time shortcuts
	+ `Option`
		- Displays boot menu
		- Used when booting from USB, Time Machine or Internet Recovery
	+ `Command + R`
		- Reinstall same version of macOS that was previously installed
	+ `Option + Command + R`
		- Upgrade to the latest version of macOS supported
	+ `Shift + Option + Command + R`
		- Install the version of macOS that shipped with your hardware
* Using the internal recovery partition
	1. Power off the computer
	2. Power on the computer while holding `Command + R`
	3. Release `Command + R` when you see the Apple logo
	4. Select `Reinstall OS X`
* Available Tools
	+ Install OS X or Reinstall OS X
	+ Get Help Online
	+ Disk Utility
	+ Startup Disk
	+ Firmware Password Utility
	+ Network Utility
	+ Terminal

-----------------------------------------------------------
### External Resources:

During this episode, you can reference the following external resources for supplementary tools and information:

- [Creating macOS Installation Media](https://support.apple.com/en-us/HT201372)
