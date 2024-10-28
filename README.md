# Health Monitoring System

This project is an IoT-based health monitoring system that measures heart rate and temperature using a Pulse Sensor and an analog temperature sensor. The system displays real-time data on an LCD screen and sends the information to ThingSpeak for remote monitoring.

## Features

- Real-time heart rate monitoring using a Pulse Sensor.
- Temperature measurement in Fahrenheit using an analog temperature sensor.
- LCD display showing heart rate (BPM) and temperature.
- Sends data to ThingSpeak for remote monitoring via ESP8266 Wi-Fi module.
- Visual and auditory indicators for heartbeats.

## Hardware Required

- Arduino board (e.g., Arduino Uno)
- Pulse Sensor
- Analog temperature sensor
- 16x2 LCD
- ESP8266 Wi-Fi module
- Resistors (if necessary)
- Breadboard and jumper wires

## Circuit Diagram

![Circuit-Diagram](https://github.com/user-attachments/assets/35a81cd3-3a1b-40d9-911e-af67c85ccb4b)
/assets/87eecf58-42e6-4b7d-b351-5487595a003d)

## Hardware Setup

1. Connect the Pulse Sensor purple wire to analog pin A0.
2. Connect the temperature sensor to analog pin A1.
3. Connect the LCD pins as follows:
   - RS -> Pin 12
   - EN -> Pin 11
   - D4 -> Pin 5
   - D5 -> Pin 4
   - D6 -> Pin 3
   - D7 -> Pin 2
4. Connect the ESP8266 module (TX, RX) to pins 9 and 10 respectively.
5. Connect the power and ground pins accordingly.

![IMG_20181211_001750-768x441](https://github.com/user-attachments/assets/90c45df1-a595-49c7-9cbd-fdb9851fcc2d)

## Result Display

Upon running the system, the LCD displays real-time heart rate and temperature readings. Additionally, the data is sent to ThingSpeak for monitoring. 

### ThingSpeak Output

![Thinspeak-graph](https://github.com/user-attachments/assets/d7323bb9-24e2-4f41-90a8-06b9002b0d45)

## Usage

1. Upload the code to your Arduino board.
2. Connect the hardware as described in the setup.
3. Open the Serial Monitor to view real-time heart rate and temperature readings.
4. Monitor the data on ThingSpeak for remote access.
