## Network Locations 

### Objectives:

At the end of this episode, I will be able to:

1. Describe network locations and their intended use. 
2. Configure network locations to support configurations for multiple networks. 

>Additional resources used during the episode can be obtained using the download link on the overview episode.

-----------------------------------------------------------

* Different settings can be defined based on the type of network you are connected to
* Types: 
	- Automatic
		+ All network services/interfaces are attached to this location by default
		+ Not automatically configured
		+ Automatically initialized at boot or resume
	- Self Defined
		+ Custom locations we have created
		+ Each location can have different adapter settings
		+ Example: Static IP at work, DHCP at home
		+ `System Preferences -> Network -> Location Drop-down -> Edit Locations`
* To switch locations
	- `Apple Menu -> Location -> <Location>`
	- Must hit *Apply* if you just edited locations
* Virtual Private Network
	- Encrypted tunnel between your computer and another system
	- Creates the equivalent of a private network between you and them
	- Not really a network in itself
* Supported Types
	- L2TP over IPSec
	- PPTP
	- Cisco IPSec
* To configure
	- `System Preferences -> Network -> + -> VPN`