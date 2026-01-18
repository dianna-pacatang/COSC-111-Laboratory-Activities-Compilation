# Laboratory Activity 1 – Arduino Running Light (Digital Output) 💡

## 📌 Overview
This laboratory activity introduces the Arduino platform as a basic tool for **IoT and embedded system development**. The exercise focuses on **digital output control** by creating a running light effect using multiple LEDs connected to the Arduino. The activity demonstrates how digital signals can be used to control external components in a sequential manner.

---

## 🎯 Objectives
- Introduce Arduino as a device used in IoT implementations
- Apply digital signal concepts using Arduino digital output pins

---

## ⚙️ Activity Description
The system uses **five LEDs** connected to digital pins **12, 11, 10, 9, and 8** of the Arduino. An array is used to store the pin numbers, allowing the LEDs to be controlled efficiently. The LEDs turn **ON one at a time** from pin 12 down to pin 8, followed by turning **OFF in the same sequence**, with a **1-second delay** between each change.

---

## ✨ Features
- Sequential LED running light pattern
- Digital control using `digitalWrite()`
- Use of arrays for pin management
- Loop-based implementation for scalability

---

## 🧰 Components Used
- Arduino Uno (or compatible board)
- 5 LEDs
- 5 Current-limiting resistors (220Ω–330Ω)
- Breadboard
- Jumper wires

---

## 🔌 Pin Configuration
| LED | Arduino Pin |
|-----|-------------|
| LED 1 | D12 |
| LED 2 | D11 |
| LED 3 | D10 |
| LED 4 | D9 |
| LED 5 | D8 |

---

## 🔄 Program Flow
1. LED pins are stored in an array.
2. All pins are configured as outputs during setup.
3. LEDs are turned ON sequentially with a 1-second delay.
4. After all LEDs are ON, they are turned OFF sequentially.
5. The sequence repeats continuously.

---

## ▶️ How to Run
1. Assemble the circuit according to the pin configuration.
2. Upload the Arduino sketch to the board.
3. Power the Arduino and observe the running light pattern.

---

## 📘 Learning Outcome
Through this activity, students gain an understanding of:
- Digital output signaling in Arduino
- Efficient pin handling using arrays
- Basic sequencing logic used in IoT applications

---

## 👤 Author
Dianna Jane Elizabeth  
Arduino Laboratory Exercises 🚀

