---
title:  How to resume an interrupted Vagrant install
layout: page
---




If your host computer goes to sleep during the Vagrant install and the install process hangs, first:

- Type `control-C` to kill the installation process.
- Remove any temporary files that Vagrant tried to download:
	- Type: `cd ~/.vagrant.d/tmp`. This navigates to the directory where Vagrant puts its temprary files.
	- Type: `open .`. (`open` followed by a space and a period character). This means "Open the directory I am currently in." This should open a "tmp" directory in your Finder (on a Mac) or the "My Computer" thing in Windows.
	- Delete any files in that folder.
- Navigate back to your `vm2015` directory. *E.g.* `cd ~/Desktop/vm2015`.
- Type `vagrant up` to restart the installation process.


