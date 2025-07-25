# 🚀 Smart Elevator System Based on Human Detection Sensors

A smart, sensor-integrated elevator prototype designed to eliminate unnecessary stops in high-rise buildings—improving energy efficiency, reducing wait times, and enhancing passenger experience. This project was developed as part of the **TARP (Technical Answers for Real-World Problems)** initiative at Vellore Institute of Technology.

---

## 📽️ Demo

▶️ [(https://drive.google.com/file/d/1if8Rj_7sFI3fdlbPxIgC5ltkuuGLcmUc/view?usp=sharing)]

---

## 📌 Problem Statement

Conventional elevators stop at every floor where a button is pressed, even if no passengers are present. This results in:
- Increased energy consumption
- Delayed travel times
- Unnecessary mechanical wear

---

## ✅ Proposed Solution

This system integrates **ultrasonic** and **IR sensors** near the elevator buttons to detect human presence. The elevator will:
- ✅ Stop only if a person is detected after a button press
- ❌ Skip floors where no presence is detected, even if a button is pressed

---

## 🧠 How It Works

1. **Human Detection Module**: 
   - Uses IR and ultrasonic sensors to sense presence near button panel.
2. **Control & Decision Module**: 
   - Microcontroller processes sensor data and applies a rule-based algorithm.
3. **Execution Module**: 
   - Sends command to elevator system to either stop or bypass the floor.
4. **Feedback Module**: 
   - LCD displays messages: “Lift will stop here” or “Lift will not stop here”.

---

## 🛠️ Technologies Used

### Hardware:
- Arduino Uno
- IR Sensor
- Ultrasonic Sensor (HC-SR04)
- LCD (I2C 16x2)
- Push Button
- LED
- Resistors

### Software:
- Arduino IDE
- C++/Arduino C
- Simulation for testing

---

## 🔁 System Architecture

```plaintext
[Button Pressed] → [IR + Ultrasonic Sensors] → [Arduino Control Logic] → 
[Decision: Stop/Skip] → [LCD Feedback + LED Indicator]
