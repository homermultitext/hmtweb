---
layout: page
title: Installing a bash shell
---


## For Mac users ##

The `bash` shell is already installed on OS X and Linux systems.

To use the `bash` shell in OS X, open the **Terminal** application (in the Utilities folder inside the Applications folder).

## For Windows users: `gitbash` ##


To install a bash shell:

- go to <https://msysgit.github.io/>
- click on **Download** and follow the installation process
- set the `Path` environmental variable as follows:
     - open your Control Panel
     - search for **variables**
     - click on **Environmental Variables**
     - select the `Path` variable, and click on **Edit**
     - add `\bin`` to the end of the variable
     - hit **Save** and **OK**

 
To test your shell, open the gitbash terminal, and type `git help`.  If you see a long help message, everything is configured correctly.
