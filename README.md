# Starbie ⭐

**Starbie** is a tiny, interactive motion-controlled digital pet—think of it as a custom-built, hardware-hackable desktop Tamagotchi! Designed from scratch as a custom PCB, Starbie brings a virtual pet to life using an embedded microcontroller, a crisp OLED display, environmental sensors, tilt detection, and tactile mechanical keyboard switches.

---

## 🌟 Features

- **Motion & Tilt Detection:** Integrated MPU6050 6-axis accelerometer and gyroscope to track orientation, shakes, and tilts so you can interact with your pet physically.
- **Environment Tracking:** Built-in DHT11 sensor to monitor ambient temperature and humidity.
- **Tactile Mechanical Input:** Uses genuine Cherry MX mechanical switches for satisfying tactile user control.
- **Crisp Visuals:** Features a 0.96-inch OLED graphic display capable of rendering smooth animations and expressions for your digital pet.
- **Compact Microcontroller Core:** Powered by the versatile Seeed Studio XIAO ESP32-C3 for low-power operation, Wi-Fi capabilities, and compact integration.

---

## 📦 Bill of Materials (BOM)

| Part Name | Qty | Description |
| :--- | :---: | :--- |
| **Seeed Studio XIAO ESP32-C3** | 1 | Low-power RISC-V microcontroller with Wi-Fi/BLE |
| **0.96" OLED Graphic Display** | 1 | Monochrome display module (I2C/SPI) for character rendering |
| **MPU6050 Sensor Module** | 1 | 3-axis accelerometer & 3-axis gyroscope |
| **Cherry MX Silent Red Switch** | 2 | Mechanical keyboard switches for user input buttons |
| **DHT11 Sensor** | 1 | Digital temperature and humidity sensor |
| **10k Resistor** | 1 | Pull-up resistor for sensor stability |

---

## 🛠️ Hardware Architecture & Pinout

Starbie's schematic routes all peripherals directly to the XIAO ESP32-C3 breakout headers:
- **I2C Bus:** Shared between the MPU6050 motion sensor and the 0.96" OLED display.
- **GPIO Inputs:** Connected to the Cherry MX mechanical switches with internal pull-ups enabled.
- **Single-Wire Interface:** Dedicated pin for reading temperature and humidity data from the DHT11 module.

---

## 🚀 Getting Started & Firmware Installation

### Prerequisites
- [Arduino IDE](https://www.arduino.cc/en/software) installed on your machine.
- ESP32 board support packages added via the Arduino Board Manager.
- Required libraries installed:
  - `Adafruit_GFX` & `Adafruit_SSD1306` (for the OLED display)
  - `Adafruit_MPU6050` (for motion tracking)
  - `DHT sensor library` (for environmental data)

### Flashing the Firmware
1. Clone this repository or download the source files.
2. Open the `starbie.ino` file inside the Arduino IDE.
3. Select your board (`Seeed Studio XIAO_ESP32C3`) and the correct COM port from **Tools > Board**.
4. Click the **Upload** button to flash the code to your microcontroller.

---

## 📸 Project Schematics

<img width="593" height="382" alt="Screenshot 2026-10-09 153249" src="https://github.com/user-attachments/assets/fe17d6f6-ae0b-469f-937a-eb095f8114ae" />

<img width="686" height="604" alt="Screenshot 2026-10-09 141937" src="https://github.com/user-attachments/assets/10f61098-01ef-4143-a8b2-92fef63a2a7b" />


---

## 🧰 Built With

- **KiCad** - Schematic capture, custom footprint creation, and PCB layout routing
- **Arduino IDE / C++** - Firmware development and sensor integration

---
