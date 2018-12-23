---
layout: page
title: Fixing files with BOM
---

Woops! You edited a file with XML Copy Editor, but missed this note about [how to make it safe to use](../xmlcopyeditor).  Now when you try to validate, you're getting mysterious messages about "Content not allowed in prolog," and your terminal looks something like this:

![sad news](../imgs/bom-bomb.png)


The fix is easy:

1. `cd` to the directory with your edited file (something like `cd /vagrant/YOUR_REPOS/editions/Iliad` or `cd /vagrant/YOUR_REPOS/editions/scholia`).
2. Fix the file with this command `bomstrip-files FILE_NAME` (where `FILE_NAME` might be something like `VenetusA-Iliad.xml` or `MainScholia.xml`).
3. Make sure you check the configuration of XML Copy Editor following [these instructions](../xmlcopyeditor).

