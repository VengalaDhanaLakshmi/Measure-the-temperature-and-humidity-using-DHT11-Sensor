**DHT11 Temperature & Humidity Measurement**

A simple project to measure temperature and humidity using the DHT11 Sensor, and display/log the values in a serial monitor using a microcontroller (Arduino/ESP/AVR).
This project demonstrates how to interface a DHT11 with a microcontroller to measure environmental temperature and humidity.
The DHT11 communicates using a single-wire digital protocol, providing calibrated values that can be directly processed and displayed.

**Features**
✔ Reads temperature (°C) and humidity (%)

✔ Uses DHT11 digital communication protocol

✔ Supports Arduino / ESP32 / ESP8266 / AVR

✔ Displays output in Serial Monitor

✔ Easy to integrate in IoT or weather monitoring projects

**Hardware Requirements**

* DHT11 Sensor
* Arduino / ESP32 / ESP8266 / ATmega microcontroller
* 10K pull-up resistor
* Jumper wires
* USB cable
**Circuit Connections**

| DHT11 Pin | Description | Connect To                   |
| --------- | ----------- | ---------------------------- |
| VCC       | +5V / 3.3V  | 5V / 3.3V pin                |
| DATA      | Sensor Data | Any digital pin (example D2) |
| GND       | Ground      | GND                          |
| NC        | No Connect  | —                            |

**Note:** -- Add a **10K pull-up resistor** between DATA and VCC.

 **How It Works**
* The microcontroller sends a start pulse to the DHT11.
* DHT11 responds and sends **40 bits** of data (humidity + temperature + checksum).
* The microcontroller decodes the data and prints it to the serial monitor.

 **Applications**
* Weather monitoring systems
* Smart home environments
* IoT dashboards
* Greenhouse monitoring
* Environmental sensing projects
  
 **Future Enhancements**
* Add LCD/OLED display
* Push data to IoT cloud platforms (Blynk, Thingspeak)
* Log data using SD Card
* Use DHT22 for better accuracy
