# AutoDrive II - Camera Drivers

This repository contains ROS packages for cameras made by FLIR Imaging (formerly known as PointGrey), this is a fork from [the original ROS drivers repository](https://github.com/ros-drivers/flir_camera_driver).

## Current cameras:
1. **Center Camera (Ethernet)**
   - Topic Name: *"/flir_camera"*
   - Serial: 21066574
   - IP Adress: 192.168.0.11
   - Model: [Blackfly S BFS-PGE-120S4C](https://www.flir.com/products/blackfly-s-gige/?model=BFS-PGE-120S4C-CS&vertical=machine+vision&segment=iis)
   - Lens: ???

2. **Center Camera (USB)**
   - Topic Name: *"/cam_usb"*
   - Serial: ???
   - IP Adress: ???
   - Model: [Blackfly S BFS-U3-200S6C-C](https://www.flir.com/products/blackfly-s-usb3/?model=BFS-U3-200S6C-C&vertical=machine+vision&segment=iis) (please confirm)
   - Lens: ???

3. **Left Camera (Ethernet)**
   - Topic Name: *"/cam_left"*
   - Serial: 17453014
   - IP Adress: 192.168.1.21
   - Model: [Blackfly BFLY-PGE-23S6C](https://www.flir.com/products/blackfly-gige/?model=BFLY-PGE-23S6C-C&vertical=machine+vision&segment=iis)
   - Lens: [Tamron 23FM65](https://www.avsupply.com/ITM/1699/23fm65.html)

4. **Right Camera (Ethernet)**
   - Topic Name: *"/cam_right"*
   - Serial: 16066975
   - IP Adress: 192.168.1.23
   - Model: [Blackfly BFLY-PGE-23S6C](https://www.flir.com/products/blackfly-gige/?model=BFLY-PGE-23S6C-C&vertical=machine+vision&segment=iis)
   - Lens: [Tamron 23FM65](https://www.avsupply.com/ITM/1699/23fm65.html)

## Packages

### spinnaker_camera_driver
The camera driver supports USB3 and GIGE cameras. The driver has been
successfully used for Blackfly, Blackfly S, Chameleon, and Grasshopper
cameras, but should support any FLIR camera that is based on the
Spinnaker SDK. See the
[spinnaker_camera_driver](spinnaker_camera_driver/README.md) for more.
This software is issued under the Apache License Version 2.0 and BSD

### flir_camera_msgs
Package with with [image exposure and control messages](flir_camera_msgs/README.md).
These are used by the [spinnaker_camera_driver](spinnaker_camera_driver/README.md).
This software is issued under the Apache License Version 2.0.

### flir_camera_description
Package with [meshes and urdf](flir_camera_description/README.md) files.
This software is released under a BSD license.
