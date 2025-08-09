# Hardware

## Homelab

My home cluster uses four older laptops as nodes for the cluster. 

- Lenovo ThinkPad X1 Carbon, 6th Gen (2018)
- Lenovo ThinkPad X1 Carbon, 7th Gen (2019)
- Asus Zephyrus G14 (2021)

- SSD Replacement Needed: Dell XPS 15, 9560 (2017) 

I removed the batteries from the machines and bought corresponding ethernet adapters to connect them all to a TP-Link Gigabit switch. All machines are running Fedora 42 Server. The lid behavior was modified to modify the flags in `/usr/lib/systemd/logind.conf` to change `HandleLidSwitch=ignore, HandleLidSwitchExternalPower=ignore, HandleLidSwitchDocked=ignore`.

The G14 in particular has a couple of quirks:
- It uses asusctl for managing profiles - by default, it's set to quiet
- There's an Nvidia RTX 3060 mobile, but it only has access to 8gb of ram (the machine won't boot with a second stick installed, whether it's 8gb or 16gb)

## Cloudlab

For CTFd and this wiki you are right now reading, I'm using a basic Digital Ocean droplet with 1GB of memory and 25GB of disk space. I want my public services to stay online consistently and my on-premsise infrastructure is not stable enough for high availability.
