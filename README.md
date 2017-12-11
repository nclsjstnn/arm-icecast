# arm-icecast

This docker image runs the streaming application [Icecast](http://icecast.org/) using Debian. A [Resin.os Raspbian image](https://hub.docker.com/r/resin/rpi-raspbian/) is used as a base image for compatibility with IoT devices, but it works well anywhere, it's just a dockerfile.

# How to use 

    docker run -p 8000:8000 --name=icecast -d jstnn/arm-icecast:latest

An instance of icecast is now running with the port 8000 mapped to your host or docker-machine IP address.

# Custom configuration 

Check the github repository and you will find an `icecast.xml` you can edit and set your custom configuration. You just need to build the image again.

The passwords in the configuration are just for testing purposes.

# Credits

This dockerfile is based on the [alpine-icecast image](https://hub.docker.com/r/vitiman/alpine-icecast/). Changes has been made to compile with an IoT device with an ARMv7 architecture like the RaspberryPi 3 using a resin.os optimized image.
