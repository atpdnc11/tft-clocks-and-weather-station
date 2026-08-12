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
   git clone https://github.com/atpdnc11/tft-clocks-and-weather-station
