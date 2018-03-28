---
layout: post
title: Postgres DigitalOcean Basic Setup
description: This is a quick run through on setting up postgres in Digital Ocean
image: assets/images/pic01.jpg
---



apt-get update
apt-get upgrade
apt-get install postgres postgres-contrib

Assume the identity of postgres
sudo -i -u postgres

Create a user role for postgres, interactively 
sudo -u postgres create user --interactive

sudo -u postgres createdb cloudcowboy

sudo adduser cloudcowboy



sudo -i -u cloudcowboy
psql
