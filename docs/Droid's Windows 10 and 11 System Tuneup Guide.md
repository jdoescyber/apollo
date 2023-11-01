---
title: Droid's Windows 10 and 11 System Tuneup Guide
---
Over the past year I've gotten requests for this information a few times. I intend to update this over time. 😊

## Disabling Startup Items

Lowering the amount of applications starting at system boot (or logon) will improve system startup time. It will also lower the amount of resource utilization by applications that you aren't actively using, but get started every time you turn on your machine.

1. Right-click the task bar and choose "Task Manager" or press `CTRL` + `ALT` + `DEL` and then select "Task Manager."
2. Navigate to the "Startup" tab.
3. Sort the items by "Status" to show the items that are startup-enabled on the top.
4. Check the list for anything you don't regularly use. Common things to disable include, but are not limited to:
	1. Bluetooth controller apps
	2. Auto-update applications
	3. RGB applications and peripheral management apps (like Logitech G, Corsair VUE, HyperX NGenuity)
5. It may help to look at the "Startup Impact" tab to target high-impact items.
6. I recommend **AGAINST** disabling things like:
	1. Your audio drivers/audio services (e.g. `Waves MaxxAudio Service` in the below screenshot)
7. Restart your PC and check that everything is working as expected.

<figure markdown>

	![Startup Items](https://i.imgur.com/U1TlvK8.png)
	<figcaption> Navigate to the "Startup" Tab and Sort </figcaption>
</figure>
## System "Sweeping"

This section will accomplish what was originally 5+ sections of this guide. We'll be using a free ([and open source](https://github.com/bleachbit/bleachbit)) application to delete junk and temporary files from the file system.

Navigate to [Bleachbit's Website](https://www.bleachbit.org/download/windows) and download whichever edition you prefer. If you aren't sure, the `installer .exe` file will likely be best for you. Install the application as you normally would any other, and then run Bleachbit **as an administrator**. It usually takes around 15-20 seconds to open because it's doing some system application discovery and calculations in the background.

Clicking an option on the left will provide you with a brief description on the right.

!!! note

	The listed applications on the left-side pane will vary by person to person. Bleachbit supports many applications, but only displays them in the list if you have a given program installed. For example, you may **not** have Firefox installed, so you **wouldn't** see Firefox listed.  Likewise, you may have applications listed that I don't have.

!!! warning

	Any selection that includes "cookies" is likely to log you out of that application. That's normal and expected. Refreshing cookies (used for authentication, among other things) on occasion isn't harmful by any stretch.

 Below are some that I would recommend everyone clean, along with some more specifics for applications I have.

- Deep Scan
	- Backup Files
	- Temporary Files
	- Thumbs.db
- Discord
	- Everything
- Firefox
	- Cache
	- Cookies
	- Crash Reports
	- DOM Storage
	- Form History
	- Passwords (please don't store your passwords in a browser)
		- If you do have passwords stored, this operation will DELETE them.
	- Session Restore
	- Vacuum
- Google Chrome
	- Cache
	- Cookies
	- DOM Storage
	- Form History
	- Passwords
	- Vacuum
- Internet Explorer
	- Everything
	- Please switch to a modern browser (Edge, Chrome, Firefox). Internet Explorer is incredibly insecure.
- Microsoft Edge
	- Cache
	- Cookies
	- DOM Storage
	- Form History
	- Passwords
	- Vacuum
- Microsoft Office
	- Debug Logs
- System
	- Clipboard
	- Logs
	- Memory Dump
	- MUICache
	- Prefetch
		- Prefetch helps applications load faster, so they'll be slower for about 10 seconds when you open them for the **FIRST** time after clearing prefetch.
	- Recycle Bin
		- Check that you don't need anything in there.
	- Temporary Files
	- Update Uninstallers
- Windows Defender
	- Temporary Files
- Windows Explorer
	- Most Recently Used
	- Recent Documents List
	- Run
	- Search History
	- Shellbags
	- Thumbnails
