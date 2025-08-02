# Smart Home Automation System – EmbedQuest 2025 Champion (Samgatha x Vashisht)

🏅 **Secured First Place** at **EmbedQuest 2025**  
Organized by **IIITDM Kancheepuram** as part of **Samgatha x Vashisht 2025**

---

## 🔍 Project Summary

This Smart Home Automation prototype is a multifunctional embedded system powered by an Arduino microcontroller. Designed with a strong emphasis on **home safety, automatic control**, and **user convenience**, the system integrates multiple sensors and actuators to respond intelligently to human presence and environmental conditions.

---

## ✨ Key Functionalities

### 👥 Human Presence Detection
- Utilizes a pair of **ultrasonic modules** to monitor room entry and exit
- **Lights switch on/off** based on real-time occupancy
- **LCD** shows personalized messages such as `"Welcome"` or `"See You!"`

### 🌧️ Smart Rain Response
- **Rain sensor** detects precipitation
- **Servo motor** automatically retracts clothes drying outside
- Audible **alert with variable buzzer tones** indicates rain status

### 🔥 Flame Hazard Monitoring
- Detects fire via a **flame sensing module**
- Triggers a **rapid buzzer alarm** for immediate attention
- Shows `"FIRE DETECTED!"` warning on the LCD

### 🧪 Gas Leak Detection
- Employs an **MQ-series gas sensor** with smart thresholding
- Emits a **moderate buzzer tone** upon leakage detection
- LCD displays `"GAS ALERT!"` in real time

### 📺 Real-Time User Interface
- A **16x2 I2C LCD** is used to:
  - Show current people count
  - Display emergency messages
  - Indicate sensor calibration and status
- All updates are **instantaneous and dynamic**

---

## 🧰 Components Used

| Component               | Quantity |
|------------------------|----------|
| Arduino Uno            | 1        |
| HC-SR04 Ultrasonic     | 2        |
| MQ Gas Sensor          | 1        |
| Flame Sensor           | 1        |
| Rain Detection Module  | 1        |
| 16x2 LCD with I2C      | 1        |
| Servo Motor            | 1        |
| Single-Channel Relay   | 1        |
| Buzzer                 | 1        |
| Jumper Wires, Resistors| As needed |

---

## ⚙️ System Workflow

### 1. **Startup Phase**
- Displays a boot message on the LCD
- Gas sensor undergoes a **self-calibration** routine with adaptive thresholding

### 2. **Occupancy-Based Lighting**
- Distance readings from ultrasonic sensors detect directional movement
- Keeps a running count of individuals in the room
- **Relay module** toggles the room light based on occupancy

### 3. **Weather-Aware Mechanism**
- Rain detection activates the **servo motor** to protect clothing
- Special **rising and falling buzzer sound** alerts users during rainfall

### 4. **Fire and Gas Threats**
- A **high-frequency beep** notifies fire detection
- Gas spikes are identified through **smoothed average analysis**
- Alerts are clearly marked with unique buzzer tones and LCD messages

---

## 👨‍💻 Developer Note

This system was created as a complete embedded solution tailored for **smart living environments**. It brings together hardware-level automation and real-time feedback to ensure **comfort, safety, and proactive control** in a home setting.

Proudly presented as a winning project in **EmbedQuest 2025**, showcasing practical innovation in **IoT and embedded systems**.

# 🏠 Smart Home Automation System using Arduino

🎉 **First Prize Winner – EmbedQuest 2025**  
🎓 **Presented at Samgatha x Vashisht**, IIITDM Kancheepuram

---

## 📌 Project Overview

This Smart Home Automation system is a fully integrated embedded solution developed using **Arduino UNO**, designed to automate home safety and convenience features. It combines multiple sensors, actuators, and alert mechanisms to deliver a smart environment that responds intelligently to real-world events like presence detection, fire, gas leaks, and rainfall.

The project was developed and demonstrated by our team as part of **EmbedQuest 2025**, where it was awarded **First Prize** for its functional depth, creativity, and real-time responsiveness.

---

## 📝 Problem Statement (Provided by Organizers)

> *Design an embedded system prototype for a smart home that uses minimal components to provide automation and safety functionalities such as environmental hazard detection and occupancy-based control. The final demo must be built on an Arduino-compatible platform and should reflect real-time responsiveness and innovation in cost efficiency.*

⏳ **Time Limit**: 9 days  
🧪 **Round 1**: Abstract + Simulation (Online)  
🔬 **Round 2**: Live Working Model Demo (Onsite)

---


## 🔧 Features

- 👥 **Occupancy Detection**: Entry/Exit sensors update people count and automate lights/fan (simulated).
- 💡 **Auto Light/Fan Control**: Based on people count, status is displayed on LCD.
- 🌧️ **Rain Detection**: Detects rainfall, rotates servo to protect clothes.
- 🔥 **Flame Detection**: Alerts user with LCD message and buzzer.
- 🛢️ **Gas Leak Detection**: Detects hazardous gas levels and triggers warning.
- 📺 **LCD Display**: Real-time feedback for all status/alerts.
- 🔔 **Distinct Buzzer Patterns**: Different tones for rain, gas, and fire alerts.

---

## 🧰 Components Used

| Component             | Functionality                      |
|----------------------|-------------------------------------|
| Arduino UNO           | Main microcontroller               |
| Ultrasonic Sensors x2 | Entry/Exit monitoring              |
| Rain Sensor (Analog)  | Detects rain                       |
| Flame Sensor          | Fire detection                     |
| MQ-2 Gas Sensor       | Detects LPG/Gas leaks              |
| Servo Motor (SG90)    | Moves cloth cover mechanism        |
| I2C LCD 16x2          | Displays messages/status           |
| Relay Module          | [Simulated] appliance switching    |
| Buzzer                | Audible hazard alerts              |

---

## 🔁 System Logic

1. **Entry/Exit Monitoring**
   - 2 ultrasonic sensors detect direction of motion.
   - People count is incremented/decremented.
   - If count > 0: Display "Lights ON, Fan ON"  
   - If count = 0: Display "Lights OFF, Fan OFF"

2. **Rain Detection**
   - Analog rain sensor detects moisture.
   - Servo rotates to cover hanging clothes.
   - LCD shows “Rain Detected”.
   - Buzzer tone sweeps from 500–2000 Hz.

3. **Flame Detection**
   - Flame sensor detects infrared radiation from fire.
   - LCD: “FLAME ALERT” + “DOORS OPEN”
   - Buzzer beeps rapidly at 2000 Hz.

4. **Gas Detection**
   - MQ-2 analog value crosses a threshold.
   - LCD: “GAS LEAKAGE” + “DOORS OPEN”
   - Buzzer gives medium alert at 1500 Hz.

---

## 🔊 Buzzer Alerts

| Alert Type | Sound Pattern               |
|------------|-----------------------------|
| Fire       | Fast beeping @ 2000 Hz      |
| Gas Leak   | Medium beeping @ 1500 Hz    |
| Rain       | Rising–falling tone sweep   |

---

## 📺 LCD Display Messages

- **Welcome Message**: On entry → `Welcome Home`
- **Exit Message**: On last exit → `Thank You`
- **Status View**:
- Line 1: People: X
- Line 2: Lights & Fan ON  or OFF

- **Alert Display**:
- Fire → `FLAME ALERT  \nDOORS OPEN`
- Gas  → `GAS LEAKAGE  \nDOORS OPEN`
- Rain → `RAIN DETECTED  \nCLOTHS PROTECTED`

---

## 🧠 Code Highlights

```cpp
getDistance();             // Reads ultrasonic range
calibrateGasSensor();      // Sets gas sensor baseline
getFilteredGasValue();     // Averaged analog gas value
updateLCD();               // Dynamic LCD updates
fireAlarm();               // Fire buzzer + LCD logic
gasAlarm();                // Gas buzzer + LCD logic
rainAlarm();               // Rain buzzer + servo logic
showMessage();             // Reusable LCD msg function
```
## 🏠 Hardware Setup Preview

Here is the physical prototype of our Smart Home Automation System developed during EmbedQuest 2025:

![Smart Home Demo Structure](images/house_demo.jpg)


# 👥 Team Members

This project was developed by students of 
**Madras Institue Of Technology(Anna University),Chrompet**
 | Name             |
|------------------|
|Anusree S         |
|Nivetha N         |
| Reshmi R        |
| Roshinee P     | 



