## Hidden Files 

### Objectives:

At the end of this episode, I will be able to:

1. Describe the function of hidden files and folders in macOS.
2. Utilize chflags and the hidden flag to hide a file or folder.
3. Utilize UNIX-style hidden files and folders. 
4. Navigate to hidden resources in the macOS file system. 

>Additional resources used during the episode can be obtained using the download link on the overview episode.

-----------------------------------------------------------

* Hidden System Folders
	+ Many files/folders are hidden from the end users
	+ Not needed by the average user
	+ Hidden for convenience and protection
	+ Example
		- Each user has a `Library` folder
		- `/User/dpezet/Library`
		- Contains user settings and system data
		- Hidden by default
* Using the *hidden* flag
	- `chflags hidden ~/file.txt`
	- `chflags nohidden ~/file.txt`
	- Hidden from Finder only
* Hiding a folder
	- `chflags hidden /User/dpezet/Test`
* UNIX-style hidden files and folders
	- File name is preceded with a `.`
	- e.g. `/User/dpezet/.ssh/`
	- Hidden from Finder and Terminal
* Accessing Hidden folders
	- Some are listed in Finder `Go` menu
		+ Hold `Option` to see `Library` in the menu
	- Otherwise, `Go -> Go to Other Folder` and manually type path
* Hidden Root Folders
	+ For most users, their file system rotates around their home directory
	+ There are numerous hidden system folders also
	+ `ls -la /`
