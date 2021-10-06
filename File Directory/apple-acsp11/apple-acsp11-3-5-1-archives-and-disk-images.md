## Archives and Disk Images 

### Objectives:

At the end of this episode, I will be able to:

1. Differentiate between archives and disk images.
2. Create disk images using the Disk Utility. 
3. Compress and decompress archives using the macOS finder. 

>Additional resources used during the episode can be obtained using the download link on the overview episode.

-----------------------------------------------------------

* macOS Archive Support
	+ macOS has native support for zip archives
	+ Combines multiple files into one file
	+ Compresses the over-all size of the files
	+ Typically named `*.zip`
	+ Decompression: 
		1. Double-click on the archive
* Compression: 
	1. Highlight desired files
	2. `Ctrl-Click -> Compress <#> Items`
	3. Rename archive file as desired
* Images
	+ File Images
	+ Similar to an archive except that compression is not normally performed
	+ Functions like a virtual hard drive
	+ Typically named `*.dmg`
	+ Like a hard drive, an image file has a set size regardless of how much data is stored inside of it
		- A special type of image called a *Sparse Disk* image can be created which will not consume empty space
* Mounting Images
	+ Disk images must be mounted
	+ Double-click the image or us Disk Utility
* Creating Images
	1. Launch `Disk Utility`
	2. Click `New Image`
	3. Fill out desired options
		+ Name
		+ Size
		+ Format
		+ Encryption
		+ Partitions
		+ Image format
			- Choose sparse disk if desired