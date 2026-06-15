 # Task 7 - CSV Data Logging

## Objective

To log environmental sensor data in CSV format for monitoring and analysis. The system records timestamp, temperature, humidity, soil moisture, and light intensity readings.

## Components Used

- Arduino Uno
- DHT11 Sensor
- Soil Moisture Sensor
- LDR Sensor
- USB Cable

## Hardware Connections

### DHT11 Sensor
- VCC → 5V
- GND → GND
- DATA → D2

### Soil Moisture Sensor
- VCC → 5V
- GND → GND
- AO → A1

### LDR Sensor
- VCC → 5V
- GND → GND
- AO → A0

## Logging Method

This project uses Serial CSV Logging. Sensor readings are collected periodically and transmitted through the Serial Monitor in CSV format. The data is saved as a CSV file for later analysis.

## CSV Columns

- timestamp : Time since Arduino startup (milliseconds)
- temp : Temperature reading
- humidity : Humidity reading
- soil : Soil moisture reading
- light : Light intensity reading

CSV Header:

timestamp,temp,humidity,soil,light

## Working

The Arduino continuously reads sensor values and generates a timestamp using the millis() function. The readings are formatted as CSV data and sent through serial communication. The data is captured and stored in sample_log.csv.

## How to Reproduce

1. Connect the sensors according to the hardware connections.
2. Upload the Arduino sketch to the Arduino Uno.
3. Open the Serial Monitor.
4. Observe the CSV formatted sensor readings.
5. Save the serial output as sample_log.csv.
6. Verify that the file contains at least 50 rows of data.

## Output

The generated CSV file contains timestamped sensor readings and can be opened using Excel, Google Sheets, or any CSV viewer.

## Result

Environmental sensor data was successfully logged and stored in CSV format for analysis and monitoring.