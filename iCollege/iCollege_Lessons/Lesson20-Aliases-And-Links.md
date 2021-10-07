## Aliases and Links 

### Objectives:

At the end of this episode, I will be able to:

1. Create and modify file system aliases in macOS. 
2. Describe and create UNIX-style hard links and symbolic links. 

>Additional resources used during the episode can be obtained using the download link on the overview episode.

-----------------------------------------------------------

* Aliases
	+ Aliases are pointers that indicate the location of a file
	+ Consume less space than a second copy of the file
		- Links are around 300Kb
		- Can be larger than a text document
	+ Created by:
		- `Option-Click` on a file and choose `Make Alias`
		- `Command-L`
	+ DEMO: Creating an alias
	+ Will continue to point to the original even if it has been renamed or moved.
	+ Aliases are not recognized by the file system
	+ DEMO: Moving the source file
* UNIX-style Links
	+ The BSD Unix system has native support for links
	+ Mac GUI will follow them, but not create them
	+ Two types
		1. Symbolic Links
		2. Hard Links
* Symbolic Links
	- Filesystem pointer to another file
	- Does not track the file
	- Moving the original breaks the symlink
	- `ln -s <target> <link>`
	- `ln -s /Volumes/USB\ HD /Users/donpezet/Documents/USB\ HD`
* Hard Links
	- An additional filesystem entry that points to existing data
	- Will survive the original being renamed/moved
	- Not typically used with directories
	- `ln <target> <link>`
	- `ln ~/Documents/file.txt ~/Desktop/file.txt`
