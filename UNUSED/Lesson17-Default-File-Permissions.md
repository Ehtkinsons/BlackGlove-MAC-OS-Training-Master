## Default File Permissions 

### Objectives:

At the end of this episode, I will be able to:

1. Describe the default file permissions created automatically by macOS. 
2. Describe the function and purpose of the "Shared" folder in a user's home directory.
3. Repair damaged permissions using the Disk Utility. 

>Additional resources used during the episode can be obtained using the download link on the overview episode.

-----------------------------------------------------------

* Home Folder Structure
	+ Read access is granted to parts of a user's home
	  folder by default
	+ Designed to facilitate sharing data
	+ Users should be aware of the default settings
	+ [Default Home Folder Permissions][]
	+ Permissions of note:
		- Everyone has *read* permissions to a user's home
		  folder (including guest)
		- Everyone has *read* permissions on the Public folder
		- Everyone has *write* permissions on the Drop Box
		  folder, but not *read* permissions
		- All other folders are secured to the user
		- It is important that private documents not be
		  stored in the users root home folder
* The Shared folder
	+ A default "Shared" folder is provided to allow users
	  to exchange data
	+ /Users/Shared
	+ All users have read/write permissions on the folder
	+ However, special permissions are applied that prevent
	  one user from deleting another user's data
	+ Special permission is referred to as the *Sticky Bit*
		- Special directory flag
		- Indicates files in a directory can only be renamed or
		  deleted by the file owner, or root
		- Used in shared folders with multiple user's data
		- Each user can copy their own data in
		- Each user can read everyone else's data
		- Each user can only delete/rename their own data
		- e.g. /tmp
		- Terminal Commands
			+ `chmod -R +t <directory>`
			+ `ls -l <directory>`
		- Example without sticky bit:
			+ `drwxr-xr-x  2 donpezet  staff  68 Feb 15 21:00 temp`
		- Example with sticky bit:
			+ `drwxr-xr-t  2 donpezet  staff  68 Feb 15 21:00 temp`
* Repairing Permissions
	+ File and Folder permissions can become damaged
		- Improper user actions
		- Target mode
		- Backup/Restore
		- Malicious software
	+ Permissions can easily be repaired
	+ Disk Utility
		- Disk Utility can be used to scan the entire disk and repair permissions wherever they deviate from Apple's best practices
		- `Disk Utility -> Select Volume -> First Aid`
* Removable Media
	+ USB sticks, thunderbolt hard drives, etc
	+ Move from computer to computer
	+ Makes tracking an owner very difficult
	+ Owner may not exist on other systems
	+ UID of owner may be assigned to another account
	+ As a result, permissions are not terribly useful on 
	  removable media
	+ Apple disables ownership on removable and non-system
	  internal disks by default
	+ Can be changed
		1. Select the removable disk
		2. `Command-I`
		3. Check/Uncheck "Ignore ownership on this volume"
	+ Effectively kills permissions on the disk
	+ Allows all users access to the media

#### Default Home Folder Permissions

```
rwxr-xr-x	/Users/donpezet
rwxr-----	/Users/donpezet/Desktop
rwxr-----	/Users/donpezet/Documents
rwxr-----	/Users/donpezet/Downloads
rwxr-----	/Users/donpezet/Library
rwxr-----	/Users/donpezet/Movies
rwxr-----	/Users/donpezet/Music
rwxr-----	/Users/donpezet/Pictures
rwxr-xr-x	/Users/donpezet/Public
rwx-wx-wx	/Users/donpezet/Public/Drop Box
```