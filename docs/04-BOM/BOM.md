---
title: Module Bill of Materials
tags:
- tag1
- tag2
---

## Overview

This page goes over the materials that are needed for the HMI Module to ensure. Some of the parts (ESP32, Power Regulator, Test Points) were ordered through Arizona State University while other parts were personally funded. The Bill of Materials is based off the [schematic](https://apoolaz.github.io/apoola01.github.io/05-Schematic/schematic/) and the [component selection](https://apoolaz.github.io/apoola01.github.io/03-Component-Selection/Component-Selection/) to determine what parts were needed to order.

## Bill of Materials 

| Part Name/ Description | QTY | Unit Cost | Total Cost | Manufacture | Manufacturer \# | Vendor Link | Datasheet Link | Schematic Ref. Designators |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| Buck Switching Regulator IC Positive Fixed 3.3V 1 Output 1A TO-263-6, D2PAK (5 Leads + Tab), TO-263BA | 2 | $2.23 | $4.46 | onsemi | LM2575D2T-3.3R4G | [Vendor](https://www.digikey.com/en/products/detail/onsemi/LM2575D2T-3-3R4G/1476688?s=N4IgTCBcDaIDIFkwFYDsyAiYAqBaAzAHT4BKALAOIgC6AvkA) | [Datasheet](https://www.onsemi.com/pdf/datasheet/lm2575-d.pdf)  | U1 |
| Bluetooth, WiFi 802.11b/g/n, Bluetooth v5.0 Transceiver Module 2.4GHz PCB Trace Surface Mount (ESP32) | 2 | $5.06 | $10.12 | Espressif | ESP32-S3-WROOM-1-N4 | [Vendor](https://www.digikey.com/en/products/detail/espressif-systems/ESP32-S3-WROOM-1-N4/16162639)  | [Datasheet](https://www.espressif.com/sites/default/files/documentation/esp32-s3-wroom-1_wroom-1u_datasheet_en.pdf)  | U2 |
| PC TEST POINT MINIATURE RED | 20 | $0.28 | $4.16 | Keystone Electronics | 5000 | [Vendor](https://www.keyelco.com/userAssets/file/K75p62.pdf)  | [Datasheet](https://www.digikey.com/en/products/detail/keystone-electronics/5000/255326)  | TP1, TP2, TP3, TP4, TP5, TP6, TP7, TP8 |
| 5600PCS 0805 SMD Resistor Kit from 0Ω to 10MΩ 1%, Electronics Component Assortment with Resistors, Capacitors, Diodes, Transistors, IC, Inductors, LEDs Sample Book for DIY and Repair  | 1 | $29.90 | $29.90 | EGSCST | B0DZXQPFHP | [Vendor](https://www.amazon.com/EGSCST-Electronics-Assortment-Capacitors-Transistors/dp/B0DZXQPFHP/ref=sr_1_1_sspa?dib=eyJ2IjoiMSJ9.OfRWEABdLA3kZNJHHYAVfZ4YJEW0lG5rjM_ZGk1NJwz6u2tDkRlYrmb8-QBM5cKSXuiTFUlcwfXikBKYKCMwEZWIxGv3DG40NdoL-VYJlP6V5Oa3DiArBIAjMEkbnkzY-UbCXw-CaH4PHLVXwFoVVuJXPWjp1K2nEmG0MF_K_SSV9xtbp-fNMDuI_VKO1PGfGyesvfGc4V5L1YS4Ksu6CqMKMXBJCiR8K1aiBWHSucE.w-NP-ytdijrmRG2kkppWNjyL2NDtBwMBDma-0-UOqEU&dib_tag=se&keywords=smd%2Bkit&qid=1773159525&sr=8-1-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9hdGY&th=1)  | \- | R1, R2, R3, R4, R5, R6, R7, R8, C1, C2, C3, D1, D2, D3 |
| 1 A 32 V Fuse Board Mount (Cartridge Style Excluded) Surface Mount 0805 (2012 Metric)  | 1 | $0.53 | $0.53 | Vishay | MFU0805FF01000P100 | [Vendor](https://www.digikey.com/en/products/detail/vishay/MFU0805FF01000P100/1206490)  | [Datasheet](https://www.vishay.com/docs/28747/mfuserie.pdf) | F1 |
| 385PCS 27Values Micro Momentary Tactile Push Button Switch Assortment Kit 2 Pins/3 Pins/4 Pins Tact Pushbutton Switches Set | 1 | $14.99 | $14.99 | EGSCST | 385PCS-Switch | [Vendor](https://www.amazon.com/dp/B0FWB4ZVKJ/ref=sspa_dk_hqp_detail_aax_0?sp_csd=d2lkZ2V0TmFtZT1zcF9ocXBfc2hhcmVk&th=1) | \- | SW1, SW2, SW3, SW4 |

