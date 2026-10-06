# Mood Light

*Drive the CYD's onboard RGB LED from the touchscreen, and let it turn itself on at dusk.*

![Mood Light, Screen1](screens/01-screen1.png)

The one that makes the board do something.

The CYD already has an RGB LED on GPIO4, GPIO16 and GPIO17. It is common anode, so each pin sinks its colour and the outputs here are configured active-low to match - tap a colour and all three channels are set at once, so what you see is always the whole state of the LED.

A BH1750 on CN1 reads the room. When it drops below 20 lx an automation turns the lamp on by itself.

The only part to buy is the light sensor. Everything else is already soldered to the board.

Three pins that are each on or off make eight states, and all eight are here. The lamp on screen is a disc that takes the colour, two fainter ones behind it for the glow, and a picture of a highlight on top that never changes - so one sprite makes a lit sphere of any colour.

## Hardware and build

- **Board:** [ESP32-2432S028R "Cheap Yellow Display"](https://lcdwizard.com/boards/cyd-2432s028r)
- **MCU:** ESP32 (WROOM / WROVER)
- **Display:** ILI9341 320 x 240, XPT2046 touch
- **Graphics library:** TFT_eSPI
- **LVGL:** 9
- **Exports to:** Arduino (C++)
- **Peripherals:** BH1750 (light)
- **Libraries:** lvgl, TFT_eSPI, BH1750
- **Screens:** 1

## Open it

1. Open the designer: https://app.lcdwizard.com/app (nothing to install, no account needed).
2. **File > Open project file** and choose `design.json` from this folder.
3. Change what you like, then **Export code** for a project that builds for the board.

Or open a copy straight from the gallery: https://lcdwizard.com/p/cyd-mood

## Artwork

The images this design uses, as the original files. They are also inside `design.json`, so the design opens without them.

- [`assets/panel-mood.png`](assets/panel-mood.png) - 240 x 320
- [`assets/lamp-gloss.png`](assets/lamp-gloss.png) - 76 x 76
