# DS18B20 Temperature Sensor with NodeMCU ESP8266 and KiwisIoT

## Project Overview

This project monitors temperature using a DS18B20 digital temperature sensor connected to an ESP8266 NodeMCU. It collects temperature readings and transmits the data to the KiwisIoT platform for real-time remote monitoring.

## Hardware Components

- ESP8266 NodeMCU
- DS18B20 Temperature Sensor
- 4.7kΩ Pull-up Resistor
- Jumper Wires
- Breadboard
- USB Cable
- Power Supply

## Software Requirements

- Arduino IDE
- ESP8266 Board Package
- KiwisIoT Arduino Library
- OneWire Library
- DallasTemperature Library

## Circuit Connections

| DS18B20 Sensor | ESP8266 NodeMCU |
| -------------- | --------------- |
| VCC            | 3.3V            |
| GND            | GND             |
| DATA           | D4              |

Connect a 4.7kΩ pull-up resistor between the DATA and VCC pins of the DS18B20 sensor.

## Working Principle

The DS18B20 measures the surrounding temperature and sends digital readings to the ESP8266 NodeMCU through the OneWire communication protocol. The controller processes the temperature data and transmits it to the KiwisIoT platform for real-time remote monitoring.

## KiwisIoT Dashboard

| Channel    | Data                          |
| ---------- | ----------------------------- |
| Channel 0  | Temperature (°C)              |
| Monitoring | Real-time temperature updates |

## Configuration

Update your Wi-Fi credentials and KiwisIoT Topic ID in the Arduino code:

```cpp
const char* ssid = "YOUR_WIFI_NAME";
const char* pass = "YOUR_WIFI_PASSWORD";
const char* topic = "YOUR_TOPIC_ID";
```

Upload the code to the NodeMCU ESP8266 and monitor temperature readings through the KiwisIoT dashboard.

## Applications

- Temperature monitoring systems
- Smart home automation
- Industrial temperature monitoring
- Aquarium temperature monitoring
- Environmental monitoring
- IoT-based temperature tracking

## Project Reference

**Hackster.io Project:**  
[https://www.hackster.io/harispidy07/ds18b20-temperature-sensor-with-nodemcu-esp8266-and-kiwisiot-990d97](https://www.hackster.io/harispidy07/ds18b20-temperature-sensor-with-nodemcu-esp8266-and-kiwisiot-990d97)

**KiwisIoT Platform:**  
[https://kiwisiot.com/](https://kiwisiot.com/)

**KiwisIoT GitHub Repository:**  
[https://github.com/Kiwistron/KiwisIoT-Projects](https://github.com/Kiwistron/KiwisIoT-Projects)

## Author

**Hariprasath S**

GitHub: [https://github.com/harispidy07](https://github.com/harispidy07)

---

_Built using ESP8266, DS18B20 Temperature Sensor, and KiwisIoT for real-time temperature monitoring._
