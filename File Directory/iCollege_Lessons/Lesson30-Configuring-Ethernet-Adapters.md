## Configuring Ethernet Adapters 

### Objectives:

At the end of this episode, I will be able to:

1. Manually configure a network adapter in macOS.
2. Configure and verify Dynamic Host Configuration Protocol (DHCP).
3. Configure and verify a Domain Name System (DNS) Server.

>Additional resources used during the episode can be obtained using the download link on the overview episode.

-----------------------------------------------------------

* Obtaining an address
	- IPv4
		+ Static IP
		+ DHCP
	- IPv6
		+ Static IP
		+ Link-local IP
		+ Stateless Auto-configuration
		+ DHCPv6
* It varies based on local vs remote systems 
* Local Communication
	1. DNS is used to resolve the IP of the destination
	2. The IP is compared against our address/subnet mask and determined to be on the same network
	3. An Address Resolution Protocol (ARP) broadcast is sent out to locate the destination system
	4. The ARP response teaches us the MAC address associated with the destination IP
	5. We then communicate with the destination using the MAC address
* Remote Communication
	1. DNS is used to resolve the IP of the destination
	2. The IP is compared against our address/subnet mask and determined to be on a different network
	3. An Address Resolution Protocol (ARP) broadcast is sent out to locate the router
	4. The ARP response teaches us the MAC address associated with the router
	5. We then communicate with the router using its MAC combined with the IP address of the destination system
	6. The router receives the data and recognizes that the router is not the final destination
	7. The router forwards the traffic along to the next router in line
* Domain Name System
	+ Resolves a name to an IP
	+ Example #1: www.apple.com = 23.78.138.214
	+ Example #2: www.apple.com = 2600:1402:14:197::c77
	+ `nslookup www.apple.com`
	+ `dig www.apple.com`
* Three primary components
	1. Service
		- Network software that supports communications
		- DHCP, DNS, Web Server, etc.
	2. Interface
		- Physical network connection
		- Ethernet, Wi-Fi, etc
	3. Protocol
		- Logical network connection
		- TCP/IP
* Basic Steps
	1. `Apple Menu -> System Preferences -> Network`
	2. Select appropriate interface
	3. Assign address, or select DHCP
	4. Select `Apply`
* Advanced configurations
	- Most adapters have an *Advanced* button
	- Used to assign less common settings
	- TCP/IP
		+ DHCP Client ID
		+ IPv6
	- DNS
		+ Additional DNS Servers
		+ Search Domains
	- WINS
		+ WINS servers
		+ Workgroup Name
	- 802.1x
		+ Enable Automatic Configuration
		+ Select a profile
	- Proxies
		+ Assign various proxies
		+ Define addresses that bypass the proxy
	- Hardware
		+ MAC address
		+ Speed
		+ Duplex
		+ MTU