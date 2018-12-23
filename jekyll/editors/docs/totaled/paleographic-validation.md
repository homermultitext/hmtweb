---
title:  Validating paleographic observations
layout: page
---

From within your VM:

1. open a terminal
2. `cd /vagrant/YOURREPO` (note that YOURREPO will vary depending on the name of your repository).
5. Run the command `sh scripts/palview.sh`. Alternatively you can copy the script from your repository and paste it in the `scripts` folder in your shared repository. If you have more than one editing repository in your VM, it is recommended you rename it something obvious. You can then just run that file name in the terminal from anywhere.
6. After the build is complete open `hmt-mom/build/paleography/viewer.html` which can be found in your `shared` folder.
7. Review the results to make sure you are happy with the images and that the letters do correspond properly. Adjust as needed.
