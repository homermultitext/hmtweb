---
layout: page
title: Setting up Atom for XML editing
---

Once you have [installed Atom](../atom), you need to link a plugin that will validate your XML against the guidelines of the Text Encoding Initiative (TEI).



1.  Clone or download the `atomic-tei` github repository at <https://github.com/neelsmith/atomic-tei>
2.  In a bash shell, `cd` into the cloned/downloaded repository, and run `apm link`


That's it. Note that if you later decide to move the `atom-tei` directory somewhere else, you'll need to rerun `apm link` from the new location.
