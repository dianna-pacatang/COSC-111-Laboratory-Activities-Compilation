# Final Laboratory Exam – Remote Arduino Control via HTTP API 🌐🔌

## 📌 Overview
This project demonstrates a **remote Arduino control system** implemented through **HTTP API communication**. A **local Arduino setup with a push button** sends a signal to a **Python application**, which then triggers an **API request to the instructor’s system**. The request activates an LED on the **instructor’s Arduino**, enabling remote hardware control.

The project showcases a complete **IoT-style interaction**, where hardware input on one device controls hardware output on another device through software and network communication.

---

## 🎯 Objectives
- Apply Arduino Serial Communication
- Integrate physical hardware input with Python
- Perform HTTP API calls to control a remote Arduino device
- Demonstrate end-to-end IoT communication flow

---

## 🧰 Components Used

### Local Setup (Student Side)
- Arduino MCU
- 1 Push Button
- Resistor
- Breadboard and jumper wires
- Laptop with Python

### Remote Setup (Instructor Side)
- Arduino MCU
- LED
- FastAPI-based control server  
*(Instructor-owned and not included in this repository)*

---

## 🔌 Local Pin Configuration
| Component | Arduino Pin |
|---------|-------------|
| Push Button | D2 |

---

## 🔧 Circuit Diagram Clarification
The included **Tinkercad circuit diagram (PNG)** represents **only the local button setup** used to initiate the API request.

- The diagram illustrates the **student’s Arduino**, which acts as a remote controller.
- Pressing the button sends a signal to the Python application via **Serial Communication**.
- The Python application then sends an HTTP request to the instructor’s API.
- The API controls the LED connected to the **instructor’s Arduino**.

⚠️ The **instructor’s Arduino circuit is not included**, as it was externally hosted and not accessible during the exam.

All provided diagrams and files therefore represent **only the client-side (remote) implementation**.

---

## 🔄 System Flow
1. A push button is pressed on the local Arduino.
2. Arduino sends a signal (`"1"`) to the Python application via Serial.
3. Python receives the signal and calls the instructor’s API endpoint.
4. The API processes the request and toggles the LED on the instructor’s Arduino.

---

## 📂 Files Included
- `*.ino` – Arduino sketch for detecting button press and sending Serial output
- `*.py` – Python script that listens to Serial input and performs API requests
- `*.png` – Tinkercad diagram of the local button setup
- `README.md` – Project documentation

---

## ▶️ How to Run

### Arduino (Local)
1. Open the Arduino sketch in Arduino IDE.
2. Connect the push button according to the pin configuration.
3. Upload the code to the Arduino board.

### Python (Local)
1. Install required libraries:
2. Update the COM port in the Python script if necessary.
3. Run the Python application.
4. Press the push button to trigger the remote LED.

---

## 🧪 Expected Output
- Button press sends a Serial signal from Arduino.
- Python immediately calls the instructor’s API.
- LED on the instructor’s Arduino toggles.
- Response time is within **1 second**.

---

## 📘 Learning Outcome
This final examination activity demonstrates the ability to:
- Combine hardware, software, and networking concepts
- Implement real-world IoT communication models
- Control remote devices using API-driven architectures
- Apply modular and scalable system design principles

---

## 👤 Author
Dianna Jane Elizabeth  
COSC 111 – Final Laboratory Exam 🚀
