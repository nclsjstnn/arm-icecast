# ARM-ICECAST
The streaming server Icecast. Optimized for raspberrypi3-debian. To use with MPD.

This is an image for the streaming application [Icecast](http://icecast.org/) using Debian with an ARMv7 architecture (to run inside a Raspberry-Pi ARMv7) as the operating system.

# How to use 

    docker run -p 8000:8000 --name=icecast -d jstnn/arm-icecast:latest

An instance of icecast is now running with the port 8000 mapped to your host or docker-machine IP address.

# Custom configuration 

Check the github repository and you will find an `icecast.xml` you can edit and set your custom configuration. You just need to build the image again.

The passwords in the configuration are just for testing purposes.

# Credits

This dockerfile is based on the [alpine-icecast image](https://hub.docker.com/r/vitiman/alpine-icecast/). Changes has been made to compile using a raspberrypi
