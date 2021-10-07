## Troubleshooting Peripherals 

### Objectives:

At the end of this episode, I will be able to:

1. Describe the types of peripherals supported by macOS and their connection types. 
2. Describe kernel extensions and their functions.
3. Verify the presence of drivers and kernel extensions in macOS. 
4. Troubleshoot hardware that is not detected by macOS. 

>Additional resources used during the episode can be obtained using the download link on the overview episode.

-----------------------------------------------------------

* Supported Devices
	- Storage
	- Imaging devices
	- Input devices
		+ Keyboards
		+ Mice
	- Output devices
		+ Displays
	- Communications devices
		+ Modems
		+ Network cards
	- Many more
* Bluetooth
	+ Short range wireless technology
	+ Up to 10m
	+ Bluetooth 3.0 up to 24Mbps
	+ Bluetooth 4.0 / Bluetooth Low Energy (BLE)
		- Normally in addition to Bluetooth 3.0
		- Provides rapid connection time
		- Low energy
		- Up to 200Kbps
* Serial ATA
	+ Serial Advanced Technology Attachment (SATA)
	+ Used in all current Macs
	+ Only one drive per channel
	+ Speeds up to 600MBps
* FireWire
	+ Also called IEEE 1394
	+ Up to 63 devices per controller
	+ Provides 2.5 watts of power
	+ FireWire 400 up to 400Mbps
	+ FireWire 800 up to 800Mbps
* USB
	+ Up to 127 devices per controller
	+ Provides 7 watts of power
	+ USB 1.1 up to 1.5Mbps
	+ USB 2.0 up to 480Mbps
	+ USB 3.1 up to 5Gbps (5,000Mbps)
* Thunderbolt
	+ Current devices ship with Thunderbolt 3
	+ Compatible with USB-C/DisplayPort
	+ Supports daisy-chaining up to 7 devices
		- Devices must have two Thunderbolt ports to support daisy-chaining
	+ Thunderbolt 1 up to 10Gbps per channel (2 channels)
	+ Thunderbolt 2 up to 20Gbps
	+ Thunderbolt 3 up to 40Gbps (USB-C)
* Drivers may be necessary for some devices
	+ In macOS, drivers come in three forms
		1. Framework Plugins
			- Hardware support is connected to an underlying framework
			- For example, OpenGL drivers
		2. Applications
			- Hardware support is provided by an app
			- For example, iTunes
		3. Kernel Extensions
			- Most drivers are loaded this way
			- Dynamically loaded
			- `/Library/Extensions`
			- `/Library/StagedExtensions`
			- `/Library/DriverExtensions`
			- `/System/Library/Extensions`
* Viewing active extensions on an M1 Mac
	+ `systemextensionsctl list`
* Drivers come in 32bit and 64bit
	+ macOS Big Sur is 64bit
	+ *System Information* shows which version you have
	+ `System Information -> Software -> Extensions`
	+ x86_64 = 64bit 
* See which devices are attached using *System Information*
	+ `System Information -> Hardware -> <bus>`
* Apple Hardware Test
	+ Hold **D** while booting
	+ Launches the hardware test from BootROM
	+ Holding **Command-Option-D** runs from Internet
