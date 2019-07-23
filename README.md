# Docker image for OpenSTLinux build (Yocto Linux)

[Docker Hub link](https://hub.docker.com/r/kbumsik/build-yocto-st)

This is an Ubuntu 16.04 image that contains necessary packages to build OpenSTLinux.
The advantage is that you can build OpenSTLinux without installing Ubuntu 16.04
on your machine. This is very useful for Windows and other Linux (e.g. Arch) users.

I successfully build STM32MP1 Distribution Package OpenSTLinux distribution
`openstlinux-4.19-thud-mp1-19-02-20` using this image.
For instructions on how to build this Yocto Linux distribution, please refer
[ST's official Wiki](https://wiki.st.com/stm32mpu/wiki/STM32MP1_Distribution_Package).
You need to run the following `docker run` command before following the instruction.

Usage example:

    docker run -it \
        --volume=${PWD}:/build \
        --volume=/my/sstate/dir:/sstate \
        kbumsik/build-yocto-st \
        /bin/bash

Setting /ssate volume is optional, use it if you need your own sstate directory.
