# 🐟 Real-Time Smart Aquarium Monitoring System

> **Published at IEEE SETCOM 2025**

An IoT-based water quality monitoring system using ESP32 that automates aquatic habitat maintenance through continuous multi-parameter sensing, threshold-based alerts, and cloud dashboard integration.

---

## 📌 Problem Statement

Manual aquarium maintenance is unreliable — water quality parameters like pH, dissolved oxygen, and temperature can shift dangerously within hours. Hobbyists and aquaculture operators lack affordable, automated tools to monitor and respond to these changes in real time.

---

## 💡 Solution

A fully automated IoT monitoring system that continuously tracks four critical water-quality parameters, triggers actuators based on threshold violations, and logs all data to a cloud dashboard for remote monitoring and historical trend analysis.

---

## 🏗️ System Architecture

```
[Water Quality Sensors]
   ├── pH Sensor
   ├── Dissolved Oxygen Sensor
   ├── Temperature Sensor (DS18B20)
   └── Turbidity Sensor
         │
   [ESP32 Microcontroller]
         │
   ├── Real-time threshold evaluation
   ├── Actuator control (pump, heater, aerator)
   └── Wi-Fi data transmission
         │
   [ThingSpeak Cloud]
         └── Live dashboard
         └── Historical trend graphs
         └── Alert notifications
```

---

## ⚙️ Hardware Stack

| Component | Purpose |
|---|---|
| ESP32 | Main microcontroller with Wi-Fi |
| pH Electrode + Amplifier | Water pH monitoring |
| DO Sensor (Gravity) | Dissolved oxygen measurement |
| DS18B20 | Waterproof temperature sensing |
| Turbidity Sensor | Water clarity monitoring |
| Relay Module | Actuator control (pump/heater) |
| OLED Display | Local parameter readout |

---

## 💻 Firmware Features

- **Language:** Embedded C (Arduino Framework)
- **Platform:** ESP32
- Continuous multi-sensor polling
- Real-time threshold-based actuator control
- Alert generation on parameter violations
- Periodic cloud sync to ThingSpeak
- Sensor fusion for correlated parameter analysis

---

## 📊 Monitored Parameters & Thresholds

| Parameter | Safe Range | Action on Violation |
|---|---|---|
| pH | 6.8 – 7.8 | Alert + dosing pump trigger |
| Dissolved Oxygen | > 5 mg/L | Alert + aerator activation |
| Temperature | 24°C – 28°C | Alert + heater control |
| Turbidity | < 100 NTU | Alert + filter pump trigger |

---

## ☁️ Cloud Integration

- **Platform:** ThingSpeak
- Real-time multi-channel data logging
- Live graphs accessible remotely
- Historical data export for trend analysis

---

## 📈 Results

- Extended real-world deployment trials conducted
- Sensor fusion techniques validated across correlated parameters
- Significant reduction in manual inspection effort
- Improved aquatic habitat maintenance accuracy

---

## 📄 Publication

> **"Real Time Smart Aquarium Monitoring System Driven by IoT"**
> IEEE SETCOM 2025
> Covers sensor fusion techniques and system performance benchmarks from extended deployment.

---

## 👤 Author

**Sri Srujan Hari T**
B.E – Electronics & Communication Engineering, BMSIT&M
[LinkedIn](https://www.linkedin.com/in/srujan-hari-undefined-1a7364399) | thammineedisrujanhari@gmail.com
