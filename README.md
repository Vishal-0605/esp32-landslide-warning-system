# Smart Landslide Warning System with Wi-Fi Integration

An ESP32-based IoT prototype for monitoring ground conditions using motion, vibration, and soil-moisture sensors, with remote data logging and Telegram notifications.

## Project Overview

Landslides can cause significant damage to life, infrastructure, and property. This project presents a prototype that monitors selected ground conditions and notifies users when sensor readings indicate a possible landslide risk.

The system uses an ESP32 to collect data from an MPU6050 accelerometer and gyroscope, an SW-420 vibration sensor, and a soil-moisture sensor. Wi-Fi connectivity supports Telegram notifications and Google Sheets logging.

**Project type:** IoT, Embedded Systems, Environmental Monitoring  
**Controller:** ESP32  
**Project status:** Prototype documented; original firmware files need to be recovered or reconstructed.

## Objectives

- Monitor soil moisture, vibration, and ground movement.
- Read sensor measurements using the ESP32.
- Compare measurements against predefined threshold limits.
- Send Telegram notifications when abnormal readings indicate a potential risk.
- Record sensor measurements in Google Sheets for remote monitoring and subsequent analysis.

## System Architecture

The system follows this general workflow:

1. Power on the ESP32 and initialize the connected sensors.
2. Read sensor measurements at regular intervals.
3. Evaluate the readings against configured threshold limits.
4. Identify potential risk conditions based on abnormal moisture, vibration, or tilt readings.
5. Send a Telegram alert through Wi-Fi when a risk condition is detected.
6. Log sensor data in Google Sheets for monitoring and analysis.
7. Repeat the monitoring cycle.

## Hardware Components

| Component | Purpose |
|---|---|
| ESP32 | Main controller and Wi-Fi connectivity |
| MPU6050 | Measures three-axis acceleration and angular velocity |
| SW-420 vibration sensor | Detects vibration or sudden shocks |
| Soil-moisture sensor | Provides an analog measurement related to soil moisture |
| Connecting wires and breadboard | Sensor interfacing and prototype assembly |

## Software and Connectivity

- **Embedded firmware:** ESP32 sensor acquisition and monitoring logic
- **Sensor communication:** I²C for the MPU6050
- **Wireless connectivity:** Wi-Fi
- **Notifications:** Telegram Bot API
- **Data logging:** Google Sheets

The exact development environment, firmware implementation, and library versions should be added after the original source files or reconstructed code have been verified.

## Monitoring and Notifications

The prototype monitors sensor readings and checks for abnormal conditions. When a configured risk condition is detected, the intended workflow sends a Telegram alert. Sensor measurements can also be recorded in Google Sheets to support remote monitoring and review.

The system is a prototype, not a certified landslide prediction or safety system. Its effectiveness depends on sensor placement, threshold calibration, environmental conditions, connectivity, and testing.


## Repository Contents

The repository is being organized to include:

- `README.md` — Project overview and documentation
- `firmware/` — ESP32 source code (to be recovered or reconstructed and tested)
- `docs/` — Block diagrams, technical documentation, and supporting material


The folders and firmware files will be added as they become available.

## Future Improvements

- Recover and document the original ESP32 firmware.
- Calibrate the sensors and document the threshold values used.
- Add sensor validation and handling for communication failures.
- Improve the alert logic and record alert events alongside sensor measurements.
- Evaluate the prototype under controlled test conditions.
- Add a dashboard for visualizing historical sensor measurements.

## Team

Project developed as a student team project.

## Disclaimer

This prototype is intended for educational and experimental use. It must not be used as the sole basis for landslide warnings, evacuation decisions, or other safety-critical actions.
