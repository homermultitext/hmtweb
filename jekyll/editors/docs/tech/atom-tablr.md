---
layout: page
title: Setting up Atom for editing tables
---

Once you have [installed Atom](../atom), you need to install a configuration file for the `tablr` plugin.

-   Download the file `atom-tablr-conf.cson` [here](https://raw.githubusercontent.com/homermultitext/editors-vm/summer2017/system/atom-tablr-conf.cson).
-   Find it on your computer.  (Note that some browsers might "helpfully" rename the file by adding an additional extension such as `.txt`  Why?)


You need to make a copy of this file in a hidden folder named `.atom`.  The copy should be named `config.cson`.

One way to do this is to open a bash shell in the same directory as the downloaded file, and use the `cp` command to copy it, like this:

    cp atom-tablr-conf.cson $HOME/.atom/config.cson
