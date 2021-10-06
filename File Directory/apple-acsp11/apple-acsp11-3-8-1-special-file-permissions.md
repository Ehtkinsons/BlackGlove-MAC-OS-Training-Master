## Special File Permissions 

### Objectives:

At the end of this episode, I will be able to:

1. View and modify UNIX-style permissions from the terminal. 
2. View and modify macOS ACL permissions from the terminal. 
3. Describe the metadata and the AppleDouble metadata file structure. 

>Additional resources used during the episode can be obtained using the download link on the overview episode.

-----------------------------------------------------------

* List permissions
	+ `ls -l <directory>`
* Modifying Permissions
	- Modify permissions: `chmod <permissions> <directory>`
	- Example #1
		+ `chmod g+w ./file.txt`
		+ Adds write permissions to the group
	- Example #2
		+ `chmod go-r ./file.txt`
		+ Removes read permissions from group and other
	- Example #3
		+ `chmod -R go+r ./tmp`
		+ Adds read access for group and other for ./tmp and all files/folders within it
		+ Recursive
	- Example #4
		+ `chmod u=rwx,go=rx ./script.sh`
		+ Grants read/write/execute permissions to the file owner
		+ Grants read/execute permissions to the group and everyone else
	- Example #5
		+ `chmod +r ./file.txt`
		+ Grants read permissions to everyone for the file
* Changing the owner/group
	- `chown <owner>:<group> file.txt`
	- `chown donpezet:admin secret.txt`
	- To modify a folder and all child objects, use -R
	- `chown -R donpezet:staff /Users/donpezet/Music`
* Access Control Lists
	+ View extended permissions (ACLs)
		- `ls -le`
	+ Add permissions
		- `chmod +a "username allow read,write" file.txt`
	+ Remove permissions
		- `chmod -a "username allow read,write" file.txt`
* File Metadata
	- Additional information about a file
	- Some file formats can store it internally
		+ PDF
		+ MP3
		+ MP4
		+ PNG
		+ GIF
	- Apple can store the metadata externally also
	- Spotlight searches are able to find files based on 
	  metadata
	- Use *Get Info* on a file to view its metadata
	- For files stored on a Mac OS Extended Volume the 
	  metadata is stored in extended file attributes
	- Use `ls -l@` in the terminal to view them
* AppleDouble Metadata
	- For files stored on FAT/ExFAT Volumes, the metadata is stored in a separate file.
	- Separate file is referred to as AppleDouble Metadata
	- Example

| Original File Name | Metadata File Name |
|--------------------|--------------------|
| File1.txt          | ._File1.txt        |
| Instrucions.pdf    | ._Instructions.pdf |