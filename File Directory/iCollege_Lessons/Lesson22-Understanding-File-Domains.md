## Understanding File Domains 

### Objectives:

At the end of this episode, I will be able to:

1. Describe the function and use of file domains in macOS. 
2. Select the appropriate file domain for a preference or file. 

>Additional resources used during the episode can be obtained using the download link on the overview episode.

-----------------------------------------------------------

* File Domains
	+ System resources are stored in *Libraries*
	+ System resources can be stored in one or more *Library*
	+ Referred to as *domains*
* Folder Domain Preference
	+ Each location is searched in a particular order
	+ Allows base functionality to be overridden
	+ File Domains Locations and Order
		1. **User**
			- `/Users/username/Library`
		2. **Local**
			- `/Library`
		3. **Network**
			- `/Network/Library`
		4. **System**
			- `/System/Library`
* Extensions
	- Drivers
	- Provide support for various hardware devices
	- Printers, network adapters, storage, etc
	- Generally installed with packages
	- `/Library/Extensions`
	- `/System/Library/Extensions`
* Fonts
	- Typeface definitions responsible for how text is rendered on screen
	- `/Library/Fonts`
	- `/Users/username/Library/Fonts`
	- `/System/Library/Fonts`
* Frameworks
	- Libraries containing shared code
	- Prevents applications from having to maintain separate copies of the same data
	- `/Library/Frameworks`
	- `/Users/username/Library/Frameworks`
	- `/System/Library/Frameworks`
* Logs
	- Text logs maintained for the system and applications
	- `/Library/Logs`
	- `/Users/username/Library/Logs`
* Preferences
	- Application and operating system settings
	- `/Library/Preferences`
	- `/Users/username/Library/Preferences`
* Managing Fonts
	+ macOS includes a utility for managing fonts
	+ `/Applications/Font Book`
	+ Double-clicking a font file will present you with the opportunity to install it
	+ Users can install a font for themselves
		- `Font Book -> Preferences -> Default Install Location -> User`
		- `/Users/username/Library/Fonts`
	+ Administrators can install it globally
		- `Font Book -> Preferences -> Default Install Location -> Computer`
		- `/Library/Fonts`
	+ Example Fonts
		- [http://tulrich.com/fonts](http://tulrich.com/fonts)

-----------------------------------------------------------
### External Resources:

During this episode, you can reference the following external resources for supplementary tools and information:

- [http://tulrich.com/fonts](http://tulrich.com/fonts)
