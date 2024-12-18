# Development-of-IOT-Smart-water-meter
Development of IOT smart water meter


Smart Water Meter Using ESP32 and LoRa


Overview
This project demonstrates the development of a Smart Water Meter capable of measuring water quality and quantity in real-time. The system uses two ESP32 microcontrollers, five sensors, two LoRa modules, and an OLED display to collect and transmit water data efficiently over long distances.


Features
Water Quality Measurement: Includes TDS, pH, and temperature monitoring.
Water Flow and Pressure Monitoring: Tracks water flow rate and pressure in the pipeline.
Wireless Communication: Uses LoRa for long-range, low-power data transmission.
Real-time Data Visualization: Displays received data on an OLED screen.

System Architecture
Transmitter Node

Components:
ESP32 Microcontroller
TDS Meter, pH Sensor, Temperature Sensor, Water Flow Sensor, Water Pressure Sensor
LoRa Module
Functionality:
Reads data from sensors via analog/digital pins.
Transmits the collected data using LoRa via SPI communication.
Receiver Node
Components:
ESP32 Microcontroller
LoRa Module
OLED Display

Functionality:
Receives data via LoRa.
Displays sensor readings on the OLED screen using I2C communication.
Hardware Requirements
Microcontrollers: 2 x ESP32
Sensors:
TDS Meter
pH Sensor
Temperature Sensor
Water Flow Sensor
Water Pressure Sensor
Communication Modules:
2 x LoRa Modules
Display: OLED Display

Additional components like wires, connectors, etc.

Software Requirements
Arduino IDE for programming ESP32.
ThinkSpeak for iot cloud to visualize data
LoRa library for SPI communication.
Adafruit SSD1306 library for OLED display control.


Installation and Usage


Transmitter Node Setup
Connect the five sensors to the ESP32 analog/digital pins.
Connect the LoRa module to the ESP32 via SPI.
Upload the transmitter code to the ESP32 using Arduino IDE.


Receiver Node Setup
Connect the OLED display to the ESP32 using I2C.
Connect the LoRa module to the ESP32 via SPI.
Upload the receiver code to the ESP32.


Running the System
Power both the transmitter and receiver nodes.
Monitor real-time data on the OLED display.


Applications
Real-time water quality monitoring.
Industrial or domestic water usage tracking.
Smart IoT-based water management systems.


Future Improvements
Add cloud integration for remote data access.
Implement battery-powered operation.
Incorporate additional sensors for advanced water analytics.
Contributing
Contributions are welcome! Feel free to fork this repository, create a new branch, and submit a pull request.

License
This project is licensed under the MIT License. See the LICENSE file for details.
