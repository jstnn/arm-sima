# arm-sima

This is an image for the interactive autoqueue client [MPD-sima](http://kaliko.me/code/mpd-sima/) using Debian. A [Resin.os Raspbian image](https://hub.docker.com/r/resin/rpi-raspbian/) is used as a base image for compatibility with IoT devices, but it works well anywhere. This is an add-on for MPD.

The idea is use this image together with a fully audio stack. You can edit the `sima.conf` or use the fully audio stack I created.

# How to use 

    docker run --name=sima -d jstnn/arm-sima:latest

An instance of sima is running. 

# Custom configuration 

Check the github repository and you will find a `sima.conf` you can edit and set your custom configuration. You just need to build the image again.

The passwords in the configuration are just for testing purposes.

# Credits

This dockerfile is based on the [alpine-sima image](https://hub.docker.com/r/vitiman/alpine-sima/). Changes has been made to compile with an IoT device with an ARMv7 architecture like the RaspberryPi 3 using a resin.os optimized image.
