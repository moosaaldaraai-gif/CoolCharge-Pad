# ❄️ CoolCharge Pad
### Smart Cooling Platform for Electric Vehicles

> Smart Cooling. Smarter Mobility. 🇦🇪

---

## 🇦🇪 عن المشروع
CoolCharge Pad هي منصة ذكية تُدمج مع مواقف محطات شحن السيارات الكهربائية، صُممت لتناسب البيئات الحارة مثل دولة الإمارات. تقوم المنصة بمراقبة درجة الحرارة وتشغيل نظام تبريد تلقائي أثناء فترة الشحن للمساعدة في تقليل تراكم الحرارة أسفل السيارة. ويُعد هذا المشروع نموذجًا أوليًا (Prototype) يمكن تطويره مستقبلًا ليتكامل مع محطات الشحن والبنية التحتية للمدن الذكية.

## 🇬🇧 About
CoolCharge Pad is a smart platform designed to integrate with EV charging station parking spaces in hot climates such as the UAE. It monitors temperature and automatically activates a cooling system during charging to help reduce heat buildup beneath parked electric vehicles. This project is a proof-of-concept prototype with the potential to integrate into future smart charging infrastructure and smart cities

---

## ✨ Features
- 🌡️ Real-time temperature & humidity monitoring
- 📺 OLED display showing live data
- 💨 Automatic fan control via MOSFET
- 🟢 LED indicators (Normal / High Temp)
- ⚡ ESP32 powered with WiFi capability
- 🔋 Helps reduce heat buildup beneath parked electric vehicles during charging.

---

## 🔧 Components
| Component | Model | Qty |
|-----------|-------|-----|
| Microcontroller | ESP32 DevKit V1 | 1 |
| Temperature Sensor | DHT22 | 1 |
| Display | OLED SSD1306 0.96" | 1 |
| Fan Controller | MOSFET Module | 1 |
| Cooling Fan | USB Fan 5V | 1 |
| Green LED | 5mm | 1 |
| Red LED | 5mm | 1 |
| Resistors | 100Ω | 2 |
| Prototyping | Breadboard + Jumper Wires | 1 |
| Power | Power Bank 5V | 1 |

---

## 📌 Wiring
| Component | Pin | GPIO |
|-----------|-----|------|
| DHT22 | DATA | GPIO4 |
| OLED | SDA | GPIO21 |
| OLED | SCL | GPIO22 |
| MOSFET | Signal | GPIO14 |
| Green LED | + | GPIO18 |
| Red LED | + | GPIO19 |

---

## 🌡️ How It Works
- DHT22 reads temperature every 2 seconds
- If temp > 40.0°C → Fan ON + Red LED 🔴
- If temp < 35.0°C → Fan OFF + Green LED 🟢
- Between 35°C and 40°C → system maintains previous state
- OLED displays real-time temperature & status

---

## 💻 Libraries Required
- DHT sensor library by Adafruit
- Adafruit SSD1306
- Adafruit GFX Library

---

## 🚀 How to Use
1. Install Arduino IDE
2. Install required libraries
3. Upload code to ESP32
4. Connect components as per wiring
5. Power on and monitor!

---

## 📜 License
MIT License - CoolCharge Pad Team 2026 🇦🇪

---

## 👨‍💻 Built With ❤️ in UAE
Smart Cooling. Smarter Mobility.
