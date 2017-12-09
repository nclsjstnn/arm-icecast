# arm_icecast
The streaming server Icecast. Optimized for raspberrypi3-debian. To use with MPD.

This is an image for the streaming application [Icecast](http://icecast.org/) using alpine as the operating system.

Based on the [alpine-icecast image](https://hub.docker.com/r/vitiman/alpine-icecast/). This is intended to run on a raspberrypi-3 using the resin.io debian image.


# How to use 

    docker run -p 8000:8000 --name=icecast -d jstnn/alpine-icecast:latest

An instance of icecast is now running with the port 8000 mapped to your host or docker-machine IP address.

# Custom configuration 

Check the github repository and you will find an `icecast.xml` you can edit and set your custom configuration. You just need to build the image again.

The passwords in the configuration are just for testing purposes.
