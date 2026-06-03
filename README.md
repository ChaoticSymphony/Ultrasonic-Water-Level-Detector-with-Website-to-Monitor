# Ultrasonic Water Level Detector with Website Monitor

A smart IoT project for homes with water tanks that uses an ultrasonic sensor connected to an ESP32 microcontroller to monitor water levels in real-time and display the data on a web interface.

## Features

- **Real-time Water Level Monitoring**: Ultrasonic sensor accurately measures water tank levels
- **Web Dashboard**: Monitor your water tank remotely through a responsive web interface
- **ESP32 Integration**: Uses ESP32 microcontroller for reliable connectivity and processing
- **Wireless Connectivity**: WiFi-enabled for remote monitoring
- **Data Tracking**: Historical data logging and visualization capabilities

## Hardware Requirements

- ESP32 Development Board
- Ultrasonic Sensor (HC-SR04 or similar)
- Water Tank
- Power Supply
- Connecting Wires & Breadboard

## Software Requirements

- Arduino IDE or PlatformIO
- Python (for web server)
- Modern web browser for dashboard access

## Installation

### Hardware Setup

1. Connect the ultrasonic sensor to the ESP32:
   - VCC → 5V
   - GND → GND
   - TRIG → GPIO pin (configurable)
   - ECHO → GPIO pin (configurable)

2. Mount the sensor above your water tank pointing downward

3. Power the ESP32 board

### Software Setup

1. Clone this repository
   ```bash
   git clone https://github.com/ChaoticSymphony/Ultrasonic-Water-Level-Detector-with-Website-to-Monitor.git
   cd Ultrasonic-Water-Level-Detector-with-Website-to-Monitor
   ```

2. Upload the ESP32 code:
   - Open `Code for ESP32 Connected to Sensor` in Arduino IDE
   - Configure your WiFi credentials
   - Select ESP32 as the board
   - Upload the sketch

3. Start the web server and access the dashboard

## Usage

Once everything is set up:
- The ESP32 continuously monitors the water level
- Data is transmitted to the web server
- Access the dashboard from any device on your network
- Monitor water levels in real-time and receive alerts

## Project Structure

```
.
├── README.md                              # This file
└── Code for ESP32 Connected to Sensor     # ESP32 firmware code
```

## Configuration

Edit the ESP32 code to customize:
- WiFi SSID and Password
- GPIO pins for sensor connection
- Measurement calibration values
- Update intervals

## Troubleshooting

- **No readings**: Check sensor connections and GPIO pin assignments
- **WiFi issues**: Verify SSID/password and signal strength
- **Inaccurate readings**: Recalibrate sensor distance offsets

## Contributing

Contributions are welcome! Feel free to fork this project and submit pull requests.

## License

This project is open source. See LICENSE file for details.

## Support

For issues, questions, or suggestions, please open an issue on GitHub.

---

**Note**: This is an ongoing project for home water tank monitoring. Stay tuned for more features and improvements!
