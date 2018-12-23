---
title: Removing the wrong git on  Mac OS X 10.7.5
layout: page
---


If you accidentally install the wrong version of git on Mac OS X 10.7.5, you'll need to remove it before you
can install the correct version.  You need to uninstall git if you have problems like the description on [this page](http://stackoverflow.com/questions/23448318/git-segmentation-fault-11), 

- Open the disk-image from which you originally installed Git. It will have a name like "Git Install…".
- In the terminal, type `cd /Volumes/Git<TAB>` to navigate to that disk-image.
- Type `./uninstall.sh`, type "yes" when it asked, then your password.
- Confirm that you have uninstalled Git by typing `which git` in the Terminal. There should be no answer.

Then install following the [instructions for installing git](../../install-git).


