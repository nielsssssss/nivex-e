# Nivex-E – Electric Motorcycle

![Nivex-E Moped](docs/images/moped.JPEG)

Nivex-E is a student-built electric moped developed as part of a diploma project at HTBLuVA Salzburg.  
The project focuses on converting a conventional combustion-powered motorcycle into a fully electric vehicle, combined with a modern and intelligent Human-Machine Interface (HMI).

---

## Project Overview

The main goal of Nivex-E is to create a reliable, efficient, and user-friendly electric mobility solution.  
In addition to the mechanical and electrical conversion, a strong focus was placed on the development of a modern embedded system architecture.

The system combines:

- Real-time data acquisition via **CAN bus**
- Embedded control using microcontrollers
- A **Raspberry Pi 5** for visualization and high-level processing
- A responsive **web-based user interface**

This allows the rider to monitor important parameters such as speed, battery status, power consumption, and range in real time.

---

## System Architecture

The system is built around a distributed architecture:

- **Raspberry Pi 5**
  - Processes incoming CAN data
  - Hosts a WebSocket server
  - Runs the graphical user interface (HTML, CSS, JavaScript)

- **RP2040 Microcontroller (Feather)**
  - Handles real-time inputs (buttons, sensors)
  - Sends and receives CAN messages
  - Acts as a bridge between hardware and higher-level systems

- **CAN Bus**
  - Ensures robust and reliable communication between all system components
  - Enables modular expansion of the system

- **Battery Management System (BMS)**
  - Provides battery data via CAN communication
  - Ensures safe operation of the battery pack

---

## Features

- Real-time speed and vehicle data display  
- Battery monitoring (voltage, current, state of charge)  
- Range estimation  
- Driving mode visualization (ECO, COMFORT, SPORT, INSANE)  
- Web-based UI optimized for touch display  
- Modular CAN-based communication system  

---

## Repository Contents

- Python backend for CAN communication and data processing  
- Web interface (HTML / CSS / JavaScript)  
- RP2040 firmware  
- Configuration files and system scripts  
- Documentation of system architecture and data flow  

---

## Technologies Used

- Python (SocketCAN, WebSockets)  
- HTML, CSS, JavaScript  
- C/C++ (RP2040 firmware)  
- CAN Bus (SocketCAN)  
- Raspberry Pi OS  

---

## Team

This project was developed by:

- Dominik Nachbar  
- Patrick Unger  
- Niels Steinböck  

---

## Acknowledgements

Special thanks to:

- Josef Diemling  
- Gerhard Egger  
- Reinhold Benedikter  
- Franz Reich  

as well as the highly supportive workshop team.

Their guidance, support, and resources made this project possible.

---

## Note

This repository contains the software part of the Nivex-E project.  
Mechanical construction, electrical integration, and full system documentation are part of the diploma thesis.
