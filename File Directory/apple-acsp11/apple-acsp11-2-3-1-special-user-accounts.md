## Special User Accounts 

### Objectives:

At the end of this episode, I will be able to:

1. Identify special and hidden user accounts in macOS. 
2. Describe the purpose of the "Guest" user account. 
3. Describe the purpose of the "root" user account.

>Additional resources used during the episode can be obtained using the download link on the overview episode.

-----------------------------------------------------------

* Special User Accounts
	- Accounts created by macOS for a specific purpose
	- Typically hidden and not used
	- Examples
		+ Root user
		+ Guest account
* Guest Account
	- Disabled by default
	- Used to provide anonymous access to resources
	- Anyone with physical access to the system could logon
* Disabling the guest account
	- Safe
	- Breaks "Find My Mac" without a cell adapter
* Root Account
	- The primary administrator account created in all Unix systems
	- Enabled by default, but logons are disabled
	- Cannot be deleted
	- Logons can be enabled by assigned a new password to the account, but it is not advised
	- "Root" is a well-known account name and is used in most brute-force attacks
* Disabling the root account
	- Can be done, but breaks numerous things
	- Change the password if desired2
		+ `sudo passwd root`
