# Fuel Gauge

*Fuel level on a round panel, read from the car over CAN: an arc that fills and a pointer that rides it.*

![Fuel Gauge, Fuel](screens/01-fuel.png)

A fuel gauge for a 240 x 240 round panel, fed from the diagnostic socket over CAN.

The arc fills with the level and carries a pointer round with it. The pointer is a picture named as the arc's Follower: the arc moves it whenever the value moves and turns it so its tip keeps pointing in at the arc, which is the part a plain knob cannot do. The graduations inside are a Scale's own ticks, with the reserve marked as a section of it.

The arc is not clickable, because a gauge is not a control: a finger on the glass must not move it. Below fifteen per cent a LOW banner comes up.

It reads PID 2F. Not every car reports fuel level over OBD-II; one that does not leaves this at empty, and the device takes a signal of your own for the frame your car puts it in instead.

## Hardware and build

- **Board:** [ESP32-S3 + GC9A01 1.28" round](https://lcdwizard.com/boards/s3-gc9a01-round)
- **MCU:** ESP32-S3
- **Display:** GC9A01 / GC9A01A 240 x 240, CST816S touch
- **Graphics library:** GFX Library for Arduino
- **LVGL:** 9
- **Exports to:** Arduino (C++)
- **Peripherals:** CAN bus / OBD-II (car diagnostics)
- **Libraries:** lvgl, GFX Library for Arduino
- **Screens:** 1

## Open it

1. Open the designer: https://app.lcdwizard.com/app (nothing to install, no account needed).
2. **File > Open project file** and choose `design.json` from this folder.
3. Change what you like, then **Export code** for a project that builds for the board.

Or open a copy straight from the gallery: https://lcdwizard.com/p/obd-fuel-gauge

## Artwork

The images this design uses, as the original files. They are also inside `design.json`, so the design opens without them.

- [`assets/gauge-fuel-face.png`](assets/gauge-fuel-face.png) - 240 x 240
- [`assets/gauge-pointer.png`](assets/gauge-pointer.png) - 22 x 18
