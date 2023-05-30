# Raspberrytinker
a look into Iot projects using raspberry pi.

# Raspberry Pi Pico Sensor Data Upload

This project enables you to read temperature and humidity data from an AHT10 sensor connected to a Raspberry Pi Pico and upload it to Adafruit IO using MQTT.

## Prerequisites

Before running the code, ensure you have the following:

- Raspberry Pi Pico board
- AHT10 temperature and humidity sensor
- Python installed on your Raspberry Pi Pico
- Internet connection
- Adafruit IO account

## Setup

1. Connect the AHT10 sensor to the Raspberry Pi Pico board.
   - Connect the VCC pin of the sensor to the 3.3V pin on the Pico.
   - Connect the GND pin of the sensor to a GND pin on the Pico.
   - Connect the SDA pin of the sensor to the SDA pin on the Pico (e.g., GP4).
   - Connect the SCL pin of the sensor to the SCL pin on the Pico (e.g., GP5).

2. Install the required libraries.
   - `umqtt.simple`: MQTT library for MicroPython.
   - `ahtx0`: Library for the AHT10 sensor.

3. Configure the code.
   - Set the appropriate values for the MQTT server, port, username, password, and topics.
   - Modify the GPIO pin numbers for the I2C bus.

## Usage

1. Upload the code to your Raspberry Pi Pico.
2. Connect the Pico to your computer.
3. Open a serial terminal to view the program output.
4. The code will attempt to connect to the Wi-Fi network and Adafruit IO MQTT broker.
5. Once connected, it will read temperature and humidity data from the AHT10 sensor.
6. The data will be published to the specified MQTT topics on Adafruit IO.
7. You can monitor the data on Adafruit IO and visualize it using graphs.

## Contributing

Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request.

## License

This
