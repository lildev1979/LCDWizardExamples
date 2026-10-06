# Desk Weather

*BME280 on the CN1 connector: temperature, humidity, pressure and a rolling chart.*

![Desk Weather, Screen1](screens/01-screen1.png)

A weather station for the corner of a desk.

A BME280 hangs off the CYD's CN1 connector as I2C - GPIO22 is SDA, GPIO27 is SCL, and the other two pins on that plug are 3V3 and ground. The sensor is polled every two seconds, which is slow enough to keep it from warming itself up.

Three variables read the three channels; bindings push them into the ring, the bars and the numbers, and the temperature also feeds an hour of history: sixty points paced a minute apart, whatever rate the sensor is read at.

The plates, the light behind them and the scale inside the ring are one picture, drawn around the layout, and the ring is an arc with no knob - it reports, so a finger on the glass cannot move it.

## Hardware and build

- **Board:** [ESP32-2432S028R "Cheap Yellow Display"](https://lcdwizard.com/boards/cyd-2432s028r)
- **MCU:** ESP32 (WROOM / WROVER)
- **Display:** ILI9341 320 x 240, XPT2046 touch
- **Graphics library:** TFT_eSPI
- **LVGL:** 9
- **Exports to:** Arduino (C++)
- **Peripherals:** BME280
- **Libraries:** lvgl, TFT_eSPI, Adafruit BME280 Library
- **Screens:** 1

## Open it

1. Open the designer: https://app.lcdwizard.com/app (nothing to install, no account needed).
2. **File > Open project file** and choose `design.json` from this folder.
3. Change what you like, then **Export code** for a project that builds for the board.

Or open a copy straight from the gallery: https://lcdwizard.com/p/cyd-weather

## Artwork

The images this design uses, as the original files. They are also inside `design.json`, so the design opens without them.

- [`assets/panel-weather.png`](assets/panel-weather.png) - 240 x 320
