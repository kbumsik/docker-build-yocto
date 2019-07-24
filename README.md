# Docker images collection for building various Yocto Linux distributions

This repo is a collection of Dockerfiles to build various Yocto Linux distros.

The advantage of using Docker is that you can build Yocto Linux without
installing a full Ubuntu or such VM. This is very useful for Windows and
other Linux (e.g. Arch) users.

Currently this repo contains the following Docker images:

* [`openstlinux`](openstlinux): To build Yocto Linux for STM32MP1 Discovery boards (aka. [STM32MP1 Distribution Package](https://wiki.st.com/stm32mpu/wiki/STM32MP1_Distribution_Package)).
* [`balena-raspberrypi`](balena-raspberrypi): To build [Balena OS image for Raspberry Pi](https://github.com/balena-os/balena-raspberrypi).
