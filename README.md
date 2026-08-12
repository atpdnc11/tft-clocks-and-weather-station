# tft-clocks-and-weather-station

ESP32-C3 Mini Demo Codes
========================

This collection contains Arduino sketches for the ESP32-C3 Mini board,
covering RGB LED animations and NTP OLED clock projects with WiFi features.

Folder Contents:
----------------
1. RGB_Blink.ino
   - Simple RGB LED cycle (Red → Green → Blue → White).
   - Works with discrete RGB pins.

2. RGB_Rainbow.ino
   - Smooth rainbow fade animation across colors.
   - Two versions: discrete pins and WS2812 NeoPixel.

3. RGB_Breathing.ino
   - Rainbow fade with breathing brightness effect.
   - LED pulses in and out for a natural look.

4. NTP_OLED_Clock.ino
   - Basic internet-synced clock using NTP.
   - Displays time and date on SSD1306 OLED.

5. NTP_OLED_AutoWiFi.ino
   - Auto-reconnects to last saved WiFi network.
   - Falls back to AP mode if none is saved.

6. NTP_OLED_WiFiManager.ino
   - Uses WiFiManager library for captive portal setup.
   - Lets you configure WiFi credentials from your phone.

7. NTP_OLED_Battery.ino
   - Adds battery percentage indicator to OLED clock.
   - Reads battery voltage via ADC pin and maps to %.

Usage Notes:
------------
- Install required libraries:
  * Adafruit_GFX
  * Adafruit_SSD1306
  * Adafruit_NeoPixel (for WS2812 LED)
  * WiFiManager (for captive portal)

- Adjust pin numbers for your board’s RGB LED wiring.
- For battery monitoring, connect Li-ion battery via voltage divider to ADC pin.
- Timezone offset (gmtOffset_sec) is set for India Standard Time (UTC+5:30).
  Change if needed.

How to Run:
-----------
1. Open any `.ino` file in Arduino IDE.
2. Select "ESP32-C3 Dev Module" as the board.
3. Upload the sketch.
4. Enjoy the demo!

Author:
-------
Prepared for ESP32-C3 Mini demo projects.
