## Initial System Configuration 

### Objectives:

At the end of this episode, I will be able to:

1. Locate configuration options in the macOS system preferences.
2. Describe using the Migration Assistant to copy settings from an existing machine. 

>Additional resources used during the episode can be obtained using the download link on the overview episode.

-----------------------------------------------------------

* Steps that every user should take immediately following installation
* These are considered the minimum
* Basic steps:
	+ Migrate previously existing data
	+ Configure networking
	+ Configure user accounts
	+ Adjust general system preferences
	+ Configure software updates
* Using the Setup Assistant
	+ Launched immediately following an installation
	+ Provides users with an easy wizard to provide an initial configuration
	+ Items include:
		- Region
		- Keyboard Definition
		- Wi-Fi / Network Configuration
		- Migration Assistant
		- Apple ID Creation and Sign-In
		- Initial Administrative Account Creation
		- Warranty / Support Registration
* Migration wizard is run upon initial boot of macOS
* Can be run at any time
	1. Launch Finder
	2. Browse to `Applications` -> `Utilities`
	3. Launch Migration Assistant
* Can import data from multiple sources
	+ Another Mac
		- Automatically locates other Macs on the network (Wired or wireless)
		- You can connect two Macs via Ethernet cross-over cable
		- You can connect two Macs via Ethernet / USB-C
		- Basic Steps
			1. On source, launch Migration Assistant
			2. Choose "To another Mac"
			3. On target, launch Migration Assistant
			4. Choose "From another Mac"
			5. Follow the on-screen instructions
	+ Time Machine Backup
		- Attach a disk to the system containing the Time Machine backup from your previous system
		- Migration Assistant will automatically find the backup and restore your data
	+ Startup Disk
		- Attach the startup disk from your previous system to your new system
		- Several methods available
			+ Attach via external connector (USB, Fire-wire)
			+ Remove the disk from the old system and install it as an additional disk to your new system (most Macs do not have room for this)
			+ Put your old system in "Target Mode" by holding "T" while booting. Then attach the old system to your new system via Fire-wire or Thunderbolt.
	+ Windows PC
		- You must install and run the Migration Assistant on your Windows PC
		- Detailed instructions can be [found here](https://support.apple.com/en-us/HT204087)
		- The Mac will scan the network until it finds the PC
		- A PIN number is displayed on the PC that must be entered on the Mac for basic authentication
* Five Categories of System Preferences
	+ Personal
		- Settings that affect the user experience
		- Typical Items
			+ Desktop & Screen Saver
			+ Dock
			+ Language & Region
			+ Notifications
	+ Hardware
		- Settings that define how hardware functions
		- Typical Items
			+ Displays
			+ Energy Saver
			+ Keyboard
			+ Printers
	+ Internet & Wireless
		- Settings that control network access
		- Typical Items
			+ Internet Accounts
			+ Network
			+ Sharing
	+ System
		- Settings that influence Operating System behavior
		- Typical Items
			+ Users & Groups
			+ Date & Time
			+ Startup Disk
			+ Time Machine
	+ Other
		- Third party preference utilities
		- Typical Items
			+ Java
			+ Logitech Control Center
			+ Proprietary Hardware Utilities

-----------------------------------------------------------
### External Resources:

During this episode, you can reference the following external resources for supplementary tools and information:

- [Move your data from a Windows PC to your Mac](https://support.apple.com/en-us/HT204087)