# esphome-weather-station
# ESPHome Weather station
This project contains the source code for a weather station built with ESPHome using an ESP32-POE board and several sensors for monitoring wind speed, wind direction, and rainfall. The weather station collects real-time data and can be integrated into platforms like Home Assistant for further automation and monitoring.

## Features
* **ESP32-POE** as the main controller.
* **WH-SP-WS01** sensor for wind speed.
* **WH-SP-WD** sensor for wind direction.
* **MS-WH-SP-RG** sensor for rainfall measurement.
* Real-time weather data collection and monitoring.
* Seamless integration with platforms such as Home Assistant.
* POE support for both power and network connectivity.

## Hardware Requirements
* **ESP32-POE**: A microcontroller with built-in support for Power-over-Ethernet (PoE).
* **WH-SP-WS01**: Wind speed sensor.
* **WH-SP-WD**: Wind direction sensor.
* **MS-WH-SP-RG**: Rain gauge sensor.
* Ethernet cable (for PoE power and connectivity).
* Enclosure (for protection, if installed outdoors).

## Software Requirements
* ESPHome: To program the ESP32-POE and configure the sensors.
* Home Assistant (optional): For visualizing the data and automating weather-related actions.

## Setup Instructions
### Clone this repository

``` bash
git clone https://github.com/rici4kubicek/esphome-weather-station.git
cd meteostation-esphome
```

### Install ESPHome
If you don't already have ESPHome installed, you can install it with:

``` bash
pip install esphome
```

### Configure the ESP32-POE
Update the esphome.yaml file with your specific network settings and any additional sensor configurations as needed.

### Upload the firmware to the ESP32-POE
Connect your ESP32-POE via USB and run:

```bash
esphome run esphome.yaml
```

### Integrate with Home Assistant (optional)
Add the ESPHome integration in Home Assistant to monitor your weather station's data on the Home Assistant dashboard.

## Sensor Overview
### WH-SP-WS01 (Wind Speed Sensor)
Captures the current wind speed. Essential for tracking real-time wind conditions.

### WH-SP-WD (Wind Direction Sensor)
Measures the wind's direction, giving insight into weather patterns.

### MS-WH-SP-RG (Rain Gauge)
Measures rainfall over time. Provides information on the amount of precipitation in your area.
