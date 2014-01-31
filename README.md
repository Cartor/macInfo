OSXey
===============

A script for OS X to display system information

!['Screenshot'](https://raw.github.com/Gary00/OSXey/master/screenshot_normal.png)
!['Screenshot'](https://raw.github.com/Gary00/OSXey/master/screenshot_color.png)


Install / Uninstall
------------
Use 'install.sh` to both install and uninstall.


Options
------------
	-c,  --color
		Color Logo	


Configuration
------------
 	$ sudo nano /usr/local/bin/OSXey

Change the value of the variable color, to change the color text. The options listed under #Colors

	color=$(tput setaf $lightblue)

Recent Changes
--------------

* Added install script.
* Now truncates long hostnames that are > 35 characters.
* Now displays names of Operating System next to version. For example, "Version: OS X 10.9 Mavericks" (Bash 3 & Bash 4)


To-Do List
------------

* Test Package Manager with macports
* Look into $terminalText bug. Maybe find a better way of displaying colors then current method.
* Look into logo allignment in code (match what is dispalyed)
* Code cleanup
* Smarter install script (create directory if doesn't exist, prompt if already uninstalled)
* Look into being able to install via package manager (homebrew / macports)
* Look up model identifier (e.g imac,12,2) and note which mac is in use