# Smart Weather Monitoring System

Welcome to the Smart Weather Monitoring System project! This system is designed to monitor environmental parameters such as temperature, humidity, and light intensity. The system is built using IoT technology, featuring the ESP32 microcontroller, DHT22 and LDR sensors, and a passive buzzer as the actuator.

## Features

- Measures temperature and humidity using a DHT22 sensor.
- Measures light intensity using an LDR (Light Dependent Resistor).
- Measures potentiometer values.
- Displays real-time data on a 16x2 I2C LCD.
- Sends data to ThingSpeak for remote monitoring and analytics.
- Triggers a buzzer alarm if temperature or humidity exceeds set thresholds.
- LED indication for Wi-Fi connection status.

## Project Description

The Smart Weather Monitoring System collects data from various sensors and transmits the data to the ThingSpeak Cloud via Wi-Fi. The data is visualized on a user-friendly dashboard, accessible through the web, providing reliable and accurate information for industries reliant on weather conditions.

## Demo Links

- **Wokwi System Simulator (with code)**: [Wokwi Project](https://wokwi.com/projects/417887757310844929)
- **ThingSpeak Dashboard**: [ThingSpeak Channel](https://thingspeak.mathworks.com/channels/2792928)

## Simmulator 
![image](https://github.com/user-attachments/assets/c874ebb1-4c66-4be9-b8d7-6e64d8b68252)


## ThingSpeak Dashboard
<p align="center">
  <img src="https://github.com/user-attachments/assets/7fb51383-3b7c-4937-92b2-daadcbd8a7ec" width="300" height="200" alt="ThingSpeak Dashboard 1"/>
  <img src="https://github.com/user-attachments/assets/5cfaf61f-55e8-4502-91c0-151ddc3a837f" width="300" height="200" alt="ThingSpeak Dashboard 2"/>
  <img src="https://github.com/user-attachments/assets/43156b90-a32f-4e98-b30f-34011ed7c496" width="300" height="200" alt="ThingSpeak Dashboard 3"/>
</p>



## Hardware Requirements

- ESP32 development board
- DHT22 temperature and humidity sensor
- LDR (Light Dependent Resistor)
- Potentiometer
- 16x2 I2C LCD
- Buzzer
- LED
- Jumper wires
- Breadboard

## Software Requirements

- Arduino IDE
- ESP32 board support for Arduino IDE
- Arduino libraries:
  - `LiquidCrystal_I2C`
  - `WiFi`
  - `DHTesp`
  - `ThingSpeak`

## Setup Instructions

1. **Install Arduino IDE**:
   Download and install the [Arduino IDE](https://www.arduino.cc/en/software).

2. **Add ESP32 Board Support**:
   - Open Arduino IDE.
   - Go to `File` > `Preferences`.
   - In the "Additional Board Manager URLs" field, add:
     ```
     https://dl.espressif.com/dl/package_esp32_index.json
     ```
   - Go to `Tools` > `Board` > `Board Manager`.
   - Search for `esp32` and install the latest version.

3. **Install Required Libraries**:
   - Go to `Sketch` > `Include Library` > `Manage Libraries`.
   - Search for and install the following libraries:
     - `LiquidCrystal_I2C`
     - `WiFi`
     - `DHTesp`
     - `ThingSpeak`

4. **Clone the Repository**:
