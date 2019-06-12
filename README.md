# Image Segmentation Robot System

This application, which implements a image semantic segmentation on ARC IoT board, is designed to show how to use camera and Machine Learning in embARC.

* [Introduction](#introduction)
	* [Function](#function)
	* [System Architecture](#system-architecture)
* [Hardware and Software Setup](#hardware-and-software-setup)
	* [Required Hardware](#required-hardware)
	* [Required Software](#required-software)
	* [Hardware Connection](#hardware-connection)
* [User Manual](#user-manual)
	* [Before Running This Application](#before-running-this-application)
	* [Run This Application](#run-this-application)

## Introduction
This project was successful in achieving a two-wheeled autonomous robot based on the inverted pendulum model.EMSK works as controller, it will deal with sensor datas and interact with user via bluetooth. We can view all data on serial terminal, and sent instructions to the robot to change its motion mode.

### Function

### System Architecture
![system architecture][4]

## Hardware and Software Setup
### Required Hardware
- [ARC IoT Development Kit][1]
- [OV7670 Camera Module][2]

### Required Software
- ARC GNU Toolset 2019
- Serial port terminal, such as putty, tera-term or minicom
- Synoposys Machine Learning Library

### Hardware Connection
1. Connect OV7670 camera module to ARC following below instructions

        # ARC: 2x18 Pin Extension Header
        SIOC   ->    I2C0_SCL (need pull-up 10K resistor)
        SIOD   ->    I2C0_SDA (need pull-up 10K resistor)

        # ARC: Arduino PIN
        VSYBC  ->    arduino IO0
        PCLK   ->    arduino IO1
        XCLK   ->    arduino IO3
        D7~D0  ->    arduino IO4~IO11

        3V3    -> +3.3V
        RESET  -> +3.3V
        GND    -> GND
        PWDN   -> GND

## User Manual
[1]: https://embarc.org/embarc_osp/doc/build/html/board/iotdk.html "ARC IoT Development Kit"
[2]: https://www.voti.nl/docs/OV7670.pdf "OV7670 Camera Module"
