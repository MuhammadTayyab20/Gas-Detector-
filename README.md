# Gas Detector 🚨

An Arduino-based gas detection system that continuously monitors the surrounding air for harmful gases — ammonia, CO₂, benzene, alcohol, and smoke — and triggers an audible alarm when the concentration crosses a safe threshold.

---

## 🔧 How It Works

A gas sensor (MQ-series) constantly reads the gas concentration in the air. The Arduino compares each reading against a defined safe limit. When the reading exceeds that limit, the Arduino activates a buzzer to warn anyone nearby of a potential gas leak or unsafe air quality.

---

## 🧰 Components Used

- Arduino Uno (or compatible board)
- MQ-series gas sensor (MQ-135) 
- Buzzer 
- Breadboard + jumper wires
- USB cable / power supply

---



## ▶️ Getting Started

1. Open the `.ino` sketch in the **Arduino IDE**.
2. Connect the components as per the wiring table.
3. Select your board and port under **Tools**.
4. Click **Upload**.
5. Open the **Serial Monitor** to watch live sensor readings.

---

## 🎚️ Calibration

The alarm threshold is set in the code as a fixed value. Let the sensor warm up for a minute or two on first power-up, note the baseline reading in clean air, then set the threshold slightly above that baseline.

---

## 🛠️ Tech

- **Language:** C++ (Arduino)
- **Platform:** Arduino IDE

---

## 📌 Possible Improvements

- [ ] Add an LCD/OLED display to show live readings
- [ ] Add Wi-Fi (ESP32) alerts to a phone
- [ ] Log readings over time
- [ ] Multiple gas-specific sensors
