---
layout: page
title: Installing the HMT VM
---

## Prerequisites

- [git](../install-git)
- [vagrant](https://www.vagrantup.com/)
- [virtual box](https://www.virtualbox.org/)
- a minimum of about 5Gb of free disk space on the host computer


## Installation ##


1. Open a terminal session.
2. Change directories to where you want to install the virtual machine (e.g. to go to your desktop enter the following: `cd Desktop`)
3. Clone the `editor` repository at <https://github.com/homermultitext/editors-vm>. Copy the clone URL and enter the command:   ` git clone https://github.com/homermultitext/editors-vm.git`
4. Change directories to the VM (`cd editors-vm`).
5. Run the command: `vagrant up` (This will start the virtual machine, and the first time you do it, it will build the VM from scratch).
6. Find something to occupy yourself for awhile. It is a lengthy process, especially if multiple people are using the same network to build a vm. Make sure you have a good internet connection and don't forget you're building a machine and do something silly like shut your laptop. It has happened.  Wait until
7. A login screen will appear before the VM has finished building. Don't attempt to login yet, however: wait until you see your bash shell prompt in the terminal
8. Now use the new window to log in to the virtual machine.  The username and password are both `vagrant`.
9. You're now ready to configure the Atom editor: in the VM, open a terminal, and run `atom-config.sh`
8. When you are done working in the virtual machine, you can log out.
9. Back in your terminal window you need to run the command: `vagrant halt`. This shuts down the machine. You will want to remember to do this because otherwise the machine will keep running and draining your battery.


For more details and troubleshooting tips, see the instructions at <http://homermultitext.github.io/hmt-docs/vm/>.
