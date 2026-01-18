# Laboratory Activity 3 – Fire Detection Using Thermistor and Photoresistor 🔥

## 📌 Overview
This laboratory activity focuses on integrating **basic sensors commonly used in IoT systems** to create a simple **fire detection prototype**. The system combines temperature sensing using a **thermistor** and light sensing using a **photoresistor (LDR)**. When both sensor readings reach their defined limits, an alert is triggered using an LED and a speaker.

---

## 🎯 Objectives
- Become familiar with basic sensor components used in IoT applications
- Integrate multiple sensors into an Arduino-based circuit
- Implement a simple fire detection logic using sensor thresholds

---

## ⚙️ Activity Description
The Arduino continuously monitors temperature and brightness levels through analog inputs. Temperature values are converted to **degrees Celsius**, while brightness values are read as analog signals. A fire condition is detected only when **both temperature and brightness thresholds are satisfied**, ensuring more reliable detection.

Once a fire condition is identified, the system activates an LED and a speaker to notify the user.

---

## ✨ Features
- Temperature sensing using a thermistor with Celsius conversion
- Brightness detection using a photoresistor (LDR)
- Dual-threshold fire detection logic
- Alert system using LED and speaker
- Modular code structure with separate functions for sensor readings
- Use of `#define` for pin assignments and `const` for threshold values
- Real-time sensor monitoring via Serial Monitor

---

## 🧰 Components Used
- Arduino Uno (or compatible board)
- Thermistor with resistor (voltage divider)
- Photoresistor (LDR) with resistor
- LED (fire indicator)
- Speaker / Buzzer
- Breadboard
- Jumper wires

---

## 🔌 Pin Configuration
| Component | Arduino Pin |
|----------|-------------|
| Thermistor | A0 |
| Photoresistor (LDR) | A2 |
| LED | D12 |
| Speaker | D11 |

---

## 📏 Threshold Values
| Parameter | Value |
|---------|-------|
| Temperature Threshold | 50°C |
| Brightness Threshold | 220 |

---

## 🔄 Program Flow
1. The thermistor reading is converted into temperature (Celsius).
2. The photoresistor provides brightness values through analog input.
3. Sensor values are displayed on the Serial Monitor.
4. If **both threshold conditions are met**, the alert system is activated.
5. The alert remains inactive when conditions are not satisfied.

---

## ▶️ How to Run
1. Assemble the circuit based on the pin configuration.
2. Upload the Arduino sketch to the board.
3. Open the Serial Monitor at **9600 baud**.
4. Simulate increased heat and reduced brightness to trigger the alert.

---

## 📘 Learning Outcome
This activity helps students understand:
- Sensor integration and analog signal processing
- Multi-condition decision logic in embedded systems
- Modular programming practices for Arduino projects

---

## 👤 Author
Dianna Jane Elizabeth  
Arduino Laboratory Exercises 🚀

