# 🚨 WiFi Deauther IoT Project using ESP8266

A powerful **WiFi Deauther tool** built using the **ESP8266** microcontroller. It performs WiFi deauthentication attacks for **penetration testing and ethical hacking education**.

> ⚠️ **Use Responsibly:** This project is for **educational purposes only**. Do **not** test on any WiFi network you don't own or have permission to test.

---

## 🛠 Features

- Scan nearby WiFi networks
- List connected devices
- Perform deauth attacks on selected targets
- Web-based interface for control
- Optional LCD/OLED display
- Easy flashing with prebuilt `.bin` file

---

## 🔧 Hardware Requirements

| Component        | Description                  |
|------------------|------------------------------|
| ESP8266          | NodeMCU, Wemos D1 Mini, etc. |
| I2C LCD / OLED   | 16x2 LCD or 128x64 OLED (optional) |
| USB Cable        | For flashing + power          |
| Jumper Wires     | For connections               |

---

## 📌 Pin Connections (for LCD)

| LCD Pin | ESP8266 Pin |
|---------|-------------|
| GND     | GND         |
| VCC     | 3V3         |
| SDA     | D2 (GPIO4)  |
| SCL     | D1 (GPIO5)  |

---

## 📐 Circuit Diagram

![ESP8266 circuit diagram OLED](https://github.com/user-attachments/assets/0336faca-23b5-4368-84ed-4906eef90827)

---

## 🧩 Schematic View
![image](https://github.com/user-attachments/assets/6bdcfe61-fe08-4718-bbcc-23eed44548ce)

---

## 📦 Flashing Firmware (No Code Needed)

### ✅ Downloads

- 🔥 Precompiled Firmware `.bin`: [Download Here](https://your-link.com/deauther-firmware.bin)
- 🧰 ESP Flasher Tool (Windows): [Download Here](https://github.com/nodemcu/nodemcu-flasher)
- 🔌 USB to UART Driver (CH340/CP210x):
  - [CH340 Driver (Windows/Mac/Linux)](https://sparks.gogo.co.nz/ch340.html)
  - [CP210x Driver](https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers)

### 🧠 How to Flash

1. Install USB to UART driver
2. Connect ESP8266 via USB
3. Open ESP8266Flasher or any flashing tool
4. Load the `.bin` file
5. Select correct COM port
6. Click **Flash**
7. Done! Connect to hotspot `Deauther-ESP`

---

## 💻 Developer Setup (Optional)

### Libraries (Arduino IDE)

- `ESP8266WiFi.h`
- `ESP8266WebServer.h`
- `Wire.h`
- `LiquidCrystal_I2C.h` or `Adafruit_SSD1306.h`

### Upload Code (if modifying)

- Select **NodeMCU 1.0** board
- Upload using Arduino IDE or PlatformIO

---

## 🖥 Web Interface

- Connect to WiFi: `Deauther-ESP`
- Go to `http://192.168.4.1`
- Control targets, start/stop attack, monitor devices


