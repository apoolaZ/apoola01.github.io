---
title: Module's Requirements
---
## Overview

The table below are requirements formed based on the needs of Team 307's project. This portion heavily focuses on the Human Machine Interface (HMI). In order to achieve this, I have decided to be focusing on the OLED module which allows users to interact with the machine through the screen. How users would interact with the machinery is by pushing a button on the PCB. When the button is pushed, the motor either moves clockwise (0) or counter-clockwise (1). As the motor is moving, the OLED displays the distance detected from the distance sensor and displays it on the screen.

## Module Requirement

| **Requirement Description** | **Measure of<br> Threshold** | **Target<br>Measure** |**Stretch<br>Requirement<br>(Y-N)**|
|-----------------------------| ----------------- | ----------------- | :-----: |
| Surface Mounted, 3.3V Switching Power Regulator | 3.2 Volts | 3.3 Volts | No |
| Surface Mounted Microcontroller | 1 PIC or ESP | 8-bit PIC | No |
| OLED Screen| Be able to showcase data  | Allows users to be able to see data by interacting with screen | No |
| Wired Communication | Ability to receive/send wired data (RX/TX) |  Receive/Send wired data through 8-pin headers | No |
| Wireless Communication | Able to receive/send Wifi data | Receive/Send Wifi data using MQTT | Yes |
