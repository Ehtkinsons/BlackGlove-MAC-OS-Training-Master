## File and Folder Sharing 

### Objectives:

At the end of this episode, I will be able to:

1. Describe file and printer sharing in macOS 11. 
2. Make a folder or printer available for access on a network. 
3. Describe alternative resource sharing protocols supported by macOS. 

>Additional resources used during the episode can be obtained using the download link on the overview episode.

-----------------------------------------------------------

+ Printer Sharing
+ File Sharing
	- Allows sharing files/folders with other users on the network
	- Shared contents are linked to the /Network path
	- Separate links are maintained because share permissions may differ from disk permissions
+ Several different ways
	- SFTP
	- FTP
	- DVD/CD Sharing
+ Two primary connection methods
	1. `Finder -> Go -> Connect to Server`
		+ Mounts shared so it remains accessible
		+ Mounts to the /Volumes folder
		+ Useful for persistent connections
	2. `Finder -> Sidebar -> Shared`
		+ Temporarily connects to a share
		+ Useful for one-off access
+ AppleShare
	- Apple File Protocol (AFP)
	- afp://computer/folder
	- Current version of AFP is 3.4 introduced in 10.8
	- Versions prior to 3.1 can cause issues as they don't support newer features
	- 3.1 was introduced in 10.2
	- File forks
		+ Basis for Time Machine
+ Service Discovery Protocols
	- Detects services on the network (LAN and WAN)
		- File Shares
		- Printers
		- Messages Clients
		- iTunes
		- OS X Server
		- Many more
	- Bonjour
	- Automatic discovery of systems on the network
	- Zero configuration
	- Leverages IPv6 Link Local addresses
	- Leverages Multicast DNS (mDNS) for name lookups
		+ Requests are sent to a multicast address
	- Name format
		+ DonsMacbookPro.local
		+ DonsMacbookPro-2.local
		+ DonsMacbookPro-3.local
	- [More on Bonjour][2]

-----------------------------------------------------------
### External Resources:

During this episode, you can reference the following external resources for supplementary tools and information:

- 
[1]:https://www.apple.com/remotedesktop/
[2]:https://developer.apple.com/library/ios/documentation/Cocoa/Conceptual/NetServices/Articles/about.html
