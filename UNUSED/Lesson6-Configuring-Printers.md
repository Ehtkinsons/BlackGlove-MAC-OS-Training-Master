## Configuring Printers 

### Objectives:

At the end of this episode, I will be able to:

1. Describe the Common Unix Printing System (CUPS).
2. Install a printer in macOS and verify functionality.
3. Share a printer on the network to make it available to other machines. 

>Additional resources used during the episode can be obtained using the download link on the overview episode.

-----------------------------------------------------------

+ Printers can be added by two methods
	1. Manually connecting the printer and installing drivers (if required)
	2. Automatically discovering the printer
+ Common Unix Printing System (CUPS)
	- The foundation of printing in most Unix-based OSes
	- Owned by Apple, but an open-source project
	- Uses PPD files for printer drivers
		+ PostScript Printer Description (PPD)
		+ Apple provides native drivers for many printers
			- `/System/Library/Printers`
		+ Most vendors provide PPD files for their printers as it enables both MacOS as well as Linux
		  	- `/Library/Printers`
	- When printing, your document is pre-processed and stored in `/var/spool/cups`
	- The spool folder is protected to ensure users cannot access each other's print jobs
+ A printer on your machine can be shared to other systems on the network
	1. `System Preferences -> Printers & Scanners`
	2. Select the printer
	3. Select *Share this printer on the network*
+ Printer Preferences
	1. `System Preferences -> Sharing`
	2. Select *Printer Sharing*
	3. Select the printer
	4. Assign desired permissions
