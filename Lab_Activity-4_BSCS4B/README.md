# Laboratory Activity 4 – Serial-Controlled Persistent Alert 💻🔔

## 📌 Overview
This laboratory activity introduces **Arduino Serial Communication** as a method for controlling hardware behavior through user input. The project demonstrates how sensor-triggered actions can be **maintained persistently** and later controlled using commands entered through the **Serial Monitor**. The activity highlights the use of serial input to override and manage system behavior.

---

## 🎯 Objectives
- Understand and apply Arduino Serial Communication
- Explore basic serial functions for user interaction
- Develop a simple circuit that can be controlled through Serial input

---

## ⚙️ Activity Description
The system monitors a selected sensor value and activates a **blinking LED alert** once a predefined threshold is reached. After activation, the LED continues blinking even if the sensor reading falls below the threshold. The blinking process can only be stopped by entering a specific command (`stop`) through the Serial Monitor.

All Serial inputs are handled in a **case-insensitive** manner to improve usability.

---

## ✨ Features
- Sensor-based trigger for LED blinking
- Persistent alert behavior once activated
- Serial command control to stop the alert
- Case-insensitive command handling
- State tracking using boolean variables
- Real-time feedback via Serial Monitor

---

## 🧰 Components Used
- Arduino Uno (or compatible board)
- Sensor (thermistor or photoresistor)
- LED
- Current-limiting resistor
- Breadboard
- Jumper wires

---

## 🔌 Pin Configuration
| Component | Arduino Pin |
|----------|-------------|
| Sensor | A0 / A2 |
| LED | D8 |

---

## 🔄 Program Flow
1. The Arduino reads sensor input continuously.
2. When the sensor value reaches the defined threshold, LED blinking is activated.
3. The blinking state remains active even if the sensor value decreases.
4. The Serial Monitor listens for user commands.
5. Entering the command `stop` disables the blinking alert.

---

## ▶️ How to Run
1. Assemble the circuit according to the pin configuration.
2. Upload the Arduino sketch to the board.
3. Open the Serial Monitor and set the baud rate to **9600**.
4. Trigger the sensor threshold to start the blinking alert.
5. Type `stop` to halt the blinking behavior.

---

## 📘 Learning Outcome
After completing this activity, students will be able to:
- Use Serial input to control Arduino behavior
- Implement persistent system states
- Manage hardware output using user commands
- Apply logical conditions in embedded applications

---

## 👤 Author
Dianna Jane Elizabeth  
Arduino Laboratory Exercises 🚀
