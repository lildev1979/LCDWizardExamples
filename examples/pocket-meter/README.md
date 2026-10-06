# Pocket Hygrometer

*Temperature, humidity and dew point on a 170 x 320 strip.*

![Pocket Hygrometer, Screen1](screens/01-screen1.png)

The T-Display-S3 is a strip, not a screen: 170 x 320. Everything stacks, and a layout that works on a CYD falls off the edge here - which is the point of having one example shaped like this.

An SHT31 reads temperature and humidity; dew point is arithmetic on the two, done in a formula rather than by a third sensor. The marker under the humidity rides a scale of too dry, comfortable and too damp.

Exports as ESPHome. The panel is 8-bit parallel, which ESPHome drives as an octal SPI bus - so this one needs an S2 or S3, and the T-Display-S3 is one.

## Hardware and build

- **Board:** [LilyGO T-Display-S3](https://lcdwizard.com/boards/lilygo-tdisplay-s3)
- **MCU:** ESP32-S3
- **Display:** ST7789 170 x 320, CST816S touch
- **Graphics library:** GFX Library for Arduino
- **LVGL:** 9
- **Exports to:** ESPHome
- **Peripherals:** SHT31 / SHT35
- **Libraries:** lvgl, GFX Library for Arduino, Adafruit SHT31 Library
- **Screens:** 1

## Open it

1. Open the designer: https://app.lcdwizard.com/app (nothing to install, no account needed).
2. **File > Open project file** and choose `design.json` from this folder.
3. Change what you like, then **Export code** for a project that builds for the board.

Or open a copy straight from the gallery: https://lcdwizard.com/p/pocket-meter

## Artwork

The images this design uses, as the original files. They are also inside `design.json`, so the design opens without them.

- [`assets/panel-pocket.png`](assets/panel-pocket.png) - 170 x 320
