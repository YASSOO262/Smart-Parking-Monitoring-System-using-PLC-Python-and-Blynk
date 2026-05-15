
# Smart Parking Monitoring System using PLC, Python, and Blynk

This project implements a real-time Smart Parking Monitoring System using an Allen-Bradley PLC, Python, RSLinx DDE communication, and the Blynk IoT Platform cloud dashboard. The system is designed to monitor parking availability, vehicle movement, parking lights, and system status remotely through a mobile and web dashboard.

The PLC ladder logic controls the parking system operation using input sensors, counters, timers, and internal control bits. Python acts as a bridge between the PLC and the Blynk cloud platform by continuously reading PLC tags through RSLinx using DDE communication and sending the data to Blynk virtual pins using HTTP API requests.

The system monitors:

* Start and Stop push buttons
* Vehicle entry and exit sensors
* Parking spot availability
* Parking status LEDs
* Parking light status
* Master control coil status
* Total vehicle count inside the parking area

The dashboard provides a real-time visualization interface that displays parking status and system operation remotely. LEDs and gauges are used to represent parking occupancy and system conditions dynamically.

## Technologies Used

* Python
* Allen-Bradley PLC
* RSLogix 500
* RSLinx Classic
* DDE Communication
* Blynk IoT Platform
* HTTP API
* Ladder Logic Programming

## Features

* Real-time PLC monitoring
* Remote IoT dashboard visualization
* Vehicle counting system
* Parking occupancy indication
* Cloud-based monitoring using Blynk
* Master system status monitoring
* Safe PLC tag reading with error handling

## System Workflow

1. Sensors and push buttons are connected to the PLC.
2. PLC ladder logic processes parking conditions and vehicle counting.
3. Python reads PLC memory addresses through RSLinx DDE.
4. Data is transmitted to Blynk Cloud using API requests.
5. The dashboard updates in real time to display system status.

This project demonstrates the integration of industrial automation with IoT technologies for smart monitoring applications.
