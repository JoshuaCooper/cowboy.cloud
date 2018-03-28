---
layout: post
title: Linux guest shared folder 
description: Sharing files with a guest linux box
image: assets/images/pic04.jpg
---

You will need to have guest additions fully installed on the guest and have a folder shared with the guest 
sudo usermod -a -G vboxsf cloudcowboy
sudo mount -t vboxsf -o ShareName NewFolder
