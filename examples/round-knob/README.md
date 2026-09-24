# Round Volume Knob

*A 240 x 240 round panel as a dial: everything centred, no corners to use.*

![Round Volume Knob, Screen1](screens/01-screen1.png)

A round panel is a different layout problem, and worth one example on its own.

There are no corners to put anything in, so everything is centred and the arc does the work the edges would. The dial writes the level and reads it back, so the number in the middle is the value the firmware holds - which is the pattern for anything the user sets and something else then acts on.

Mute is a separate variable rather than level zero, so unmuting returns to where the dial was rather than to silence.

## Hardware and build

- **Board:** [ESP32-S3 + GC9A01 1.28" round](https://lcdwizard.com/boards/s3-gc9a01-round)
- **MCU:** ESP32-S3
- **Display:** GC9A01 / GC9A01A 240 x 240, CST816S touch
- **Graphics library:** GFX Library for Arduino
- **LVGL:** 9
- **Exports to:** MicroPython
- **Libraries:** lvgl, GFX Library for Arduino
- **Screens:** 1

## Open it

1. Open the designer: https://app.lcdwizard.com/app (nothing to install, no account needed).
2. **File > Open project file** and choose `design.json` from this folder.
3. Change what you like, then **Export code** for a project that builds for the board.

Or open a copy straight from the gallery: https://lcdwizard.com/p/round-knob
