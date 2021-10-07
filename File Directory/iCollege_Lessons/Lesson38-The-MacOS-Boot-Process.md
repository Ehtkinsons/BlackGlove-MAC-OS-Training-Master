## The macOS Boot Process 

### Objectives:

At the end of this episode, I will be able to:

1. Describe the five phases of the macOS boot process.
2. Select the appropriate troubleshooting method based on the phase where a system stops responding properly. 

>Additional resources used during the episode can be obtained using the download link on the overview episode.

-----------------------------------------------------------

* macOS Boot Phases
	1. Firmware
	2. Booter
		+ File Vault
	3. Kernel
	4. System *launchd*
	5. Login
* STEP 1: **Firmware** (BootROM)
	- Stored in hardware
	- Power On Self Test (POST)
	- Extensible Firmware Interface (EFI)
	- Mac chime plays
	- Power light flashes
	- Appears as an Apple logo on the screen
	- If everything passes, moves on to boot selection
	- Allows the user to select which drive to boot
	- Uses *Startup Disk* system preference by  default
	- If FileVault is enabled, it boots from Recovery to unlock the disk
	- Executes the Booter
	- Troubleshooting
		+ Audible beep codes
		+ Power light flashing patterns
		+ Apple Hardware Diagnostics
			- Hold **D** while booting to access diagnostics
		+ Generally hardware issues requiring maintenance
		+ If no booter is found, a folder with a "?" is  displayed
		+ Startup disk could be incorrectly set
			- `System Preferences -> Startup Disk`
			- Can be set from Recovery also
		+ Boot to recovery and use Disk Utility to  repair the disk
* STEP 2: **Booter**
	- `/System/Library/CoreServices/boot.efi`
	- Loads the kernel and initial extensions
	- Basic extensions are cached by default
	- Booting in safe mode flushes the cache
	- Appears as a spinning wheel on the screen
	- When booting from Internet Recovery it displays as a globe
	- Turns over control to Kernel
	- Troubleshooting
		+ Attempt Safe Boot to flush the KEXT cache
* STEP 3: **Kernel**
	- Loads additional extensions as necessary
	- Starts underlying core (BSD)
	- Executes *launchd*
	- Troubleshooting
		+ Attempt Safe Boot to flush the KEXT cache
		+ Boot in verbose mode to see where the boot process halts
		+ Use target mode to remove newly added extensions
* STEP 4: **System** *launchd*
	- `/sbin/launchd`
	- Process ID #1
	- Executes remaining system processes
		+ `/System/Library/LaunchDaemons`
		+ `/Library/LaunchDaemons`
		+ `/System/Library/StartupItems`
		+ `/Library/StartupItems`
	- Displays login window
	- *loginwindow* process is owned by root at this stage
	- Troubleshooting
		+ Boot into Safe Mode
		+ Clear out caches in /Library/Caches
		+ Clear out preferences
				- `/Library/Preferences`
				- `/Library/Preferences/SystemConfiguration`
* STEP 5: **Login**
	- *loginwindow* process prompts for credentials
	- User provides credentials
	- *loginwindow* transitions to the user's credentials
	- *launchd* is executed on behalf of the user
	- Builds user interface
	- Executes launch agents
		+ `/System/Library/LaunchAgents`
		+ `/Library/LaunchAgents`
		+ `/Users/username/Library/LaunchAgents`
	- Finally, executes *Login Items*
		+ `System Preferences -> Users & Groups -> Select User -> Login Items`
	- Troubleshooting
		+ Perform *Safe Mode* login
			- Hold **Shift** while logging in
		+ Check/Remove Launch Agents and login items
			+ `/Users/username/Library/Preferences/loginwindow.plist`
