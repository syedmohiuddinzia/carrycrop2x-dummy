# carrycrop2x-dummy

## Introduction
This project is designed for the ESP32 microcontroller to transmit sensor data via Bluetooth using the Arduino framework. The sensor data includes values such as moisture, temperature, conductivity, pH, and nutrient levels (nitrogen, phosphorus, and potassium). The data is serialized into JSON format and sent over Bluetooth.

## Requirements
Ensure you have the following components and libraries:

 - ESP32 microcontroller
 - Arduino IDE with ESP32 board support
 - ArduinoJson library
 - BluetoothSerial library

## Setup Instructions
**Install Arduino IDE:** Download and install the Arduino IDE from the official website.

**Add ESP32 Board Support:** In Arduino IDE, go to ```File > Preferences```. Add the following URL to the "Additional Board Manager URLs": ```https://dl.espressif.com/dl/package_esp32_index.json```. Then, go to ```Tools > Board > Board Manager```, search for ```esp32```, and install it.

**Install ArduinoJson Library:** Go to ```Sketch > Include Library > Manage Libraries```, search for ```ArduinoJson```, and install it.

**Enable Bluetooth and SPP in ESP32:** Ensure that Bluetooth and Serial Port Profile (SPP) are enabled in the ESP32 configuration. If not, use the command ```make menuconfig``` to enable them.

## Description:
In our work, code initializes Bluetooth on an ESP32 and transmits sensor data as a JSON object. The data is sent every 5 seconds. 

The code handles the following tasks:

- **Library Inclusions:** Includes necessary libraries for JSON handling and Bluetooth communication.
- **Bluetooth Configuration Checks:** Ensures that Bluetooth and SPP are enabled on the ESP32.
- **Sensor Data Variables:** Initializes variables to simulate sensor data.
- **Bluetooth Initialization:** Sets up Bluetooth with a specific device name.
- **Data Transmission Loop:** Serializes sensor data into a JSON document and sends it over Bluetooth at regular intervals.

## Contact
For more details or any inquiries about this project, please contact the project owner:

Email: syedmohiuddinzia@gmail.com
