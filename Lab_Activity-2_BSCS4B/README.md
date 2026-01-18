# Laboratory Activity 2 – Running Light with PWM Brightness Control 🌈

## 📌 Overview
This laboratory activity builds upon the digital running light circuit from the previous exercise by introducing **analog signal behavior** in Arduino. The activity demonstrates how **Pulse Width Modulation (PWM)** can be used to control LED brightness using the `analogWrite()` function. Emphasis is placed on structured programming using **arrays** and **`while()` loops**.

---

## 🎯 Objectives
- Understand analog signal implementation in Arduino
- Apply PWM concepts using `analogWrite()`
- Practice structured looping using `while()` and arrays

---

## ⚙️ Activity Description
The system consists of **five LEDs** connected to Arduino pins **12, 11, 10, 9, and 8**. Each LED is assigned a predefined brightness value stored in an array. The LEDs turn **ON sequentially** with their corresponding brightness levels applied, followed by turning **OFF sequentially**, each with a **1-second delay**.

---

## ✨ Features
- PWM-based LED brightness control
- Individual brightness values per LED
- Uses `analogWrite()` for output control
- Array-based pin and brightness management
- Looping logic implemented using `while()` loops

---

## 🧰 Components Used
- Arduino Uno (or compatible board)
- 5 LEDs
- 5 Current-limiting resistors (220Ω–330Ω)
- Breadboard
- Jumper wires

---

## 🔌 Pin and Brightness Configuration
| LED | Arduino Pin | Brightness (PWM) |
|-----|-------------|------------------|
| LED 1 | D12 | 255 |
| LED 2 | D11 | 20 |
| LED 3 | D10 | 80 |
| LED 4 | D9  | 100 |
| LED 5 | D8  | 150 |

> ⚠️ Note: PWM brightness control works properly only on PWM-capable pins. LEDs connected to non-PWM pins may behave as simple ON/OFF outputs.

---

## 🔄 Program Flow
1. LED pin numbers and brightness levels are stored in arrays.
2. All LED pins are configured as outputs using a `while()` loop.
3. LEDs are activated one by one using their assigned brightness values.
4. LEDs are then turned OFF sequentially.
5. The sequence repeats continuously.

---

## ▶️ How to Run
1. Assemble the circuit based on the pin configuration table.
2. Upload the sketch to the Arduino board.
3. Observe the running light pattern with varying brightness levels.

---

## 📘 Learning Outcome
After completing this activity, students will understand:
- How PWM simulates analog output in Arduino
- LED brightness control using `analogWrite()`
- The use of arrays and `while()` loops in embedded programming

---

## 👤 Author
Dianna Jane Elizabeth  
Arduino Laboratory Exercises 🚀
