---
layout: post
title: dotnet Ubuntu Setup
description: Setting up a dotnet environment on Ubunto 16.04
image: assets/images/pic13.jpg
---



A quick guide to setting up a dotnet build environment on Ubuntu 16.04

Step 1: Ensure your ranch is ready.
<pre>
sudo apt-get update
sudo apt-get upgrade 
</pre>
Step 2: Add the proper keys and sources for Microsoft.
<pre>
sudo apt-get install apt-transport-https
curl https://packages.microsoft.com/keys/microsoft.asc | gpg --deamor > microsoft.gpg
sudo mv microsoft.gpg /etc/apt/trusted.gpg.d/
sudo sh -c 'echo "deb [arch=amd64] https://packages.microsoft.com/repos/microsoft-ubuntu-xenial-prod xenial main" > /etc/apt/sources.list.d/dotnetdev.list'
sudo apt-get update
</pre>
Step 3: Ensure https transport is installed and then install the dotnet application.
<pre>
sudo apt-get install apt-transport-https
sudo apt-get install dotnet-sdk-2.1.101
</pre>

