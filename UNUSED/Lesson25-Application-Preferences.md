## Application Preferences 

### Objectives:

At the end of this episode, I will be able to:

1. Describe the various locations macOS applications can store data. 
2. Describe the format and function of an Apple plist preference file.
3. Change the default application used when launching a file. 

>Additional resources used during the episode can be obtained using the download link on the overview episode.

-----------------------------------------------------------

* Application Binaries
	- Stored in multiple places
		+ `/Applications`
		+ `/Users/username/Applications`
* Application Files
	- `/Users/username/Documents`
* Application Preferences
	- Stored in multiple places
		+ `/Library/Preferences`
		+ `/Users/username/Library/Preferences`
		+ `/Library/Application Support`
		+ `/Users/username/Library/Application Support`
* Preference Files
	- Stored in `*.plist` files
	- `plutil -convert xml1 <file>`
	- `plutil -convert binary1 <file>`
* File Locking
	- Prevents modification by users
	- `Command-I -> General -> Locked`
	- `sudo chflags nouchg <file>`
* Launch Services
	- macOS tracks which programs can open a file type
	- Referred to as *Launch Services*
	- Stored in: 
		+ `/Library/Preferences/com.apple.LaunchServices.plist`
		+ `/Users/username/Library/Preferences/com.apple.LaunchServices.plist`
* Changing the default application for an extension
	- One time
		+ `Control-Click -> Open With`
	- Permanently
		+ `Control-Click -> Get Info`
