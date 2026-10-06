# LCD Wizard examples

18 LVGL designs for ESP32 display boards, made in [LCD Wizard](https://lcdwizard.com). Each folder holds the design as `design.json`, a picture of every screen, and the artwork where it has any. Open one in the designer with **File > Open project file**, change it, and export a project that builds for the board: Arduino or PlatformIO, MicroPython, or ESPHome, depending on the design.

| | Example | Board | Builds with | Screens |
|---|---|---|---|---|
| <img src="examples/neon-deck/screens/01-radio.png" width="160" alt=""> | [**NEON DECK**](examples/neon-deck)<br>An internet radio with real VU meters, a station list and WiFi setup on the panel. | [LCDWIKI 2.8" ESP32-32E (E32R28T)](https://lcdwizard.com/boards/lcdwiki-e32r28t) | Arduino (C++) | 4 |
| <img src="examples/orbital/screens/01-radio.png" width="160" alt=""> | [**ORBITAL**](examples/orbital)<br>A deep-space internet radio with a HUD volume dial, live bitrate and VU meters, for a 3.5" ESP32-S3 with a proper audio codec. | [LCDWIKI 3.5" ESP32-S3 (ES3C35P)](https://lcdwizard.com/boards/lcdwiki-es3c35p) | Arduino (C++) | 4 |
| <img src="examples/hello-cyd/screens/01-screen1.png" width="160" alt=""> | [**Hello CYD**](examples/hello-cyd)<br>A dial, a readout and a button. Nothing to wire - press Play and drag something. | [ESP32-2432S028R "Cheap Yellow Display"](https://lcdwizard.com/boards/cyd-2432s028r) | Arduino (C++) | 1 |
| <img src="examples/cyd-weather/screens/01-screen1.png" width="160" alt=""> | [**Desk Weather**](examples/cyd-weather)<br>BME280 on the CN1 connector: temperature, humidity, pressure and a rolling chart. | [ESP32-2432S028R "Cheap Yellow Display"](https://lcdwizard.com/boards/cyd-2432s028r) | Arduino (C++) | 1 |
| <img src="examples/cyd-air/screens/01-screen1.png" width="160" alt=""> | [**Air Quality**](examples/cyd-air)<br>SCD40 CO2 plus a BH1750 light sensor, with a verdict that changes colour. | [ESP32-2432S028R "Cheap Yellow Display"](https://lcdwizard.com/boards/cyd-2432s028r) | Arduino (C++) | 1 |
| <img src="examples/cyd-mood/screens/01-screen1.png" width="160" alt=""> | [**Mood Light**](examples/cyd-mood)<br>Drive the CYD's onboard RGB LED from the touchscreen, and let it turn itself on at dusk. | [ESP32-2432S028R "Cheap Yellow Display"](https://lcdwizard.com/boards/cyd-2432s028r) | Arduino (C++) | 1 |
| <img src="examples/bench-meter/screens/01-live.png" width="160" alt=""> | [**Bench Supply Meter**](examples/bench-meter)<br>Volts, amps and watts from an INA219, with a current limit you set on the panel. | [ESP32 + ILI9341 2.8" SPI](https://lcdwizard.com/boards/esp32-ili9341-spi) | ESPHome | 2 |
| <img src="examples/thermostat/screens/01-main.png" width="160" alt=""> | [**Heating Thermostat**](examples/thermostat)<br>A room thermostat with a dial, hysteresis, and a boost that expires by itself. | [ESP32-2432S028C (capacitive CYD)](https://lcdwizard.com/boards/cyd-2432s028c) | ESPHome | 2 |
| <img src="examples/wall-panel/screens/01-screen1.png" width="160" alt=""> | [**Lighting Wall Panel**](examples/wall-panel)<br>Four rooms, a dimmer and an all-off, published to Home Assistant as entities. | [WT32-SC01](https://lcdwizard.com/boards/wt32-sc01) | ESPHome | 1 |
| <img src="examples/pocket-meter/screens/01-screen1.png" width="160" alt=""> | [**Pocket Hygrometer**](examples/pocket-meter)<br>Temperature, humidity and dew point on a 170 x 320 strip. | [LilyGO T-Display-S3](https://lcdwizard.com/boards/lilygo-tdisplay-s3) | ESPHome | 1 |
| <img src="examples/greenhouse/screens/01-main.png" width="160" alt=""> | [**Greenhouse Watering**](examples/greenhouse)<br>Soil moisture on the ADC, a pump on a relay, and a lockout so it cannot flood the bench. | [ESP32-S3 + ILI9341 SPI](https://lcdwizard.com/boards/s3-ili9341-spi) | MicroPython | 2 |
| <img src="examples/shot-timer/screens/01-screen1.png" width="160" alt=""> | [**Espresso Shot Timer**](examples/shot-timer)<br>A big readable number, a target band, and the last shot to compare against. | [M5Stack Core2](https://lcdwizard.com/boards/m5stack-core2) | MicroPython | 1 |
| <img src="examples/round-knob/screens/01-screen1.png" width="160" alt=""> | [**Round Volume Knob**](examples/round-knob)<br>A machined knob on a 240 x 240 round panel: turn the dimple, press the middle to mute. | [ESP32-S3 + GC9A01 1.28" round](https://lcdwizard.com/boards/s3-gc9a01-round) | MicroPython | 1 |
| <img src="examples/obd-coolant-gauge/screens/01-coolant.png" width="160" alt=""> | [**Coolant Gauge**](examples/obd-coolant-gauge)<br>Engine temperature on a round panel, read from the car over CAN: a real needle on a real scale. | [ESP32-S3 + GC9A01 1.28" round](https://lcdwizard.com/boards/s3-gc9a01-round) | Arduino (C++) | 1 |
| <img src="examples/obd-fuel-gauge/screens/01-fuel.png" width="160" alt=""> | [**Fuel Gauge**](examples/obd-fuel-gauge)<br>Fuel level on a round panel, read from the car over CAN: an arc that fills and a pointer that rides it. | [ESP32-S3 + GC9A01 1.28" round](https://lcdwizard.com/boards/s3-gc9a01-round) | Arduino (C++) | 1 |
| <img src="examples/reflow-oven/screens/01-run.png" width="160" alt=""> | [**Reflow Oven Controller**](examples/reflow-oven)<br>A lead-free profile, a thermocouple on SPI, and a chart of what the oven actually did. | [STM32F407 + ILI9341 SPI](https://lcdwizard.com/boards/stm32f407-ili9341) | Arduino (C++) | 1 |
| <img src="examples/dust-extraction/screens/01-screen1.png" width="160" alt=""> | [**Dust Extraction Panel**](examples/dust-extraction)<br>Four blast gates on an I2C expander, an extractor that follows them, and a filter that says when it is blocked. | [Sunton ESP32-8048S043 (4.3" RGB)](https://lcdwizard.com/boards/sunton-8048s043) | Arduino (C++) | 1 |
| <img src="examples/solar-dashboard/screens/01-screen1.png" width="160" alt=""> | [**Solar Dashboard**](examples/solar-dashboard)<br>Array, house, battery and net power, with a day of history on one chart. | [Sunton ESP32-8048S070 (7" RGB)](https://lcdwizard.com/boards/sunton-8048s070) | Arduino (C++) | 1 |

## Using a design

1. Open the designer at https://app.lcdwizard.com/app. It runs in the browser and needs no account to design or open a file.
2. **File > Open project file**, and pick an example's `design.json`.
3. Press **Play** to try it with simulated readings, or **Export code** for the project.

The same designs are in the [gallery](https://lcdwizard.com/gallery), where **Open a copy** does the same in one click.

## Contributing

Made something with LCD Wizard? Publish it to the gallery from the designer, or open a pull request here with its `design.json` and a screenshot.

## Licence

© 2026 Jonathan Harrocks (LCD Wizard). [MIT](LICENSE): use the designs, and anything you build from them, for anything. Fonts and icons the designs use carry their own licences (SIL OFL 1.1 and the Unlicense), noted inside each export.

[![Designed with LCD Wizard](https://lcdwizard.com/img/badge.svg)](https://lcdwizard.com)
