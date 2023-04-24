---
layout: page
title: Getting started with building your own ArseLinux OS
permalink: /getting-started/
---

The ISO files are already available here - https://github.com/ArseLinuxOS-Development/ArseLinuxOS-ISO/releases

But if you wish to help out with development it's always handy to know how to build an ISO yourself.

[ArseLinuxOS-ISO](https://github.com/ArseLinuxOS-Development/ArseLinuxOS-ISO)

This ISO is based on a modified Arch-ISO to provide Installation Environment for ArseLinuxOS. As you can imagine, this project is for fun and isn't meant to be used for anything serious, or rather, anything at all.

### Building

    git clone https://github.com/LiamAEdwards/ArseLinuxOS-ISO.git && cd ArseLinuxOS-ISO
    mkarchiso -v -w /archiso-tmp -o ../ .

### With Docker

    docker build -t arselinux-build . --no-cache
    docker run --privileged -it arselinux-build:latest /bin/bash

Once completed you will have an ISO image to test/boot.
