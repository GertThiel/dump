# Docker #

[Docker](https://www.docker.com/)

## Docker Hosts ##

[Atomic](http://www.projectatomic.io/)

[Boot2Docker](https://github.com/boot2docker/boot2docker)

[CoreOS](https://coreos.com/)

[OSv](http://osv.io/)

[RancherOS](http://rancher.com/rancher-os/)
([Documentation](http://docs.rancher.com/os/),
[Github](https://github.com/rancher/os),
[Vagrantfile](https://github.com/rancher/os-vagrant))
is an OS made of containers.
In RancherOS, the Docker daemon runs as first process the kernel starts when it boots.
We call this instance of Docker "System Docker," as it is responsible for initiating system services,
such as udev, DHCP and the console. Each of these system services run as containers.
System Docker takes the place of the init system, such as sysvinit or systemd, in other Linux distributions.

[Docker @ wiki.debian.org](https://wiki.debian.org/Docker)

[How to install and setup **Debian 8** minimalist Docker Host](https://linuxconfig.org/how-to-install-and-setup-debian-8-minimalist-docker-host)

[phusion/baseimage-docker](https://github.com/phusion/baseimage-docker)
is a minimal **Ubuntu** base image modified for Docker-friendliness

## Smaller Docker Images ##

[Docker Base Image OS Size Comparison](https://www.brianchristner.io/docker-image-base-os-size-comparison/)
