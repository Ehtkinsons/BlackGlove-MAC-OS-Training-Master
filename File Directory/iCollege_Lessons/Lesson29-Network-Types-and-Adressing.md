## Network Types and Addressing 

### Objectives:

At the end of this episode, I will be able to:

1. Describe the types of networks supported by macOS.
2. Differentiate between IP, TCP, and UDP and describe their uses.
3. Describe IPv6, IPv4, and MAC addresses.

>Additional resources used during the episode can be obtained using the download link on the overview episode.

-----------------------------------------------------------

* Physical Network Connections
	+ Wired Ethernet
	+ Wireless Ethernet
	+ FireWire
	+ Bluetooth
	+ Thunderbolt Bridge
* Logical Protocols
	+ IPv4
	+ IPv6
	+ NetBIOS
	+ PPP
* Transmission Control Protocol (TCP)
	+ Responsible for reliable delivery of data
	+ Disassembles and re-assembles data
	+ Retransmits data if necessary
* Internet Protocol (IP)
	+ Responsible for navigating the network
	+ Defines the start and end point of a communication
	+ Represented as a binary number (base-2)
* IPv4
	+ Uses a 32bit address
	+ 4,294,967,295 Addresses
	+ Represented as a dotted decimal number (base-10)
	+ Example: 192.168.0.1/24
	+ Composed of a network ID and a host ID
	+ Subnet mask defines the separation between the two
* IPv6
	+ Uses a 128bit address
	+ Massive address space
	+ 340,282,366,920,938,463,463,374,607,431,768,211,456 Addresses
	+ Represented as a hexadecimal number (base-16)
	+ Example: 2600:1402:14:197::c77/64
* MAC
	+ Media Access Control
	+ Address assigned to all Ethernet interfaces
	+ For local, non-routable communications
	+ 48bit Hexadecimal number
	+ Example: 3e:15:c2:7c:89:00
	+ First 24 bits are the OUI (Vendor ID)
	+ Remaining 24 bits identify the unique interface
	+ All local communications use MAC address to communicate