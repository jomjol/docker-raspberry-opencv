# docker-raspberrypi3-opencv
 OpenCV 4.1 on Raspberry B3
 
This repository creates a Docker-Image with OpenCV 4.1 installed in a Python 3.7 environment running on a docker installation on a Raspberry B3

**Even if the os/arch is shown as "linux/amd64" it is build for "linux/armv7"**

## Docker-Versions

| Label | 	Content  |
| -------------- | -------------|
| latest | identical to v1.0.0 (Status 2019-12-27) | 
| v1.0.0 | Inital Version - Tested and Running | 


## Content
| Software | Version | Comment |
| --------- | ------- | ------- |
| OpenCV | 4.1 |  |
| Python | 3.7 |  |
| Raspberry | B3 - armv7 |  |

## Changelog - lastest version
##### 1.0.0 (2019-12-27)
* Running and tested version
##### 0.9.0 (2019-12-08)
* Inital Vesion

### [Full Changelog](Changelog.md)

## Remark
It is necessary to extend the preload path for the specific library libatomic.so.1.2.0:

```ENV LD_PRELOAD=$LD_PRELOAD:/usr/lib/arm-linux-gnueabihf/libatomic.so.1.2.0```


