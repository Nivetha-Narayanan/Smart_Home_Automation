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
