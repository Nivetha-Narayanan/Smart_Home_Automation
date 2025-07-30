# Smart Home Automation System – EmbedQuest Winner (Samgatha x Vashisht 2025)

🏆 **First Prize Winner – EmbedQuest 2025**  
Hosted by **IIITDM Kancheepuram** during **Samgatha x Vashisht 2025**

---

## Overview

This **Smart Home Automation System** is a fully integrated embedded solution built using **Arduino**, focusing on **safety**, **automation**, and **convenience**. It combines **occupancy-based control**, **environmental hazard alerts**, and **automated rain protection** using sensor-actuator fusion.

---

## 🔧 Features

### ✅ Occupancy-Based Control
- Entry/Exit detection using **two ultrasonic sensors**
- Automatic **room light control** based on people count
- LCD greetings: `"Welcome!"` and `"Thank You!"`

### 🌧️ Rain Detection and Clothes Protection
- **Rain sensor** detects showers
- **Servo motor** automatically pulls clothes indoors
- Rising/Falling **buzzer tone** alerts users

### 🔥 Fire Detection System
- **Flame sensor** detects fire
- **Fast pulsing buzzer** alert
- LCD displays: `"FLAME ALERT!"`

### 🛢️ Gas Leakage Detection
- **MQ-based gas sensor** with adaptive threshold calibration
- **Medium-tone buzzer** alert
- LCD displays: `"GAS LEAKAGE!"`

### 📟 Live Display and Interaction
- **I2C LCD (16x2)** displays:
  - Occupancy count
  - Alert messages
  - Calibration progress
- All values update **in real-time**

---

## 📦 Hardware Components

| Component                 | Quantity |
|--------------------------|----------|
| Arduino Uno              | 1        |
| Ultrasonic Sensors       | 2        |
| MQ Gas Sensor (A1)       | 1        |
| Flame Sensor (D7)        | 1        |
| Rain Sensor (A0)         | 1        |
| I2C LCD Display (16x2)   | 1        |
| Servo Motor (Clothes)    | 1        |
| Relay Module (Light)     | 1        |
| Buzzer                   | 1        |
| Wires, Resistors, etc.   | -        |

---

## ⚙️ How It Works

### 1. **System Initialization**
- LCD shows **startup message**
- Gas sensor **calibrates** and sets **dynamic threshold**

### 2. **Occupancy Logic**
- **Ultrasonic sensors** detect entry/exit
- **People count** updates accordingly
- **Light control** using relay module

### 3. **Environmental Sensing**
- **Rain sensor** activates **servo motor** + buzzer (rising/falling tone)
- **Flame sensor** triggers **high-priority alarm**
- **Gas sensor** applies **moving average filter** to detect spikes

### 4. **Alerts and Outputs**
Each alert has **distinct outputs**:
- **Rain**: Rising/Falling buzzer tone
- **Gas**: Medium buzzer tone
- **Fire**: Fast beeping buzzer tone
- Corresponding **LCD messages** shown clearly

---


