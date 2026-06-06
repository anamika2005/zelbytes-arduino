Hardware Documentation

Project

Analog Sensor Calibration Suite

Microcontroller

Component| Specification
Board| Arduino Uno
Operating Voltage| 5V
Serial Communication| 9600 baud

---

Components Used

Component| Quantity
Arduino Uno| 1
LDR (Light Dependent Resistor)| 1
10kΩ Resistor| 1
DHT22 Temperature & Humidity Sensor| 1
HC-SR04 Ultrasonic Sensor| 1
Capacitive Soil Moisture Sensor v1.2| 1
Breadboard| 1
Jumper Wires| As Required

---

Pin Configuration

Sensor| Arduino Pin
LDR| A0
DHT22 Data| D4
HC-SR04 TRIG| D9
HC-SR04 ECHO| D10
Soil Moisture AOUT| A1
Soil Moisture Power| D7

---

Sensor Descriptions

LDR (Light Dependent Resistor)

- Analog light sensor.
- Used to classify light conditions as DARK, AMBIENT, or BRIGHT.
- Connected through a voltage divider circuit.

Calibration Parameters

- DARK_THRESHOLD = 300
- BRIGHT_THRESHOLD = 700

---

DHT22

- Digital temperature and humidity sensor.
- Measures ambient temperature and relative humidity.
- Sampling interval set to 2 seconds.

---

HC-SR04 Ultrasonic Sensor

- Measures distance using ultrasonic pulses.
- Operating range approximately 2 cm to 400 cm.
- Timeout protection implemented to prevent blocking.

Pin Assignment

- TRIG → D9
- ECHO → D10

---

Capacitive Soil Moisture Sensor v1.2

- Measures soil moisture using capacitive sensing.
- Analog output connected to A1.
- Sensor power controlled through D7.

Calibration Constants

- DRY_ADC = 820
- WET_ADC = 380

---

Operating Conditions

Parameter| Value
Supply Voltage| 5V
Baud Rate| 9600
Controller| Arduino Uno

---

Summary

This hardware setup integrates four sensors:

1. LDR for light intensity measurement.
2. DHT22 for temperature and humidity monitoring.
3. HC-SR04 for distance measurement.
4. Capacitive Soil Moisture Sensor for soil condition monitoring.

The sensors are calibrated and validated through Serial Monitor outputs and logged in CSV-compatible format.
