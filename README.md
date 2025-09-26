Health Monitoring System with Blynk IoT

This project demonstrates a simple IoT-based health monitoring system using the ESP32 and two biomedical sensors. Data is collected from the sensors and sent to the Blynk IoT platform for real-time monitoring.

📌 Features

Pulse Oximeter & Heart Rate Monitoring using MAX30102

Non-contact Temperature Measurement using MLX90614 (GY906)

Real-time Data Logging on Blynk IoT

Health Status Indicators for both temperature and heart rate

Uptime Monitoring to track device running time

🛠️ Hardware Components

ESP32 Development Board

MAX30102 Pulse Oximeter & Heart Rate Sensor

MLX90614 (GY906) Infrared Temperature Sensor

Jumper Wires & Breadboard

🔌 Pin Connections

Both sensors communicate using I2C protocol:

SDA → GPIO21

SCL → GPIO22

📡 Blynk Virtual Pins Mapping
Virtual Pin	Function
V10	Power Control
V11	Uptime Monitor
V12	Temperature Reading
V13	Heart Rate Average
V14	Temperature Status
V15	Heart Rate Status
🚀 Getting Started

Clone this repository.

Install the required Arduino libraries:

Adafruit MLX90614

MAX30102 Library
 (or equivalent for MAX30102)

Blynk IoT Library

Open the .ino file in Arduino IDE / PlatformIO.

Configure your Wi-Fi credentials and Blynk template ID.

Upload the code to ESP32.

📲 Blynk IoT Setup

Create a new Blynk template.

Add datastreams for V10–V15 as defined above.

Deploy the dashboard with buttons, gauges, and status indicators.

📊 Example Dashboard

Power Button (V10) → Start/Stop data collection

Gauge/Display (V12) → Temperature in °C

Gauge/Display (V13) → Heart Rate in BPM

Status Widgets (V14 & V15) → Normal / Alert conditions

Label (V11) → Uptime in seconds/minutes

📄 License

This project is licensed under the MIT License – feel free to use and modify it for your own applications.