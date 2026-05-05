---
title: Hardware V2.0
tags:
- tag1
- tag2
---

## Overview

There was a lot that I learned from this project. One major thing I would improve on is the design of the PCB Board itself as I cam across many hardware issues. I assumed a lot of things for this project, but a huge flaw was the Micro-USB port as I assumed that power going through the port was 3.3V. After going through with it with the professor and others, I needed to manually solder the D+/D- and ground wires from a cable to the ESP32 to make sure I don't fry the ESP32. If given another chance with this project, I wiuld throughly research and consult with the professor before manufactor to avoid this error again. 

Another thing I would change is the layout of the components as it looks like it's all over the place and it got confusing on where things are supposed to go. Furthermore, I should've double checked the pinouts of certain components as there were times (like the layout of the OLED in the schematic) where it was completely wrong, so I had to manually rewire/solder certain parts to get it to work.

In conclusion, the PCB design is one thing I would heavily improve on if given another chance to work on this project as many issues stemmed from is the traces right and did I order/read the right part (such as accidentally using an ADJ regulator instead of the class one).

