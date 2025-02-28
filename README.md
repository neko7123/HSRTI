# ESP8266 Ultrasonic Sensor Data Logger with ThingSpeak & Android App

## 📌 Project Overview
This project uses an **ESP8266** (Arduino UNO D1 WiFi) to collect real-time distance measurements from **ultrasonic sensors** and uploads the data to **ThingSpeak** for remote monitoring. Additionally, an **Android app (built with Kotlin)** retrieves and displays the data for easy visualization.

## 🛠 Features
- Real-time distance measurement using **four ultrasonic sensors** (HC-SR04)
- **WiFi connectivity** for uploading data to ThingSpeak
- **Android app** (built with Kotlin) for displaying sensor data
- **Data logging & cloud storage** for remote access

## 🏗 Hardware Requirements
- **ESP8266 (NodeMCU/Arduino UNO D1 WiFi)**
- **4× HC-SR04 Ultrasonic Sensors**
- **Jumper Wires**
- **5V Power Supply** (for sensors & ESP8266)

## 📲 Software Requirements
- **Arduino IDE** (for ESP8266 programming)
- **ESP8266 Board Package** installed in Arduino IDE
- **Kotlin-based Android App** (for mobile monitoring)
- **ThingSpeak API Key** (for cloud data storage)

## 🔧 Circuit Diagram & Connections
| Sensor | Trig Pin (ESP8266) | Echo Pin (ESP8266) |
|--------|-------------------|-------------------|
| Left 1 | D7 | D8 |
| Left 2 | D2 | A0 |
| Right 1 | D5 | D6 |
| Right 2 | D3 | D4 |

**Note:** Ensure that each sensor has a stable **5V power supply** for accurate measurements.

## 🚀 Setup Instructions
### 1️⃣ ESP8266 Configuration
1. Install **Arduino IDE**
2. Add ESP8266 support in **Boards Manager**
3. Install required libraries: `ESP8266WiFi`, `WiFiClient`
4. Upload the provided **ESP8266 code**
5. Replace WiFi SSID & password in the sketch
6. Get a ThingSpeak **API key** and update it in the code
7. Flash the code onto ESP8266

### 2️⃣ ThingSpeak Setup
1. Create a **ThingSpeak account**
2. Set up a new **channel**
3. Note the **API key** and update it in the ESP8266 code

### 3️⃣ Android App Setup
1. Install **Android Studio**
2. Clone the **Kotlin-based app repository**
3. Replace the ThingSpeak API key in the app’s code
4. Build & install the app on an Android device

## 📡 Data Flow
1. **ESP8266 reads** distances from ultrasonic sensors
2. **Uploads data** to ThingSpeak every second
3. **Android app retrieves** data from ThingSpeak and displays it

## 🔍 Troubleshooting
- **WiFi Not Connecting?** Check SSID & password in the ESP8266 code.
- **ThingSpeak Not Updating?** Ensure your API key is correct.
- **Corrupt Serial Output?** Set baud rate to **115200** in Serial Monitor.
- **Android App Not Displaying Data?** Ensure the API key is correctly entered in the app.

## 📌 Future Enhancements
- Add **MQTT support** for real-time updates
- Implement **push notifications** for sensor alerts
- Improve **UI/UX of Android app**

## 🤝 Contributions
Feel free to contribute by optimizing the **ESP8266 code** or improving the **Android app UI**.

## 📜 License
This project is open-source under the **MIT License**. Use and modify freely!

---

### 📧 Contact
For any questions or support, reach out to **Narong** (Project Developer).

