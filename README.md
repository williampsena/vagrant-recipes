# Intro

This repository contains Vagrant machine examples.

# Requirements

- Virtualbox

# Virtualbox settings

To allow virtual to assign IP addresses, create a file called `/etc/vbox/networks.conf`. In the example below, we set a range of `192.168.0.0/16`.

```bash
sudo mkdir -p /etc/vbox
echo "* 192.168.0.0/16" | sudo tee -a /etc/vbox/networks.conf
```

# Time to up virtual machines

```bash
(cd hello-vagrant/ && vagrant up)
```