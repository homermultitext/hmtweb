---
title:  Installing the HMT VM
layout: page
---






## Prerequisites ##

The HMT VM uses Vagrant to define a virtual machine you can run with  VirtualBox.  In addition to the [general technical prerequisites](http://homermultitext.github.io/hmt-docs/tech/) for the HMT project therefore, the two specific prerequisites for running the VM are:

- [Vagrant](https://www.vagrantup.com/)
- [VirtualBox](https://www.virtualbox.org/)


## Getting started ##

In the course of building the VM, your computer will download a load of material, so make sure you have a good internet connection.  Start by opening a terminal session, and change directories to where you want to install the virtual machine (e.g. to go to your desktop: `cd Desktop`).

The  github repository for the VM is <https://github.com/homermultitext/editors-vm.git>.  Clone it with the normal git command:

    git clone https://github.com/homermultitext/editors-vm.git

Change directories to the newly cloned VM (`cd editors-vm`), and from within the `editors-vm` directory, run

    vagrant up

> Your machine must be able to run a 64-bit VM.  Some computers have BIOS settings that prohibit this.  If that happens, you will have to change your BIOS settings to allow the 64-bit VM to run.  Here is [some help](../bios).


This is the routine command to start the virtual machine: since this is first time you have run it, vagrant will proceed to build the VM from scratch.

Find something to occupy yourself for awhile, but don't let your computer go to sleep before the build has completely finished:  vagrant is not always able to resume cleanly if the process is interrupted.  (Don’t forget and do something silly like shut your laptop. It has happened.)

A new window with a login screen will eventually pop up.  Don't log in until the entire build process has completed in your original terminal session on your host computer, however.

When the build is complete, log in to the VM from the new window. The username and password are both `vagrant`.  When you have logged in, your desktop should include a dock that looks like this:


![dock](../imgs/yourdock.png)

The items on the dock are (from left to right):

6.  System Settings
8.  a terminal running the bash shell
1.  a link to the shared folder where you will keep all your work
3.  Atom, a text editor you can use for writing markdown and other text


At this point, if you'd like to install a Greek keyboard layout or additional keyboard layouts, follow [these instructions](../keyboard).

To be sure all the automatically installed configurations have taken effect, logout of your account, and then log back in.  You can logout from the "power sign" menu at the time right of your screen:


![logout](../imgs/logout.png)


## Installing the HMT editorial system ##



First, we'll configure your editor (Atom) to help you with the different kinds of content we edit (XML files, delimited-text files, texts in markdown, and even scripts in Scala).



Open a terminal to run your familiar bash shell, and run

    atom-config.sh




When you are done , you can shut down the virtual machine from your original terminal session on your host computer by running

    vagrant halt

You will want to remember to do this because otherwise the machine will keep running and draining your battery.


## Trouble shooting ##


If your host machine goes to sleep before Vagrant finishes the initial installation, it might not be able to resume building without a little help.  Follow [these steps](../resume-vagrant-up) to complete your install.
