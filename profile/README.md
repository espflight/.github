<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
<img width="1200" height="300" alt="ESPFlight_Banner" src="https://github.com/user-attachments/assets/b1f6d7cf-0bc7-4c71-9295-187bbf2753f5" />

Open Source Flight Controller Firmware for ESP MCUs

<div align="center">
  <img src="https://img.shields.io/badge/ESP32-Flight_Controller-blue?style=for-the-badge&logo=espressif&logoColor=white"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge"/>
  <img src="https://img.shields.io/github/stars/ESPFlight/ESPFlight?style=for-the-badge&color=yellow"/>
  <img src="https://img.shields.io/badge/Build-Passing-brightgreen?style=for-the-badge"/>
</div>

# 🚁 ESPFlight – The Most Open ESP32 Flight Controller

**Fly with Wi‑Fi, Bluetooth, and dual‑core power – no expensive flight boards needed.**

> ⚡ A complete flight controller for quadcopters, robots, and drones, running on ESP32 modules. Lightweight, modular, and ready to hack.

---

## ✨ Key Features

- 🔄 **8 motor outputs** @ 4 kHz update rate  
- 📡 **Dual radio** – Wi‑Fi for configuration, Bluetooth for joystick  
- 🧠 **Complementary filter** + angle estimator  
- 🎮 **Supports CRSF, SBUS, PPM** receivers  
- 🧩 **Built with Arduino & PlatformIO** – easy to extend  
- 📊 **Telemetry streaming** to Mission Planner, QGroundControl, or custom dashboard  
- 💾 **Settings saved in SPIFFS** – fly without re‑flashing  

---

## 🚀 Quick Start (3 commands)

```bash
git clone https://github.com/ESPFlight/ESPFlight.git
cd ESPFlight
pio run --target upload
