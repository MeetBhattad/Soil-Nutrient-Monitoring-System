# 🌱 Soil Nutrient Monitoring System using ESP32 and NPK Sensor

An IoT-based soil nutrient monitoring system that measures **Nitrogen (N), Phosphorus (P), and Potassium (K)** levels in soil using an RS485 NPK sensor. The collected data is processed by an ESP32 and displayed on a real-time web dashboard over Wi-Fi.

---

## 📌 Overview

This project helps users monitor soil nutrient levels without traditional laboratory testing. The ESP32 creates a Wi-Fi Access Point and hosts a web dashboard where users can view real-time NPK values from any smartphone or laptop connected to the ESP32 network.

---

## ✨ Features

- Real-time NPK monitoring
- ESP32 Wi-Fi Access Point (AP Mode)
- Web-based dashboard
- RS485 communication using MAX485
- Modbus RTU protocol
- Portable and low-cost design

---

## 🛠 Hardware Used

- ESP32 Development Board
- RS485 Soil NPK Sensor
- MAX485 RS485 to TTL Converter
- 12V Power Supply
- Jumper Wires

---

## 💻 Software Used

- Arduino IDE
- ESP32 Board Package
- Embedded HTML/CSS/JavaScript
- Modbus RTU Communication

---

## 🔄 System Architecture

```

Soil
│
▼
NPK Sensor
│
▼
RS485 Communication
│
▼
MAX485 Module
│
▼
ESP32
│
▼
Wi-Fi Access Point
│
▼
Web Dashboard

```

---

## 🔌 Pin Connections

| ESP32 | MAX485 |
|--------|---------|
| GPIO16 (RX2) | RO |
| GPIO17 (TX2) | DI |
| GPIO4 | DE |
| GPIO5 | RE |
| 5V | VCC |
| GND | GND |

### NPK Sensor

| Sensor | MAX485 |
|---------|---------|
| A | A |
| B | B |

Sensor Power: **12V DC**

---

## ⚙ Working

1. ESP32 sends Modbus commands through MAX485.
2. MAX485 converts TTL signals to RS485.
3. NPK sensor measures soil nutrients.
4. Sensor returns Nitrogen, Phosphorus and Potassium values.
5. ESP32 receives the data.
6. ESP32 hosts a web server.
7. Users connect to the ESP32 Wi-Fi and open the dashboard.
8. Live NPK values are displayed.

---

## 📸 Dashboard

(Add a screenshot here)

```
images/dashboard.png
```

---

## 📁 Project Structure

```

Soil-Nutrient-Monitoring-System
│
├── NPK_ESP32.ino
├── README.md
├── images
│   ├── dashboard.png
│   ├── hardware.jpg
│   └── block_diagram.png
├── circuit
│   └── circuit_diagram.png
└── docs
├── Project_Report.pdf
└── Presentation.pdf

```

---

## 🚀 Future Improvements

- Cloud connectivity
- Mobile application
- Data logging
- Automatic fertilizer recommendation
- Integration with irrigation systems

---

## 📚 Skills Demonstrated

- Embedded Systems
- ESP32 Programming
- C++
- UART Communication
- RS485
- Modbus RTU
- Web Server Development
- HTML/CSS/JavaScript
- IoT

---

## 👨‍💻 Author

**Meet Bhattad**

Electronics & Telecommunication Engineering

Mini Project
