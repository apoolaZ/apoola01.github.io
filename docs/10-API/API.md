title: API Message Definitions (OLED Subsystem)
---

## Overview

For Team 307's submersible exploration device, we will be using a daisy chain network with UART to send messages within one another which came from Team 307's [Message Structure](https://egr-314-team-307-spring-2026.github.io/Team307.github.io/04-Team-Block-Diagram/Team-Diagram/). The communication roles for the UART in this module is split into two:

* **Receives:** distance, pressure, temperature, status, errors, emergency stop
* **Sends:** HMI display updates, HMI button events, optional status requests

## Message Types

### Message Type 3 - Distance Value

| Field | Byte(s) | Type | Variable Name | Min | Max |
| ---- | ---- | ---- | ---- | ---- | ---- |
| Message Type | 1-2 | uint16_t | message_type | 3 | 3 |
| Distance | 3-4 | uint16_t | distance_value | 0 | 4000 |
| Padding | 5-58 | uint8_t[] | padding | 0 | 0 |

### Message Type 5 - Depth/Pressure Value

| Field | Byte(s) | Type | Variable Name | Min | Max |
| ---- | ---- | ---- | ---- | ---- | ---- |
| Message Type | 1-2 | uint16_t | message_type | 5 | 5 |
| Depth/Pressure | 3-4 | uint16_t | pressure_value | 0 | 10000 |
| Padding | 5-58 | uint8_t[] | padding | 0 | 0 |

### Message Type 6 - Temperature Value

| Field | Byte(s) | Type | Variable Name | Min | Max |
| ---- | ---- | ---- | ---- | ---- | ---- |
| Message Type | 1-2 | uint16_t | message_type | 6 | 6 |
| Temperature | 3-4 | uint16_t | temperature_c | 0 | 125 |
| Padding | 5-58 | uint8_t[] | padding | 0 | 0 |

### Message Type 7 - HMI Display Update

| Field | Byte(s) | Type | Variable Name | Min | Max |
| ---- | ---- | ---- | ---- | ---- | ---- |
| Message Type | 1-2 | uint16_t | message_type | 7 | 7 |
| Display Page | 3 | uint8_t | display_page | 0 | 5 |
| Display Value | 4-5 | uint16_t | display_value | 0 | 9999 |
| Padding | 6-58 | uint8_t[] | padding | 0 | 0 |

### Message Type 8 - HMI Button Event 

| Field | Byte(s) | Type | Variable Name | Min | Max |
| ---- | ---- | ---- | ---- | ---- | ---- |
| Message Type | 1-2 | uint16_t | message_type | 8 | 8 |
| Button ID | 3 | uint8_t | button_id | 1 | 4 |
| Event | 4 | uint16_t | button_event | 0 | 2 |
| Padding | 5-58 | uint8_t[] | padding | 0 | 0 |

### Message Type 10 - System Status Response

| Field | Byte(s) | Type | Variable Name | Min | Max |
| ---- | ---- | ---- | ---- | ---- | ---- |
| Message Type | 1-2 | uint16_t | message_type | 10 | 10 |
| Status Code | 3 | uint8_t | status_code | 0 | 5 |
| Padding | 4-58 | uint8_t[] | padding | 0 | 0 |

### Message Type 11 - Error Code

| Field | Byte(s) | Type | Variable Name | Min | Max |
| ---- | ---- | ---- | ---- | ---- | ---- |
| Message Type | 1-2 | uint16_t | message_type | 11 | 11 |
| Error Code | 3-4 | uint8_t | error_code | 0 | 999 |
| Padding | 5-58 | uint8_t[] | padding | 0 | 0 |

### Message Type 12 - Emergency Stop

| Field | Byte(s) | Type | Variable Name | Min | Max |
| ---- | ---- | ---- | ---- | ---- | ---- |
| Message Type | 1-2 | uint16_t | message_type | 12 | 12 |
| Padding | 3-58 | uint8_t[] | padding | 0 | 0 |
