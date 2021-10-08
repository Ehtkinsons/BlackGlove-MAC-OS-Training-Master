## Building Installation Media 

### Objectives:

At the end of this episode, I will be able to:

1. Describe how macOS software is distributed. 
2. Build a USB installation media for macOS. 

>Additional resources used during the episode can be obtained using the download link on the overview episode.

-----------------------------------------------------------

* Obtaining macOS
	+ macOS is pre-installed on all new purchases
	+ macOS is available through the Mac App Store as a free download
	+ The installer is only visible to OS X 10.8 and higher
	+ Download is a little over 5GB
* macOS Physical media
	+ Installation media is not provided in a physical form
	+ You can create your own physical media from any mac
* Once downloaded, you can create physical media
	+ [How to create a bootable installer for macOS](https://support.apple.com/en-us/HT201372)
* To create a physical USB installation media:
	1. Download the macOS installer on any machine running OS X 10.8 or higher
	2. Get a USB flash drive or HD with at least 8GB of storage
	3. Format the removable drive using Disk Utility
		- NOTE: All contents will be lost
	4. From the terminal execute:
		- `sudo /Applications/Install\ macOS\ Big\ Sur.app/Contents/Resources/createinstallmedia --volume /Volumes/Untitled`
* Uses for installation media
	+ Install macOS
	+ Repair macOS
	+ macOS Recovery
	+ Troubleshooting

-----------------------------------------------------------
### External Resources:

During this episode, you can reference the following external resources for supplementary tools and information:

- [How to create a bootable installer for macOS](https://support.apple.com/en-us/HT201372)