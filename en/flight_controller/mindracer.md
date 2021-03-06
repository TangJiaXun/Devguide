# MindRacer Hardware

The MindRacer series were created by AirMind. Please refer to: http://mindpx.net

![](../../assets/hardware/hardware-mindracer.png)

## Quick Summary

MindRacer is a fully stackable flight platform for miniature UAVs. Based on MindPX, MindRacer further scales down in formfactor while focused on providing modularity. MindRacer is a platform rather than a flight controller.
MindRacer implements the SEP(soldering-elimination-port) and WEP(wiring-elimination-protocol) concepts. Before SEP and WEP, soldering and wiring are always the major pain and efficiency killer during UAV manufacturing and tuning.

> **Note** The main hardware documentation is here: http://mindpx.net/assets/accessories/mindracer_spec_v1.2.pdf

- Ultra mini size, weight ~6g
- High performance STM32F427 168MHz floating point processor, super fast throttle response
- Support OneShot ESC
- Support PPM/SBUS/DSM radio receivers, support D.Port/S.Port/Wifi telemetry
- On board flight data recorder
- Support IMU isolation
- DroneCode standard compliance connector

|Item|Description|
|:--:|:--:|
|Flight controller/Processor|F427VIT6|
|Weight|~6g|
|Dimension|35x35mm|
|PWM Outputs|maximum 6|
|IMU|10DOF|
|IMU isolation|YES/Optional|
|Radio Receiver|S.BUS/PPM/DSM/DSM2/DSMX/SUMD|
|Telemetry|FrSky D.Port, S.Port, Wifi, 3DR radio|
|On board TF card for flight data recording|YES|
|OneShot ESC Support|YES|
|Expansion Slots|2x7(pin)x2|
|On board Real time clock|YES|
|Connector|JST GH(compliance with DroneCode standard)|

## Quick Start

### Pin out map

![](../../assets/hardware/hardware-mindracer-pinout.png)

### How to build

Please follow [Getting Started](setup/getting_started.md) and [Building the Code](setup/building_px4.md).  And the target for MindRacer is \[nuttx_\]mindpx-v2_default (it's right, compatible with MindPX):

`make nuttx_mindpx-v2_default`

### Companion PC connection

MindRacer has an attached Adapt IO board. 

![](../../assets/hardware/hardware-mindracer-conn.png)

MindRacer has a built-in UART-to-USB convertor. To connect a companion computer, stack MindRacer on an interface board, and connect the companion computer to the USB port on the interface board.

And the max BAUD rate is the same with px4 family, which is up to 921600.

### User Guide

> **Note** The user guide is here: http://mindpx.net/assets/accessories/mindracer_user_guide_v1.2.pdf

## Where to buy

MindRacer is available at [AirMind Store](http://drupal.xitronet.com/?q=catalog) on internet. You can also find MindRacer at Amazon or eBay.

## Support

Please visit http://www.mindpx.org for more information. Or you can send email to <support@mindpx.net> for any inquiries or help.
