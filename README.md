## pi-dev
A local docker-based webdevelopment environment built for Raspberry Pi under Raspbian OS with 64bit kernel

### overview
The goal is to provide developers with a configurable local development environment in their Raspberry Pi by running a set of orchestrated docker containers - a webserver, a database, and php at least - the traditional LAMP stack. Please note that this is experimental and not suited for production servers.

### preparing the Raspbery Pi
Running docker inside a Raspberry Pi raises a fundamental issue: as Pi's architecture is ARM and it's official OS is (still) 32bit, the choice of docker images is limited. Emulating x86_64 architecture on ARM is not viable but we can run a 64bit guest OS inside our 32bit raspbian to gain access to more docker images.

In the following steps we'll briefly cover:
1. installing the official 32bit Raspbian OS on the Raspberry Pi;
2. installing a 64bit guest OS on Raspbian linked to its 32bit host OS, and configuring it in order to be able to run docker;
3. installing docker and docker-compose on the 64bit guest OS.

### downloading the development environment / starting a new local project

### configuring the development environment: available containers
