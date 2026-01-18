# Laboratory Activity 7 – Controlling Arduino Using FastAPI 🌐🔌

## 📌 Overview
This laboratory activity demonstrates how **Arduino hardware can be controlled through HTTP requests** using **FastAPI**. The project integrates **Serial Communication** and **web-based APIs**, allowing LED control on an Arduino board through REST endpoints accessed via a browser or API client.

This activity introduces a **network-based control approach**, commonly used in IoT systems, where hardware devices are managed remotely using web technologies.

---

## 🎯 Objectives
- Implement Arduino Serial Communication
- Utilize Python and FastAPI to create an HTTP-based control system
- Control Arduino outputs through REST API endpoints

---

## ⚙️ Activity Description
The system consists of an Arduino connected to **three LEDs (Red, Green, Blue)**. Arduino listens for commands sent through Serial Communication. A **FastAPI server** running on Python exposes endpoints that translate HTTP requests into Serial commands, which are then processed by the Arduino to control the LEDs.

Each API endpoint corresponds to a specific LED action, such as toggling individual LEDs or turning all LEDs ON or OFF.

---

## ✨ Features
- RESTful API for controlling Arduino LEDs
- Integration of FastAPI with Serial Communication
- Individual LED control through URL parameters
- Group LED control (all ON / all OFF)
- Case-insensitive command handling on the Arduino side
- Real-time response to HTTP requests

---

## 🧰 Components Used
- Arduino Uno (or compatible board)
- 3 LEDs (Red, Green, Blue)
- Current-limiting resistors
- Breadboard
- Jumper wires
- Laptop with Python, FastAPI, and `pyserial`

---

## 🔌 Pin Configuration
| LED Color | Arduino Pin |
|----------|-------------|
| Red | D7 |
| Green | D6 |
| Blue | D5 |

---

## 🌐 API Endpoints

### `GET /led/{color}`
- `{color}` can be `red`, `green`, or `blue`
- Sends the corresponding Serial command to toggle the selected LED

### `GET /led/on`
- Turns all LEDs ON

### `GET /led/off`
- Turns all LEDs OFF

---

## 🔄 Program Flow
1. FastAPI receives an HTTP request from the client.
2. Python sends a corresponding command to Arduino via Serial.
3. Arduino processes the command and updates LED states.
4. Arduino sends status messages back through Serial (optional).

---

## ▶️ How to Run
### Arduino
1. Upload the Arduino sketch and ensure the header file is included.
2. Connect LEDs according to the pin configuration.

### FastAPI (Python)
1. Install required dependencies:
2. Update the COM port in the Python file if necessary.
3. Start the FastAPI server:
4. Access the API endpoints using a browser or API client.

---

## 📘 Learning Outcome
This activity allows students to:
- Apply web technologies to embedded systems
- Understand REST-based hardware control
- Integrate Arduino with modern backend frameworks
- Build foundational IoT-style applications

---

## 👤 Author
Dianna Jane Elizabeth  
Arduino Laboratory Exercises 🚀
