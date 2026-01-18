# Laboratory Activity 6 – Bidirectional Control Using Arduino and Python 🔁

## 📌 Overview
This laboratory activity demonstrates **bidirectional Serial Communication** between **Arduino and Python**. Unlike previous activities where communication was one-way, this exercise allows **both systems to send and receive data**, enabling real-time interaction between hardware inputs and software responses.

---

## 🎯 Objectives
- Understand and implement bidirectional Serial communication
- Use Python to process incoming data from Arduino
- Control Arduino outputs based on responses sent from Python

---

## ⚙️ Activity Description
The system uses **three push buttons** connected to the Arduino and **three LEDs (Red, Green, Blue)**. When a button is pressed, the Arduino sends a corresponding signal to the Python application. The Python program listens for these signals and immediately sends back a command to the Arduino, which then toggles the appropriate LED.

This interaction demonstrates a **two-way communication loop** between hardware and software.

---

## ✨ Features
- Bidirectional Serial communication between Arduino and Python
- Button-triggered outbound signals from Arduino
- Python-based command processing and response
- LED control based on returned commands
- Edge detection to ensure single signal per button press
- Fast response time (less than 1 second)

---

## 🧰 Components Used
- Arduino Uno (or compatible board)
- 3 LEDs (Red, Green, Blue)
- 3 Push Buttons
- Current-limiting resistors
- Breadboard
- Jumper wires
- Laptop with Python and `pyserial`

---

## 🔌 Pin Configuration

### LEDs
| LED Color | Arduino Pin |
|----------|-------------|
| Red | D7 |
| Green | D6 |
| Blue | D5 |

### Buttons
| Button | Arduino Pin |
|--------|-------------|
| Button 1 | D12 |
| Button 2 | D11 |
| Button 3 | D10 |

---

## 🔄 Program Flow
1. Arduino monitors button presses using edge detection.
2. When a button is pressed, Arduino sends a single character (`R`, `G`, or `B`) via Serial.
3. Python listens for incoming Serial data from Arduino.
4. Upon receiving the signal, Python sends a numeric command (`1`, `2`, or `3`) back to Arduino.
5. Arduino receives the command and toggles the corresponding LED.

---

## ▶️ How to Run
### Arduino
1. Upload the Arduino sketch and ensure the header file is included.
2. Connect LEDs and buttons according to the pin configuration.

### Python
1. Install required dependency:
2. Update the COM port in the script if necessary.
3. Run the Python program and press the buttons to observe LED responses.

---

## 📘 Learning Outcome
After completing this activity, students will be able to:
- Implement two-way communication between Arduino and Python
- Handle real-time data exchange between hardware and software
- Design responsive embedded systems with external software control

---

## 👤 Author
Dianna Jane Elizabeth  
Arduino Laboratory Exercises 🚀

