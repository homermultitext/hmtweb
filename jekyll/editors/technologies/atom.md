---
layout: page
title:  Atom
---


## Overview

Atom is "a hackable text editor."  People have written plugins for Atom to do just about anything you can think of (and probably more).  We use it for editing many kinds of documents, incuding

-   tabular text data
-   prose written in Markdown
-   scripts in Scala
-   TEI XML documents

## Installation

Download and install Atom:  <https://atom.io/>.  If you are on OS X, open Atom and choose from the Atom menu, "Install Shell Commands".

From a bash shell, use the atom package manager `apm` to install several packages that will be useful in your editing work.  You can copy and paste the following commands directly in a bash shell:


    apm install intentions
    apm install busy-signal
    apm install linter
    apm install linter-ui-default
    apm install linter-autocomplete-jing
    apm install atom-xsltransform
    apm install xml-formatter
    apm install rainbow-csv
    apm install atom-wrap-in-tag
    apm install https://github.com/mfripp/atom-tablr.git
