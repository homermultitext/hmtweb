---
layout: page
title: Installing Virtual Box and Vagrant
---

## Virtual Box ##

1. Go to the following [link](https://www.virtualbox.org/wiki/Downloads).
2. Select the appropriate download for your operating system (Mac, Windows, Linux, etc...)

## Vagrant ##

1. Go to the following [link](https://www.vagrantup.com/downloads.html).
2. Select the appropriate download for your operating system (Mac, Windows, Linux, etc...)

## Testing your Installation ##

1. On your desktop (or another convenient location) create a new empty folder. You can name it something obvious like "test."
2. Open a bash shell.
3. Change directories to the new test folder you created.

  cd desktop/test
  
4. Enter the following two commands in your bash shell:

  vagrant init hashicorp/precise64
  
  vagrant up

These two commands will first download a very basic 64-bit virtual machine and then attempt to build it. If they run successfully, then you know that you have correctly installed your virtual machine software. If they do not run successfully, you should reinstalled Virtual Box and Vagrant and try again.


## Trouble shooting: how to Resume an Interrupted Vagrant Install

If your laptop goes to sleep while doing the Vagrant install, it might not be able to resume when the computer wakes up. Do this:

- Type `control-C` to kill the installation process.
- Remove any temporary files that Vagrant tried to download:
	- Type: `cd ~/.vagrant.d/tmp`. This navigates to the directory where Vagrant puts its temprary files.
	- Type: `open .`. (`open` followed by a space and a period character). This means "Open the directory I am currently in." This should open a "tmp" directory in your Finder (on a Mac) or the "My Computer" thing in Windows.
	- Delete any files in that folder.
- Navigate back to your `vm2015` directory. *E.g.* `cd ~/Desktop/vm2015`.
- Type `vagrant up` to restart the installation process.