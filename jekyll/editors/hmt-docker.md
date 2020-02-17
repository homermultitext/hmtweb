---
title: "Cheat sheet: the HMT Docker container"
layout: page
---


## Start the container

    docker run -ti --name hmt -v $(pwd):/workspace neelsmith/hmteditor

When you're done working, from the bash shell, just `exit`.  (Remember that if you're in an sbt console, you need to quit that first, with `:quit`.)

Exiting the shell stops the container.


## Resuming work


To resume work in a stopped container, first restart the container:

    docker restart hmt

then run a bash sh (`/bin/bash`)  in the restarted container:

    docker exec -ti hmt /bin/bash



## Optional short cuts

In bash, you can put two commands together with `&&`, for example,


    docker restart hmt && docker exec -ti hmt /bin/bash

You can define a short cut, or alias, for those commands in a configuration file (named `.bash_profile` in OS X, or `.bashrc` in Windowsn and Linux).  Here's an example defining a short cut named `dbash`:

    alias dbash='docker restart hmt && docker exec -ti hmt /bin/bash

The next time you start a bash terminal, you can use the command `dbash` instead of the long comand sequence.  If you want to use the alias immediately, run `source .bash_profile` or `source .bashrc`.
