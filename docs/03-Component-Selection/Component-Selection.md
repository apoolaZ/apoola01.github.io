---
title: Module's Selected Major Components
---

## Module's Selected Major Components

This page outlines the main components selected for the Human Machine Interface (HMI) module. The list includes power sources (barrel jacks), power regulators and OLEDs. These three are the main focuses of this page as the resistors, compacitors, leds, and headers are provided from the course. 

## Power Source

### Choice 1: CONN PWR JACK 1.35X3.5MM SOLDER

![TH Barrel Jack](TH_Barrel.webp)

* **Price:** $0.67/each
* **Product Link:** [Pj-007](https://www.digikey.com/en/products/detail/same-sky-formerly-cui-devices-/PJ-007/263523?gclsrc=aw.ds&gad_source=1&gad_campaignid=17336967819&gbraid=0AAAAADrbLlgs4hw9LztVYDF5uuUEHngrn&gclid=Cj0KCQiAk6rNBhCxARIsAN5mQLsoOYExZJqYb1FyfbmE2W-5naa-h_G_fIaPOKq9fLMpaS6GJ0RPOZUaAtrQEALw_wcB)

| **Pros** | **Cons** |
| ----------------- | ----------------- |
| Inexpensive compared to others | Needs correct orientation | 
| Easy to install | polarity needs to correct | 
| Already given CAD Model | Familar |

### Choice 2: Power Barrel Connector Jack 2.10mm ID (0.083"), 5.50mm OD (0.217") Surface Mount

![SMD Barrel Jack](SM_Barrel.jpg)

* **Price:** $0.91/each
* **Product Link:** [PJ-006A-SMT-TR](https://www.digikey.com/en/products/detail/same-sky-formerly-cui-devices/PJ-006A-SMT-TR/408456)

| **Pros** | **Cons** |
| ----------------- | ----------------- |
| Can handle temperature when soldering | Expensive | 
| Is a Surface Mount | Harder to place in PCB design | 
| Has 5,000 cycles of life| --- |

### Choice 3: CONN PWR JACK 2X5.5MM SOLDER

![K_Barrel Jack](K_Barrel.webp)

* **Price:** $0.69/each
* **Product Link:** [KLDX-0202-A](https://www.digikey.com/en/products/detail/kycon-inc/KLDX-0202-A/9975992)

| **Pros** | **Cons** |
| ----------------- | ----------------- |
| A TH component | Orientation is different from classic | 
| Detailed Datasheet | Different CAD Model | 
| Operating Temperature: -25˚C to +85˚C | --- |

### Selected Component

The component selected for the power source is option 1: CONN PWR JACK 1.35X3.5MM SOLDER. The main reason is the pricing being significantly cheaper if ordered in bulk as this is a critical piece for the PCB. Furthermore, this item is given in class and something that we are familiar when working with it for other labs throughout the course. 

## Power Regulator

### Choice 1: Linear 3.3V Voltage Regulator
![3 prong 3.3V Voltage Regulator](3p.webp)

* **Price:** $0.41/each
* **Product Link:** [L7809CV](https://www.digikey.com/en/products/detail/umw/L7809CV/24889965?gclsrc=aw.ds&gad_source=1&gad_campaignid=21136823955&gbraid=0AAAAADrbLli0bIFVhRCsyialuzG6uLAUV&gclid=Cj0KCQiAk6rNBhCxARIsAN5mQLvVgdvWiP_iBn4oW_0oh67-wxJjyq7hfaxu65XctnEDpUbIFSJuw18aAkpmEALw_wcB)

| **Pros** | **Cons** |
| ----------------- | ----------------- |
| Very simple to use | A through-hole which we cannot use| 
| Linear | Only 3 prongs which doesn't have the stuff required for the project | 
| --- | DC-DC Conversion |


### Choice 2: Switching Regulator IC Positive Fixed 3.3V 
![SOT 3.3 Voltage Regulator](VOLT.webp)

* **Price:** $0.22/each
* **Product Link:** [AP2112K-3.3TRG1](https://www.digikey.com/en/products/detail/diodes-incorporated/AP2112K-3-3TRG1/4470746)

| **Pros** | **Cons** |
| ----------------- | ----------------- |
| Better Performance | Generates heat at high Voltage  | 
| Cheap to order  | has a 600MA limit | 
| Can solder easily on board | --- |


### Choice 3: SMD 3.3V Power Regulator
![SMD 3.3 Voltage Regulator](SMDvolt.webp)

* **Price:** $0.25/each
* **Product Link:** [MIC5528-3.3YMT-TR](https://www.digikey.com/en/products/detail/microchip-technology/MIC5528-3-3YMT-TR/4864020)

| **Pros** | **Cons** |
| ----------------- | ----------------- |
| Has protection for over current/temperature | Out of the three options, it is slightly expensive | 
| Can handle -40°C ~ 125°C | Can be difficult to install | 
| Saves space on the PCB Board | --- |

### Selected Component

The selected component for this project is the second option: Switching Regulator IC Positive Fixed 3.3V. The reason why is because it has all the pinouts that are required for the main project and is inexpensive to order multiple for different scenerios. Furthermore, it would easier to implement in the PCB design and when soldering in-person.

## OLED Screen

### Choice 1:

| **Pros** | **Cons** |
| ----------------- | ----------------- |
|  |  | 
|  |  | 
|  |  |
|  |  | 

### Choice 2:

| **Pros** | **Cons** |
| ----------------- | ----------------- |
|  |  | 
|  |  | 
|  |  |
|  |  | 

### Choice 3:

| **Pros** | **Cons** |
| ----------------- | ----------------- |
|  |  | 
|  |  | 
|  |  |
|  |  | 

### Selected Components:
