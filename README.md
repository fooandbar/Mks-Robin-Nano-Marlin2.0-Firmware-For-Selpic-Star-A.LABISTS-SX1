# Mks-Robin-Nano-Marlin2.0-Firmware for Star A/LABISTS SX1 3D printer
## Features
The firmware of Star A/LABISTS SX1, based on [Marlin2.0.x](https://github.com/MarlinFirmware/Marlin) and[Marlin2.0-For-Robin-Nano](https://github.com/makerbase-mks/Mks-Robin-Nano-Marlin2.0-Firmware), supporting classical GUI and touch screen. Unfortunately the [LittlevGL](https://github.com/littlevgl/lvgl) is not supported. This firmware requires [a TFT LCD](https://www.amazon.com/dp/B08SGN7WDV) and [a heated bed](https://www.amazon.co.jp/dp/B08TH7SVMH).

## Build
As the firmware is based on Marlin2.0.x which is built on the core of PlatformIO, the buid compiling steps are the same as Marlin2.0.x. You can directly using [PlatformIO Shell Commands](https://docs.platformio.org/en/latest/core/installation.html#piocore-install-shell-commands), or using IDEs contain built-in PlatformIO Core(CLI), for example, [VSCode](https://docs.platformio.org/en/latest/integration/ide/vscode.html#ide-vscode) and [Atom](https://docs.platformio.org/en/latest/integration/ide/atom.html). VSCode is recommended.

### Firmware Can be run with/without [an autoleveling sensor](https://www.thingiverse.com/thing:4831530).
#### With an autoleveling sensor.

1. Build firmware:
2. Update firmware:
   
- Enter the `.pio\build\mks_robin_nano35` directory, copy `Robin_nano35.bin` to the sd card, rename `Robin_nano.bin` . The pre-built firmware can be found [here](https://github.com/fooandbar/Mks-Robin-Nano-Marlin2.0-Firmware/tree/master/Firmware/wBLTOUCH).
- Insert SD card to the motherboard, and you can see the update interface after power on.   

#### Without an autoleveling sensor.

1. Build firmware:

- Configuation.h:
    //#define AUTO_BED_LEVELING_BILINEAR
    //#define BLTOUCH
    //#define Z_MIN_PROBE_USES_Z_MIN_ENDSTOP_PIN

2. Update firmware:
   
- Enter the `.pio\build\mks_robin_nano35` directory, copy `Robin_nano35.bin` to the sd card, rename `Robin_nano.bin` . The pre-built firmware can be found [here](https://github.com/fooandbar/Mks-Robin-Nano-Marlin2.0-Firmware/tree/master/Firmware/woBLTOUCH).
- Insert SD card to the motherboard, and you can see the update interface after power on.   
