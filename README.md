# Air-Quality-Monitoring-System
Air quality monitoring system continuously measures pollutants and basic environmental conditions to show how clean or harmful the air is. It uses gas and particle sensors, a controller (like ESP32), and communication/display to present real time data and alarms, helping people react quickly to gas leaks, smoke, or unhealthy indoor and outdoor air.
## Materials Required

- ESP32 DevKit V1
- MQ2 Gas Sensor Module (LPG, Smoke, CO)
- DHT22 Temperature & Humidity Sensor
- SSD1306 OLED Display (128x64, I2C)
- Active Buzzer (5V)
- Red LED + Green LED
- 220Ω Resistors (2 nos)
- Breadboard & Jumper Wires
- USB Power Bank (5V)

## Connection Procedure

ESP32 → Sensors

VIN(5V) → MQ2 VCC

3.3V → DHT22 VCC, OLED VCC

GND → All GND

GPIO36 → MQ2 AO (Analog)

GPIO15 → MQ2 DO (Digital)

GPIO4 → DHT22 DATA

GPIO23 → Buzzer +

GPIO19 → Red LED + (220Ω)

GPIO18 → Green LED + (220Ω)

GPIO21 → OLED SDA

GPIO22 → OLED SCL


## How It Works

- **Green LED ON** = GOOD AIR QUALITY
- **Red LED + Buzzer** = POOR AIR QUALITY
  - Gas > 1200 (Pollutants detected)
  - Temperature > 35°C (Uncomfortable)

## OLED Shows
Air Quality Monitor
T: 28.5 C
H: 65.2%
AQI: 800
GOOD


## Setup Steps
1. Install Libraries: Adafruit SSD1306, Adafruit GFX, DHT sensor
2. Connect as shown above
3. Upload code to ESP32
4. Power with USB power bank
5. Wait 20 sec for warmup

## Cost: ₹2200-2800
## Power: USB Power Bank (8+ hrs)

**By JP Harikrishna Raj**  
**Embedded & IoT Developer**
