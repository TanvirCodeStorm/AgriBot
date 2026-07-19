<div align="center">

# 🌱 AgriBot
### Smart Automated Irrigation & Fertilizer Distribution System

**Developed by Tanvir Hussain**

*An Arduino-based smart farming project that monitors soil moisture, automates irrigation, controls water distribution using a servo mechanism, and provides manual fertilizer dispensing.*

---

![Arduino](https://img.shields.io/badge/Arduino-Uno-blue?style=for-the-badge&logo=arduino)
![Sensor](https://img.shields.io/badge/Soil-Moisture-green?style=for-the-badge)
![Relay](https://img.shields.io/badge/Relay-Control-red?style=for-the-badge)
![Servo](https://img.shields.io/badge/Servo-30°--120°-orange?style=for-the-badge)


</div>

---

# 📖 Overview

AgriBot is an **Arduino-powered smart irrigation system** designed to automate watering based on real-time soil moisture levels.

The project continuously measures soil moisture using an **Arduino Soil Moisture Sensor**. When the soil becomes dry, the system automatically:

- 💧 Turns ON a **5V DC Water Pump**
- 🔄 Rotates a **Servo Motor** from **30° to 120°**
- 🚿 Sprinkles water evenly through a pipe
- 🛑 Stops irrigation automatically when sufficient moisture is detected

Additionally, the system includes a **manual fertilizer dispensing mechanism** controlled through a **push button**, allowing fertilizer to be released whenever required.

---

# ✨ Features

- 🌱 Real-time soil moisture monitoring
- 💧 Automatic irrigation
- 🔌 Relay-controlled 5V DC water pump
- 🔄 Servo-based water distribution
- 🚿 Uniform sprinkler movement
- 🌾 Manual fertilizer release system
- 🔘 Push-button fertilizer pump control
- ⚡ Low-cost and easy to build
- 🔧 Arduino compatible

---

# 🛠 Components Required

| Component | Quantity |
|-----------|---------:|
| Arduino UNO | 1 |
| Soil Moisture Sensor | 1 |
| 5V Relay Module | 2 |
| 5V DC Water Pump | 2 |
| Servo Motor (SG90/MG90S) | 1 |
| Push Button | 1 |
| Pipes/Sprinkler | 1 |
| Jumper Wires | Several |
| Breadboard / PCB | 1 |
| Power Supply | 5V |

---

# ⚙ Working Principle

```text
                Soil Moisture Sensor
                         │
                         ▼
                  Arduino UNO
                         │
          ┌──────────────┴──────────────┐
          │                             │
          ▼                             ▼
      Relay Module                  Servo Motor
          │                             │
          ▼                             ▼
     Water Pump                  30° ↔ 120°
          │                             │
          └──────────────┬──────────────┘
                         ▼
                Water Sprinkler Pipe

Push Button ─────► Relay ─────► Fertilizer Pump
```

---

# 🔄 System Workflow

```text
        Start
          │
          ▼
 Read Soil Moisture
          │
          ▼
Is Soil Dry?
   │            │
 Yes           No
   │            │
   ▼            ▼
Turn ON Pump   Pump OFF
   │
   ▼
Servo Moves
30° → 120°
   │
   ▼
Sprinkle Water
   │
   ▼
Read Sensor Again
   │
   ▼
Enough Moisture?
   │           │
 No           Yes
 │             │
 └──────┐      ▼
        │   Stop Pump
        │   Servo Reset
        ▼
      Repeat
```

---

# 🌿 Fertilizer System

A dedicated fertilizer dispensing system is included.

### Operation

- Press the push button.
- Relay activates.
- Fertilizer pump turns ON.
- Fertilizer flows through the delivery pipe.
- Release or press again (depending on implementation) to stop the pump.

This system operates independently from the automatic irrigation mechanism.

---

# 🔌 Pin Connections

| Arduino Pin | Connected Device |
|-------------|-----------------|
| A0 | Soil Moisture Sensor |
| D7 | Water Pump Relay |
| D9 | Servo Motor |
| D8 | Fertilizer Pump Relay |
| D2 | Push Button |

*(Pins can be modified according to the Arduino code.)*

---

# 🚿 Irrigation Logic

```text
Dry Soil
   │
   ▼
Relay ON
   │
   ▼
Water Pump ON
   │
   ▼
Servo rotates
30°
 ↓
45°
 ↓
60°
 ↓
75°
 ↓
90°
 ↓
105°
 ↓
120°
   │
   ▼
Water spreads uniformly
```

---

# 📊 Project Architecture

```text
             +----------------------+
             |  Soil Moisture Sensor|
             +----------+-----------+
                        |
                        |
                        ▼
                +---------------+
                | Arduino UNO   |
                +-------+-------+
                        |
        +---------------+---------------+
        |                               |
        ▼                               ▼
  Relay Module                    Servo Motor
        |                               |
        ▼                               ▼
  Water Pump                 Water Distribution
                                      |
                                      ▼
                               Sprinkler Pipe

Push Button
      │
      ▼
Relay Module
      │
      ▼
Fertilizer Pump
```

---

# 💻 Software

- Arduino IDE
- Embedded C / Arduino Language

---

# 📈 Advantages

- Saves water
- Fully automatic irrigation
- Uniform water distribution
- Low maintenance
- Low power consumption
- Affordable hardware
- Easy to expand
- Beginner-friendly Arduino project

---

# 🚀 Future Improvements

- 📶 IoT Monitoring
- ☁ Cloud Integration
- 📱 Mobile App Control
- 🌦 Weather Forecast Integration
- 🌡 Temperature & Humidity Sensor
- 📊 Data Logging
- 🌍 Solar Power
- 📍 GPS-based Farm Mapping
- 🤖 AI-based Irrigation Prediction

---

# 📷 Project Preview

```
          _______________________

           🌱        🌱        🌱
            |         |         |
        ----------------------------
             Water Sprinkler Pipe
                  ↔ Servo

                 💧💧💧💧💧

              5V Water Pump

                    │
                Relay Module

                    │
               Arduino UNO

                    │
         Soil Moisture Sensor

-----------------------------------------

      Push Button
            │
            ▼
      Relay Module
            │
            ▼
     Fertilizer Pump
```

---

# 📚 Applications

- Smart Farming
- Home Gardens
- Greenhouses
- Nurseries
- Vegetable Farms
- Indoor Plant Irrigation
- Agricultural Research

---

# 👨‍💻 Author

## **Tanvir Hussain**

**Project:** AgriBot

Smart Automated Irrigation & Fertilizer Distribution System using Arduino.

---

# 📜 Poject

This project is open-source and was developed by Tanvir Hussain for his school exhibition in 2024.

---

<div align="center">

### ⭐ If you found this project useful, please give it a Star ⭐

**Made with ❤️ by Tanvir Hussain**

</div>
