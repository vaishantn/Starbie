# Starbie ⭐

A tiny motion-controlled digital pet—basically a desktop Tamagotchi! 

## About
Starbie is an interactive hardware project built around a custom PCB. It features a microcontroller, an OLED display to show your digital pet, motion and environment sensors, and tactile mechanical keyboard switches for user input.

## Features
- **Motion Control:** Uses an MPU6050 sensor to detect tilt and motion.
- **Environment Tracking:** Includes a DHT11 sensor to check temperature and humidity.
- **Interactive Input:** Built with Cherry MX mechanical switches.
- **Visual Display:** Equipped with a sharp OLED screen to bring your pet to life.

## Bill of Materials (BOM)
| Part | Qty | Description |
| :--- | :---: | :--- |
| **Seeed Studio XIAO ESP32-C3** | 1 | Microcontroller |
| **0.96" OLED Graphic Display** | 1 | Display module for the character |
| **MPU6050** | 1 | Motion and tilt sensor |
| **Cherry MX Silent Red Switch** | 2 | User input switches |
| **DHT11 Sensor** | 1 | Temperature & humidity sensor |
| **10k Resistor** | 1 | Pull-up resistor for the sensor |

## Project Schematics

<img width="593" height="382" alt="image" src="https://github.com/user-attachments/assets/9ff98d4f-aff8-4787-b942-e1bcef7ba611" />
<img width="686" height="604" alt="Screenshot 2026-10-09 141937" src="https://github.com/user-attachments/assets/d41827e3-fde1-45f9-87da-9d24950c6901" />



## Built With
- **KiCad** - PCB design and schematic routing
- **Arduino IDE / C++** - Firmware (`starbie.ino`)
