# 🎤 ESP3V2 4x5 Free - EBJRemote

A custom Bluetooth and Web-based remote controller for **SongHub Karaoke**, built using an **ESP32-C3** and a **4x5 Matrix Keypad**. 

## ✨ Features
- **Bluetooth HID**: Connects seamlessly to Android TV / SongHub app as `EBJRemote`.
- **Built-in Web Remote**: Connect to WiFi AP `EBJRemote` (IP: `192.168.4.1`) to control the karaoke system from your phone.
- **Full Controls**: Play, Pause, Stop, Next, Prev, Volume, Melody, BGV, Reserve, and numeric song codes.
- **Plug & Play**: No registration or activation required.

---

## ⚡ One-Click Web Flasher
You don't need to install Arduino IDE to use this! 
1. Plug your ESP32-C3 into your computer using a USB cable.
2. Open **Google Chrome** or **Microsoft Edge**.
3. Go to the Web Flasher page: **[Click Here to Flash][(https://ryusukilight.github.io/ESP3V2_4x5_free/)](https://ryusukilight.github.io/ESPC3V2_4x5_free/)**
4. Click the **"CONNECT & INSTALL"** button.

---

## 🔌 Wiring Diagram (ESP32-C3 to 4x5 Keypad)

| Keypad Wire | ESP32-C3 Pin | Code Variable | Buttons on this Line |
| :--- | :--- | :--- | :--- |
| **Row 1** | **GPIO 4** | `rowPins[0]` | Melody, 1, 2, 3, Reserve |
| **Row 2** | **GPIO 3** | `rowPins[1]` | BGV, 4, 5, 6, Clear |
| **Row 3** | **GPIO 1** | `rowPins[2]` | Vol+, 7, 8, 9, PREV |
| **Row 4** | **GPIO 0** | `rowPins[3]` | Vol-, STOP, 0, PLAY, NEXT |
| **Column 1** | **GPIO 5** | `colPins[0]` | Melody, BGV, Vol+, Vol- |
| **Column 2** | **GPIO 6** | `colPins[1]` | 1, 4, 7, STOP |
| **Column 3** | **GPIO 7** | `colPins[2]` | 2, 5, 8, 0 |
| **Column 4** | **GPIO 10** | `colPins[3]` | 3, 6, 9, PLAY |
| **Column 5** | **GPIO 2** | `colPins[4]` | Reserve, Clear, PREV, NEXT |

---

## 📱 How to Use
1. Power on the ESP32-C3.
2. On your TV or Android device, open Bluetooth settings and pair with **`EBJRemote`**.
3. On your phone, connect to the WiFi network named **`EBJRemote`** (Password: none).
4. Open a web browser and go to **`192.168.4.1`** to access the on-screen remote!

## 👨‍💻 Developer
**Electronicsbuilds by ArnelJr**
- [Facebook Page](https://www.facebook.com/Arneljreasybuild)
- [GitHub Profile](https://github.com/Ryusukilight)
