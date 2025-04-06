# 🚗💡 Multifunctional Vehicle Safety & Security System using IoT

> 🚘 Empowering safer roads with smart IoT-based vehicle safety.  
> 🎓 Final Year Project | Computer Science & Engineering | East West Institute of Technology (2024-25)

A smart, sensor-driven system built on **ESP32** microcontroller that proactively detects driving hazards and sends real-time alerts. The system enhances road safety by integrating multiple sensors (alcohol, tilt, ultrasonic, LDR, IR) and communication modules (Bluetooth, Telegram Bot) to assist drivers and ensure quick emergency response.

---

## 🧭 Table of Contents

- [🚀 Introduction](#-introduction)
- [✨ Features](#-features)
- [🛠️ System Architecture](#-system-architecture)
- [🧩 Hardware & Software Requirements](#-hardware--software-requirements)
- [⚙️ Implementation](#-implementation)
- [📊 Results & Insights](#-results--insights)
- [💻 Installation](#-installation)
- [🚦 Usage](#-usage)
- [🤝 Contributing](#-contributing)
- [📝 License](#-license)

---

## 🚀 Introduction

Modern vehicles need modern safety solutions.  
This project introduces an integrated **Multifunctional Vehicle Safety System**, designed to:
- Prevent accidents 🚑
- Detect unsafe driving behaviors 🍷
- Monitor vehicle surroundings 🧭
- Provide real-time alerts and emergency communication 📲

By leveraging IoT technology and ESP32’s processing power, we aim to create safer driving environments and smarter vehicles.

---

## ✨ Features

✅ **High Beam Detection**  
Automatically adjusts headlights to reduce glare from oncoming traffic.

✅ **Accident Detection**  
Detects vehicle tilt or collision and instantly sends emergency location via Telegram.

✅ **Alcohol Detection**  
Monitors driver's breath for alcohol content and prevents vehicle ignition if unsafe.

✅ **Blind Spot & Object Monitoring**  
Ultrasonic sensors alert the driver of nearby obstacles and blind spots.

✅ **One-Handed Driving Detection**  
IR sensors detect unsafe posture and trigger alerts.

✅ **Real-time Alerts**  
Bluetooth voice notifications and Telegram emergency messages with GPS data.

✅ **GPS Tracking**  
Live vehicle location sharing for emergencies.

---

## 🛠️ System Architecture

```plaintext
[Sensors (LDR, Alcohol, Tilt, IR, Ultrasonic)]
            │
            ▼
[ESP32 Microcontroller] — Processes sensor data
            │
            ├─> [LCD Display] — Visual Alerts
            ├─> [Bluetooth Module] — Voice Alerts
            ├─> [Telegram Bot] — Emergency Notifications
            └─> [Relay & Buzzer] — Safety Actions

## 🧩 Hardware & Software Requirements

## 🔌 Hardware
ESP32 Microcontroller
Ultrasonic Sensors
Tilt Sensor (ADXL345)
MQ-3 Alcohol Sensor
IR Sensors
Light Dependent Resistor (LDR)
Relay Module & Buzzer
LCD Display
Bluetooth Module
Power Supply, Jumper Wires, Breadboard
## 🖥️ Software
Arduino IDE
Arduino Libraries:
LiquidCrystal_I2C
Wire
Adafruit_Sensor
Adafruit_ADXL345_U
WiFi
UniversalTelegramBot
ArduinoJson
Telegram Bot API
Wi-Fi Connection
##⚙️ Implementation

--
Sensor Integration
Sensors continuously monitor environment and driver behavior.
Data Processing with ESP32
Real-time data handling and decision making.
Alerts & Communication
Triggering visual, sound, and message alerts in critical situations.
Vehicle Control
If hazardous conditions are detected, the system disables vehicle ignition.
--

📊 Results & Insights

✅ Successfully detects:

High beam glare
Alcohol consumption
One-handed driving
Blind spots and obstacles
Accident scenarios
✅ Real-time alerts reduce reaction time and enable faster emergency responses.
--
💻 Installation

Clone the Repository
git clone https://github.com/yourusername/vehicle-safety-system.git
cd vehicle-safety-system
Install Dependencies
Use Arduino Library Manager to install required libraries.
Configure Credentials Update your Wi-Fi and Telegram bot details in the code:
const char* ssid = "Your_SSID";
const char* password = "Your_PASSWORD";
#define BOTtoken "Your_Telegram_Bot_Token"
#define CHAT_ID "Your_Chat_ID"
Connect Hardware & Upload Code Assemble the circuit and upload the code to your ESP32.
--

🚦 Usage

Power the ESP32 microcontroller and connected modules.
Monitor alerts on:
LCD display
Bluetooth audio notifications
Telegram messages
Test different scenarios for comprehensive safety monitoring.
