# 🚗 ESP32 Dual Mode Smart Car

An advanced **ESP32-based Wi-Fi Smart Car** with **Dual Mode operation**:
- 🧠 **Auto Mode** → Line follower + Obstacle avoidance
- 📱 **Manual Mode** → Controlled via smartphone web interface (Wi-Fi)

Built using **Arduino IDE** and **ESP32 WebServer** library.  
No external app required — just connect to the ESP32's Wi-Fi network.



## ✨ Features
✅ Dual mode switching (Auto ↔ Manual)  
✅ Web-based controller (works on any phone browser)  
✅ Real-time distance + line sensor dashboard  
✅ Smooth press-to-move control (stops when released)  
✅ Fully standalone — no internet required  



## 🛠️ Hardware Setup

| Component | ESP32 Pin | Description |
|------------|------------|-------------|
| L298N ENA | 14 | Motor A speed control |
| L298N IN1 | 27 | Left Motor direction |
| L298N IN2 | 26 | Left Motor direction |
| L298N IN3 | 25 | Right Motor direction |
| L298N IN4 | 33 | Right Motor direction |
| L298N ENB | 32 | Motor B speed control |
| IR Left Sensor | 34 | Line follower left |
| IR Right Sensor | 35 | Line follower right |
| Ultrasonic Trigger | 23 | Distance sensor |
| Ultrasonic Echo | 22 | Distance sensor |
| Servo (Ultrasonic mount) | 13 | Rotation for scanning |
| GND | GND | Common ground |



## ⚙️ Software Setup

1. Install [Arduino IDE](https://www.arduino.cc/en/software)
2. Add ESP32 board manager URL:  
   `https://dl.espressif.com/dl/package_esp32_index.json`
3. Select **Board → ESP32 Dev Module**
4. Install libraries (if missing):
   - `WiFi.h`
   - `WebServer.h`
5. Upload code from `src/esp32_dual_mode_car.ino`

---

## 🌐 How to Use

1. Power on the ESP32 car.  
2. Connect your phone to:
