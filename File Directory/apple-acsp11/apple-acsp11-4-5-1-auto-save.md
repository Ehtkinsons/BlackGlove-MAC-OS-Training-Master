## Auto Save 

### Objectives:

At the end of this episode, I will be able to:

1. Describe the function and purpose of macOS Auto Save.
2. Configure Auto Save to save application data and window information.
3. Revert a document to its previous version using Auto Save. 

>Additional resources used during the episode can be obtained using the download link on the overview episode.

-----------------------------------------------------------

* Auto Save
	+ Feature built-in to macOS
	+ Automatically saves a user's work
	+ Maintains file revisions also
* Application Support
	+ Requires the app developer to support Apple's Auto Save extension
  	+ Easy test
  		- `File -> Duplicate/Rename/Move To/Revert To`
  	+ If those options are present, auto save is supported
* Disabling Auto Save
	+ `System Preferences -> General -> Ask to keep changes when closing documents`
	+ Enabled = No auto save
	+ Disabled = Auto save
* Application Resuming with Auto Save
	+ Normally when you close an application, all of its associated windows close also
	+ Upon re-opening an application, no windows are open
	+ The *Resume* features allows previous windows to automatically re-open with the app
	+ Auto save makes this possible
	+ Can be toggled
	+ `System Preferences -> General -> Close windows when quitting an app`
		- Disabled = Re-open windows when launching the app
		- Enabled = New window when launching the app
