## Configuring WiFi Adapters 

### Objectives:

At the end of this episode, I will be able to:

1. Differentiate between configuration options for physical and wireless network adapters.
2. Describe Wi-Fi security options and their appropriate use.

>Additional resources used during the episode can be obtained using the download link on the overview episode.

-----------------------------------------------------------

* Wi-Fi Network Settings
	+ Enable Wi-Fi
		- `System Preferences -> Network -> Interface -> Turn Wi-Fi On`
		- Wireless icon in menu bar
	+ OS X will automatically connect to non-secure networks
		- At power on
		- At resume
		- Can be disabled using the *Ask to Join New Networks*
		  option in the system preferences
	+ Secure networks require authentication
		- Prompted to enter credentials
* Credentials can be a pre-shared key (PSK or password)
	+ Password is stored in the user's keychain
	+ Not shared between users on the system
* Credentials can be certificate based
	+ 802.1x
	+ WPA Enterprise and WPA2 Enterprise
	+ Certificates are stored in the system keychain 
	+ Available to all users
* SSID
	+ Service Set Identifier
	+ Name that identifies a wireless network
	+ Typically broadcast out every few seconds
	+ Can be hidden
	+ If hidden, you must manually type the SSID name by using the *Join Other Network* option
* Ad Hoc Networks
	+ Wireless network built between two Macs
	+ Use the *Create Network* option in the menu bar