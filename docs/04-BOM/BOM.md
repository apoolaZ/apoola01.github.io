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
| Buck Switching Regulator IC Positive Adjustable 1.2V 1 Output 3A TO-263-6, D2PAK (5 Leads \+ Tab), TO-263BA | 2 | $5.91 | $11.82 | UMW | LM2596HVS-ADJ | [Vendor](https://www.digikey.com/en/products/detail/umw/LM2596HVS-ADJ/16842152?gclsrc=aw.ds&gad_source=1&gad_campaignid=21136823955&gbraid=0AAAAADrbLljZpI0SsZ4sJXFNmhFGfhN2I&gclid=Cj0KCQjwgr_NBhDFARIsAHiUWr6UDMAJC9ENGULzuyYLmnFkEWxnuukVFu1KhG3kBfGe4BE9L-kEGiUaAlgAEALw_wcB)  | [Datasheet](https://mm.digikey.com/Volume0/opasdata/d220001/medias/docus/2577/UMW%20LM2596_HV.pdf?_gl=1*fmqm0t*_up*MQ..*_gs*MQ..&gclid=Cj0KCQjwgr_NBhDFARIsAHiUWr6UDMAJC9ENGULzuyYLmnFkEWxnuukVFu1KhG3kBfGe4BE9L-kEGiUaAlgAEALw_wcB&gclsrc=aw.ds&gbraid=0AAAAADrbLljZpI0SsZ4sJXFNmhFGfhN2I)  | U1 |
| Bluetooth, WiFi 802.11b/g/n, Bluetooth v5.0 Transceiver Module 2.4GHz PCB Trace Surface Mount (ESP32) | 2 | $5.06 | $10.12 | Espressif | ESP32-S3-WROOM-1-N4 | [Vendor](https://www.digikey.com/en/products/detail/espressif-systems/ESP32-S3-WROOM-1-N4/16162639)  | [Datasheet](https://www.espressif.com/sites/default/files/documentation/esp32-s3-wroom-1_wroom-1u_datasheet_en.pdf)  | U2 |
| PC TEST POINT MINIATURE RED | 20 | $0.28 | $4.16 | Keystone Electronics | 5000 | [Vendor](https://www.keyelco.com/userAssets/file/K75p62.pdf)  | [Datasheet](https://www.digikey.com/en/products/detail/keystone-electronics/5000/255326)  | TP1, TP2, TP3, TP4, TP5, TP6, TP7, TP8 |
| 5600PCS 0805 SMD Resistor Kit from 0Ω to 10MΩ 1%, Electronics Component Assortment with Resistors, Capacitors, Diodes, Transistors, IC, Inductors, LEDs Sample Book for DIY and Repair  | 1 | $29.90 | $29.90 | EGSCST | B0DZXQPFHP | [Vendor](https://www.amazon.com/EGSCST-Electronics-Assortment-Capacitors-Transistors/dp/B0DZXQPFHP/ref=sr_1_1_sspa?dib=eyJ2IjoiMSJ9.OfRWEABdLA3kZNJHHYAVfZ4YJEW0lG5rjM_ZGk1NJwz6u2tDkRlYrmb8-QBM5cKSXuiTFUlcwfXikBKYKCMwEZWIxGv3DG40NdoL-VYJlP6V5Oa3DiArBIAjMEkbnkzY-UbCXw-CaH4PHLVXwFoVVuJXPWjp1K2nEmG0MF_K_SSV9xtbp-fNMDuI_VKO1PGfGyesvfGc4V5L1YS4Ksu6CqMKMXBJCiR8K1aiBWHSucE.w-NP-ytdijrmRG2kkppWNjyL2NDtBwMBDma-0-UOqEU&dib_tag=se&keywords=smd%2Bkit&qid=1773159525&sr=8-1-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9hdGY&th=1)  | \- | R1, R2, R3, R4, R5, R6, R7, R8, C1, C2, C3, D1, D2, D3 |
| BOJACK T1.5AL250V 5x20mm 1.5A 250V Slow Blow Fuses 1.5 amp 250 Volt 0.2 x 0.78 Inch Glass Tube Time-delay Fuses (Pack of 20\)  | 1 |  | 6.99 | BOJACK | B07X1KCTZT | [Vendor](https://www.amazon.com/BOJACK-T1-5AL250V-5x20mm-Fuses-Time-delay/dp/B07X1KCTZT?pd_rd_w=UGsBO&content-id=amzn1.sym.28c64fbb-22b3-4b43-9c44-fc03d50fe5f9&pf_rd_p=28c64fbb-22b3-4b43-9c44-fc03d50fe5f9&pf_rd_r=G0HMJS2JFA7NB2XMD7YG&pd_rd_wg=kL61W&pd_rd_r=5b6eba08-d15e-42b4-a2a7-87973236a586&pd_rd_i=B07X1KCTZT&psc=1&ref_=pd_bap_d_grid_rp_hxwhrp_sspa_dk_bia_0_3_i)  | \- | F1 |


## Resouce

The Bill of Material as a PDF download is available [*here*](PDF_For_BOM_EXAMPLE.pdf).
