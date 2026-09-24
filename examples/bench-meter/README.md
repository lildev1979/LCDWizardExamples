# Bench Supply Meter

*Volts, amps and watts from an INA219, with a current limit you set on the panel.*

![Bench Supply Meter, Live](screens/01-live.png)

A bench supply with no display, given one that reads better than most.

An INA219 sits across the output and reports voltage, current and power over I2C. The live screen is three tiles and a bar; the second sets the current you want warning about, which is a variable the spinbox writes and an automation reads.

Nothing is switched: an INA219 measures, it does not interrupt. The banner tells you, and what you do about it is yours.

Exports as ESPHome, so there is no compiler to install - one command flashes it.

## Hardware and build

- **Board:** [ESP32 + ILI9341 2.8" SPI](https://lcdwizard.com/boards/esp32-ili9341-spi)
- **MCU:** ESP32 (WROOM / WROVER)
- **Display:** ILI9341 240 x 320, XPT2046 touch
- **Graphics library:** TFT_eSPI
- **LVGL:** 9
- **Exports to:** ESPHome
- **Peripherals:** INA219 (current)
- **Libraries:** lvgl, TFT_eSPI, Adafruit INA219
- **Screens:** 2

## Open it

1. Open the designer: https://app.lcdwizard.com/app (nothing to install, no account needed).
2. **File > Open project file** and choose `design.json` from this folder.
3. Change what you like, then **Export code** for a project that builds for the board.

Or open a copy straight from the gallery: https://lcdwizard.com/p/bench-meter

## Screens

### Live

![Live](screens/01-live.png)

### Limits

![Limits](screens/02-limits.png)

