---
title: Module Microcontroller Selection
tags:
- tag1
- tag2
---

## Overview

This page will go over the selection of the microcontroller used for the HMI module. It would focus on the ESP32 and how the configuration were made to ensure connectivity for the OLED and communication for the Team 307's Submersible Exploration Device. 

## ESP32 Table of Contents
| ESP Info                                      | Answer | 
| --------------------------------------------- | ------ | 
| ESP32-S3-WROOM-1-N8R8  | [Product Link](https://www.digikey.com/en/products/detail/espressif-systems/ESP32-S3-WROOM-1-N8R8/16705630?gclsrc=aw.ds&gad_source=1&gad_campaignid=20228387720&gbraid=0AAAAADrbLlibQhTWJak6K7PSw4Xuq7jNl&gclid=Cj0KCQiAk6rNBhCxARIsAN5mQLu1rFLmtxPV_GK7DUA-tHljgNQjzwU1_xEu0L1qGVhMom4Mq7k5_AkaAg35EALw_wcB) |
| Datasheet | [ESP32-S3-WROOM-1](https://www.espressif.com/sites/default/files/documentation/esp32-s3-wroom-1_wroom-1u_datasheet_en.pdf) |
| Vendor | [Espressif Systems](https://www.digikey.com/en/supplier-centers/espressif-systems?_gl=1*zml3xs*_up*MQ..*_gs*MQ..&gclid=Cj0KCQiAk6rNBhCxARIsAN5mQLu1rFLmtxPV_GK7DUA-tHljgNQjzwU1_xEu0L1qGVhMom4Mq7k5_AkaAg35EALw_wcB&gclsrc=aw.ds&gbraid=0AAAAADrbLlibQhTWJak6K7PSw4Xuq7jNl) |
| Unit cost                                     | $6.13/each      |
| Supply Voltage Range  | 3V ~ 3.6V  |
| Absolute Maximum current | 500mA     |
| Maximum GPIO current <br> (per pin)           | 40mA     |
| Supports External Interrupts?                 | Yes (All GPIOs)      |
| Programming Hardware    | Micropython     | 

## Pin layout for ESP32
| Module         | # Available | Needed | Associated Pins  |
| -------------- | ----------- | ------ | ------------------------------ |
| UART           | 3           | 1      | Rx - RXD0 and Tx - TXD0 |
| I2C            | 38          | 2      | IO15 and IO16 |
| GPIO           | 38          | 8      | IO6/IO7/IO11/IO12/IO13/IO14/IO46/IO23                              |
| LED            | 38          | 2      | IO10 and IO5                               |
| USB Programmer | 2           | 2      | IO19 and IO20                              |

