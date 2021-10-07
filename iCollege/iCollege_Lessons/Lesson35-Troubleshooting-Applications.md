## Troubleshooting Applications 

### Objectives:

At the end of this episode, I will be able to:

1. Determine if a system error is caused by an application or hardware extension. 
2. Use Safe Mode, Safe Boot, and Verbose Mode to isolate the cause of a system error. 

>Additional resources used during the episode can be obtained using the download link on the overview episode.

-----------------------------------------------------------

* Application issues
	+ Poor performance
	+ Spinning wheel
	+ Lockup on boot
	+ Unable to login
	+ Random reboots
* Safe Mode
	+ Hold **Shift** while logging in
	+ Does not load Startup Agents and Launch Items
* Troubleshooting
	+ Disable all startup items
	+ Re-enable one-by-one
* SafeBoot
	- Hold **Shift** while booting
	- Flushes startup cache
	- Does not load third-party extensions
* Verbose Mod
	- Hold **Command-V** while booting
	- Displays text based output of boot process
* Troubleshooting Software
	+ Single User Mode
		- Hold **Command-S** while booting
		- Boots to CLI
* Sleep Mode
	+ Safe Sleep
		- Supported on all Macs with a battery
		- When going to sleep, all system memory is written to disk
		- If the device runs out of power, the memory is preserved on disk
		- On reboot, memory is copied from disk back to RAM
		- System resumes where it left off
	+ Automatic Sleep
		- Supported on Macs with SSD
		- Sometimes called Standby
		- When idle, the system goes in to a low power mode
		- Can be resumed with any keyboard/mouse interaction
	+ Power Nap
		- System enters sleep mode as usual
		- System awakens from low power mode periodically to check e-mail, perform time-machine backups, etc.
		- Display does not wake up
		- `System Preferences -> Energy Savers -> Enable Power Nap`
		- Set under battery and power adapter
