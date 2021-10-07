## User Account Security 

### Objectives:

At the end of this episode, I will be able to:

1. Delete a user and their home directory from macOS.
2. Describe the methods of restoring a user account or its home directory. 
3. Describe the methods available for resetting a user's password. 

>Additional resources used during the episode can be obtained using the download link on the overview episode.

-----------------------------------------------------------

* Deleting a User Account
	+ `Apple Menu` -> `System Preferences` -> `Users & Groups`
	+ Select the user and click on `-`
	+ Three options
		1. Save the home folder in a disk image
			- User account is deleted and the contents of their home folder are stored in a .dmg file in `/Users/Deleted Users/`
		2. Don't change the home folder
			- The user account is deleted, but their home folder is left in place
			- `(Deleted)` is added to the end of the folder name
		3. Delete the home folder
			- Home folder is deleted, bypassing the trash bin
			- "Erase home folder securely" provides a data scrub to help prevent file recovery with 3rd party tools
* Restoring a deleted user
	+ There is no direct way to recover a user account
	+ If the home folder was not backed up, just create a new account
	+ If the home folder was backed up, follow these steps:
		1. Restore the home folder to the `/Users/` directory
		2. Create a new user account with the same name
		3. When you click "Create" you will be prompted to use the existing home folder
* User Passwords
	+ Users can change their password themselves
		- `Apple Menu` -> `System Preferences` -> `Security & Privacy` -> `General`
	+ An administrator can reset anyone's passwords
		- `Apple Menu` -> `System Preferences` -> `Users & Groups`
* Reseting the Administrator's Password
	+ If FileVault is not enabled
		1. Boot to Recovery
		2. `Utilities -> Terminal`
		3. `resetpassword`
	+ If FileVault is enabled
		- iCloud password reset
	+ Otherwise
		- Format and reinstall
* Keychains
	+ Encrypted database that stores user passwords for easy/automated recall
	+ Resetting a user's password does not update their keychain
	+ User will be prompted to automatically repair their keychain the first time they login after a password change
	+ A new Keychain will be generated
	+ The old keychain is saved, but will be inaccessible unless the old password can be retrieved
