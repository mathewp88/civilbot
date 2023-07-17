# Civilbot

The civilbot is a project to test basic mapping and navigation using a lidar for a 4 wheeled robot.

## Objectives:

* Make a low cost robotics platform
* Test both the lidar and stero camera
* Test the feasability of the ZED Open Capture Library
* Have full navigation and mapping capabilities


### Hardware and Low Level Code 

The rover was controlled using the two front wheels in a differential drive configuration. 
An arduino was used to receive signals from the wheel encoders and to send signals to the motor driver. 
As the low level code is dependent on both the motor driver and the wheel encoders, I have omitted the code form this repo.

### High level Architecture

The overall system based on the ROS architecture more specifially the ROS Navstack and Hector Mapping.
As an experiment I opted to test the ZED open capture library, however the video processing ran too slowly on a Raspberry Pi 4B although capturing sensor data worked without any issues.
