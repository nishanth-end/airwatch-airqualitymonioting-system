# AirWatch — Air Quality Monitoring System

A real-time environmental monitoring system built with ESP32, MQ-2, and DHT11 sensors. Live data is pushed to ThingSpeak cloud and displayed on a custom web dashboard.

## Hardware
- ESP32 Development Board
- MQ-2 Gas Sensor (GPIO 34)
- DHT11 Temperature & Humidity Sensor (GPIO 4)
- SSD1306 OLED Display (SDA: GPIO 21, SCL: GPIO 22)

## Features
- Real-time gas, temperature, and humidity readings
- OLED display for local monitoring
- Cloud data logging via ThingSpeak every 20 seconds
- Web dashboard with historical graphs
- Outdoor air quality comparison via OpenWeatherMap API
- Health advisory based on gas levels

## Dashboard
Built with vanilla HTML/CSS/JS. Dark control panel aesthetic.

## Setup
1. Flash `airwatch.ino` to ESP32 via Arduino IDE
2. Add WiFi credentials and ThingSpeak API key to the sketch
3. Create `config.js` with your API keys (see `config.example.js`)
4. Open `index.html` in browser or host on GitHub Pages