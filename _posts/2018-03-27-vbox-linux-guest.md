---
layout: post
title: Ubuntu 16.04 Addons Setup
description: Configuring and installing guest additions to a linux guest
image: assets/images/pic04.jpg
---

sudo su 
mount /dev/cdrom /media/cdrom -o loop 
cd /media/cdrom.
apt-get install -y dkms build-essential linux-headers-generic linux-headers-$(uname -r).
./VBoxLinuxAdditions.run.
reboot




