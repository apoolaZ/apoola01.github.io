title: API Message Definitions (OLED Subsystem)
---

## Overview

For Team 307's submersible exploration device, we will be using a daisy chain network with UART to send messages within one another which came from Team 307's [Message Structure](https://egr-314-team-307-spring-2026.github.io/Team307.github.io/04-Team-Block-Diagram/Team-Diagram/). 

This page is a reflection of the coding done for the project. This is the [Zip file](ESP32_Code.zip) this whole page is based off of. 

## Subsystem Information

| Item | Value |
| ----- | ----- |
| Subsystem Name | OLED / Human Interface Subsystem |
| Subsystem ID | A |
| Broadcast ID | X |
| UART Baud Rate | 9600 |
| Maximum Message Length | 64 bytes |
| Message Prefix | AZ |
| Message Suffix | YB |

The OLED subsystem uses UART to receive messages from other team boards, display the data on the OLED screen, forward messages that are not meant for it, and send a button press message to the motor subsystem. The code defines the OLED subsystem ID as A, uses broadcast ID X, and limits messages to 64 bytes.

## Message Format

All messages follow this format:

AZ \+ Sender ID \+ Receiver ID \+ Payload \+ YB

Example:

AZAGbutton onYB

| Section | Description |
| ----- | ----- |
| AZ | Start of message |
| Sender ID | Device sending the message |
| Receiver ID | Device receiving the message |
| Payload | Message data |
| YB | End of message |


# **Valid Team IDs**

The OLED subsystem recognizes the following team IDs:

A, E, D, J, G, k, Z

Any message from an unknown sender is rejected.


# **Messages Received by OLED**

## **Message From Distance Subsystem**

| Field | Value |
| ----- | ----- |
| Sender ID | J |
| Receiver ID | A |
| Payload Type | String |
| Variable Name | distance_data |
| Min Length | 1 character |
| Max Length | 58 characters |
| Example Payload | 1200 mm |
| Example Message | AZJA1200 mmYB |

**OLED Behavior:**  
 When the OLED receives a message from sender J, it displays:

Distance:  
1200 mm  

## **Message From Pressure Subsystem**

| Field | Value |
| ----- | ----- |
| Sender ID | E |
| Receiver ID | A |
| Payload Type | String |
| Variable Name | pressure_data |
| Min Length | 1 character |
| Max Length | 58 characters |
| Example Payload | 650 |
| Example Message | AZEA650YB |

**OLED Behavior:**  
 When the OLED receives a message from sender E, it displays:

Pressure:  
650  


## **Message From Hall Sensor Subsystem**

| Field | Value |
| ----- | ----- |
| Sender ID | D |
| Receiver ID | A |
| Payload Type | String |
| Variable Name | hall_sensor_data |
| Min Length | 1 character |
| Max Length | 58 characters |
| Example Payload | 300 |
| Example Message | AZDA300YB |

**OLED Behavior:**  
 When the OLED receives a message from sender D, it displays:

Hall Sensor:  
300  

## **Message From Motor Subsystem**

| Field | Value |
| ----- | ----- |
| Sender ID | G |
| Receiver ID | A |
| Payload Type | String |
| Variable Name | motor_data |
| Min Length | 1 character |
| Max Length | 58 characters |
| Example Payload | motor on |
| Example Message | AZGAmotor onYB |

**OLED Behavior:**  
 When the OLED receives a message from sender G, it displays:

Motor Data:  
motor on  

# **Message Sent by OLED**

## **Button Press Message**

| Field | Value |
| ----- | ----- |
| Message Name | Button Event |
| Sender ID | A |
| Receiver ID | G |
| Payload Type | String |
| Variable Name | button_state |
| Payload Value | button on |
| Example Message | AZAGbutton onYB |

**Purpose:**  
 When the button connected to GPIO 35 is pressed, the OLED subsystem sends a message to subsystem G with the payload button on.


# **Broadcast Message Handling**

| Field | Value |
| ----- | ----- |
| Receiver ID | X |
| Behavior | Display and forward |
| Example Message | AZJXdistance 1200YB |

If the OLED receives a broadcast message, it displays the sender and payload, then passes the message along the UART chain.

# **Error Handling**

The OLED subsystem handles these message errors:

| Error | OLED Response |
| ----- | ----- |
| Message longer than 64 bytes | Displays ERROR Msg too long |
| Unknown sender ID | Displays Bad Sender |
| Message from itself | Displays From Self Ignored |
| Invalid or incomplete message | Ignored |
| Message not for OLED | Forwarded |

