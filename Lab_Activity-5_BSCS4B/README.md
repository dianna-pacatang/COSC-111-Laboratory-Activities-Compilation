# Laboratory Activity 5 – Arduino and Python Serial LED Control 🐍🔌

## 📌 Overview
This laboratory activity demonstrates how **Arduino and Python** can communicate through **Serial Connection** to control electronic components. A Python application is used as an external controller that sends commands to Arduino, allowing users to toggle individual LEDs or control them simultaneously through a simple text-based menu.

---

## 🎯 Objectives
- Implement Serial Communication between Arduino and Python
- Utilize Python as a tool for interacting with Arduino hardware
- Develop a command-based LED control system using Serial input

---

## ⚙️ Activity Description
The system consists of an Arduino connected to **three LEDs (Red, Green, and Blue)**. Arduino listens for incoming Serial commands sent by a Python script. Based on the received command, the Arduino toggles a specific LED, turns all LEDs ON, or turns all LEDs OFF.

The Python script runs continuously and presents a menu that allows the user to select LED actions. All inputs are handled in a **case-insensitive** manner.

---

## ✨ Features
- Serial-based communication between Arduino and Python
- Individual LED ON/OFF toggling
- Group LED control (all ON / all OFF)
- Non-terminating Python menu
- Case-insensitive command handling
- Modular Arduino code using a header file

---

## 🧰 Components Used
- Arduino Uno (or compatible board)
- 3 LEDs (Red, Green, Blue)
- 3 Current-limiting resistors
- Breadboard
- Jumper wires
- Laptop with Python and `pyserial`

---

## 🔌 Pin Configuration
| LED Color | Arduino Pin |
|----------|-------------|
| Red | D8 |
| Green | D9 |
| Blue | D10 |

---

## 🔄 Program Flow
1. Arduino initializes Serial communication and waits for commands.
2. Python displays a menu and accepts user input.
3. Python sends a corresponding character to Arduino via Serial.
4. Arduino processes the command and updates LED states.
5. The process repeats until the user exits the Python program.

---

## ▶️ How to Run
### Arduino
1. Upload the Arduino sketch to the board.
2. Ensure the header file is included in the project.

### Python
1. Install required library:
2. Run the Python script.
3. Use the menu options to control the LEDs.

---

## 📘 Learning Outcome
This activity enables students to:
- Integrate Python with Arduino through Serial communication
- Design interactive control systems for hardware
- Apply modular programming practices in embedded systems

---

## 👤 Author
Dianna Jane Elizabeth  
Arduino Laboratory Exercises 🚀

