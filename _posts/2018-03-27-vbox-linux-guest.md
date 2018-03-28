---
layout: post
title: Ubuntu 16.04 Addons Setup
description: Configuring and installing guest additions to a linux guest
image: assets/images/pic12.jpg
---

Well cowpoke, I seem to always forget the steps required wrangling up an Ubuntu VM in the proper way on VirtualBox. This should get you going from a fresh install to a loaded wagon. Ford the river and keep coding.

<pre>
sudo su 
mount /dev/cdrom /media/cdrom -o loop 
cd /media/cdrom.
apt-get install -y dkms build-essential linux-headers-generic linux-headers-$(uname -r).
./VBoxLinuxAdditions.run.
reboot
</pre>

This has been tested on Ubuntu 16.04 but should work on their next release due out in 2018.04 Bionic Beaver.

Photo generously provided by:
https://www.flickr.com/photos/lsmith2010/
