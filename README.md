# tft-clocks-and-weather-station

# 🕒 TFT Clocks and Weather Station

### Author: Arvind Patil  
### Location: Nandurbar, Maharashtra, India  

## Overview
This project demonstrates how to use an **ILI9341 TFT display** with Arduino/ESP32 to show:
- Digital Clock (HH:MM:SS)
- Weather Station (Temperature + Humidity via DHT sensor)

## Features
- Modular functions for TFT setup, clock, and weather display
- Color-coded UI (green for time, cyan for weather)
- Error handling for sensor failures
- Easy to extend with battery/Wi-Fi status

## Hardware Requirements
- Arduino UNO / ESP32 board
- ILI9341 TFT display (SPI)
- DHT11/DHT22 sensor

## Software Requirements
- Adafruit GFX Library
- Adafruit ILI9341 Library
- DHT sensor library

## Setup
1. Clone the repo:
   ```bash
 Here’s the pin‑mapping table you can add to your README so users can adapt wiring easily across boards. This complements the wiring diagram graphic and makes your repo beginner‑friendly.

📌 Pin Mapping Table
TFT Pin	Arduino UNO	ESP32 (default SPI)	Notes
VCC	3.3V	3.3V	⚠️ Use 3.3V only (ILI9341 is not 5V tolerant)
GND	GND	GND	Common ground
CS	D10	GPIO5	Chip Select
DC (RS)	D9	GPIO2	Data/Command
RST	D8	GPIO4	Reset
MOSI	D11	GPIO23	SPI MOSI
MISO	D12	GPIO19	SPI MISO
SCK	D13	GPIO18	SPI Clock


DHT11/DHT22 Sensor
Sensor Pin	Arduino UNO	ESP32	Notes
VCC	5V	3.3V	DHT works with both 3.3V/5V
GND	GND	GND	Common ground
DATA	D2	GPIO21	Requires 10k pull‑up resistor  git clone https://github.com/atpdnc11/tft-clocks-and-weather-station
## Pin Mapping

### TFT Display (ILI9341)
| TFT Pin | Arduino UNO | ESP32 | Notes |
|---------|-------------|-------|-------|
| VCC     | 3.3V        | 3.3V  | ⚠️ Use 3.3V only |
| GND     | GND         | GND   | Common ground |
| CS      | D10         | GPIO5 | Chip Select |
| DC      | D9          | GPIO2 | Data/Command |
| RST     | D8          | GPIO4 | Reset |
| MOSI    | D11         | GPIO23| SPI MOSI |
| MISO    | D12         | GPIO19| SPI MISO |
| SCK     | D13         | GPIO18| SPI Clock |

### DHT Sensor
| Pin | Arduino UNO | ESP32 | Notes |
|-----|-------------|-------|-------|
| VCC | 5V          | 3.3V  | Works with both |
| GND | GND         | GND   | Common ground |
| DATA| D2          | GPIO21| Needs 10k pull‑up resistor |

