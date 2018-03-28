---
layout: post
title: Linux guest shared folder 
description: Sharing files with a guest linux box
image: assets/images/pic04.jpg
---

You will need to have guest additions fully installed on the guest and have a folder shared with the guest see [Vbox linx guest additions](/2018/03/27/vbox-linux-guest.html).

It easier to add your user to the vboxsf group.
<pre>
sudo usermod -a -G vboxsf cloudcowboy
</pre>
Mount the share to the mount point you desire.
<pre>
sudo mount -t vboxsf -o sharename mountpoint
</pre>
