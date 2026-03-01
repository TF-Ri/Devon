# Seeed XIAO nRF52840

## Overview
The Seeed XIAO nRF52840 is an ultra-compact Bluetooth Low Energy (BLE) development board built around the Nordic Semiconductor nRF52840 SoC. At just 21x17.5mm, it's one of the smallest development boards available with full BLE 5.0, NFC, and USB-C support. The board features a powerful ARM Cortex-M4F processor with floating-point unit, 1MB flash, and 256KB RAM — all in a breadboard-friendly thumb-sized package. Part of the Seeed Studio XIAO series, it maintains the same compact pinout footprint as other XIAO boards for drop-in compatibility.

## Identification
| Field | Value |
|-------|-------|
| Manufacturer | Seeed Studio |
| Model | XIAO-nRF52840 |
| SoC | Nordic nRF52840 |
| Type | BLE Microcontroller Board |
| Buttons | RST (Reset), USR (User) |
| Connector | USB-C |
| Form Factor | 21 x 17.5 mm |

## Images
| Image | Description |
|-------|-------------|
| *(Add image)* | Top view on Seeed carrier board showing XIAO-nRF52840 label, USB-C port, RST and USR buttons, Seeed logo |

## Technical Specifications
- **SoC**: Nordic nRF52840
  - ARM Cortex-M4F @ 64 MHz
  - Floating Point Unit (FPU)
  - 1 MB Flash
  - 256 KB RAM
- **Wireless**: Bluetooth 5.0 / BLE, NFC, Zigbee, Thread, ANT, 802.15.4
- **USB**: USB-C (native USB via nRF52840 USB peripheral)
- **GPIO**: 11 digital pins, 6 analog pins (12-bit ADC)
- **Communication**: UART, I2C, SPI
- **PWM**: 11 channels
- **Buttons**: RST (reset), USR (user-programmable)
- **LEDs**: 3 built-in LEDs (power, charging, user)
- **Power**: USB-C (5V), 3.3V logic, battery charging circuit
- **Battery**: JST connector for 3.7V LiPo with on-board charging
- **Current Draw**: ~5 mA active, ~5 uA deep sleep
- **Dimensions**: 21 x 17.5 mm
- **Operating Temp**: -40°C to +85°C

## Development Interfaces
- **USB-C**: Programming, power, serial debug, native USB HID/CDC
- **SWD**: Debug pads on bottom (SWDIO, SWCLK, RST, GND, 3V3)
- **UART**: TX/RX on GPIO pins
- **I2C**: SDA/SCL with internal pull-ups
- **SPI**: MOSI/MISO/SCK/CS
- **ADC**: 6 channels, 12-bit resolution
- **NFC**: NFC antenna pads (NFC1/NFC2)
- **PDM**: Digital microphone interface
- **I2S**: Digital audio interface
- **Battery**: 3.7V LiPo charging via USB-C

## Capabilities
- Bluetooth 5.0 with long range (coded PHY) and high throughput (2 Mbps PHY)
- Native USB HID (keyboard, mouse, gamepad emulation)
- NFC tag emulation and reader mode
- Ultra-low power deep sleep (~5 uA) for battery applications
- Zigbee/Thread mesh networking (802.15.4)
- TinyML capable (TensorFlow Lite Micro)
- On-board LiPo battery management
- IMU support (nRF52840 Sense variant has LSM6DS3TR-C)
- Arduino, CircuitPython, MicroPython, Zephyr RTOS support
- Breadboard-friendly pinout

## Potential Development Projects
1. **BLE Beacon Network**: Deploy multiple XIAO units as BLE beacons for indoor positioning or asset tracking
2. **Wireless HID Controller**: Build a custom USB/BLE keyboard, mouse, or game controller using native USB HID
3. **TinyML Sensor Node**: Run TensorFlow Lite Micro for edge AI inference on sensor data with BLE reporting
4. **NFC Smart Tag**: Create programmable NFC tags for access control, data sharing, or automation triggers
5. **Mesh Sensor Network**: Use Zigbee/Thread to build a low-power mesh network of environmental sensors
6. **Wearable Health Monitor**: Combine with pulse/SpO2 sensor and LiPo battery for a tiny BLE health wearable
7. **BLE-UART Bridge**: Create a wireless serial bridge for debugging other embedded devices
8. **Portable Battery Monitor**: Use ADC inputs to monitor and report LiPo battery health over BLE

## Getting Started

### Required Tools
- USB-C cable
- Arduino IDE 2.x or PlatformIO
- Seeed nRF52840 board package for Arduino
- nRF Connect app (iOS/Android) for BLE testing
- Optional: J-Link or DAPLink for SWD debugging

### Initial Setup
1. Connect via USB-C — the board appears as a USB serial device
2. Install Arduino IDE and add Seeed nRF52840 board support:
   - Add board manager URL: `https://files.seeedstudio.com/arduino/package_seeeduino_boards_index.json`
   - Install "Seeed nRF52 mbed-enabled Boards" package
3. Select "Seeed XIAO nRF52840" as the board
4. Upload the Blink example to verify the toolchain
5. Install nRF Connect on your phone and scan for BLE devices
6. Upload the BLE Peripheral example to test wireless connectivity
7. For advanced: install Zephyr RTOS for full nRF52840 SDK access

### Alternative Frameworks
- **CircuitPython**: Flash the CircuitPython UF2 bootloader for Python scripting
- **MicroPython**: Flash MicroPython firmware for interactive development
- **Zephyr RTOS**: Use the Nordic nRF Connect SDK for production-grade BLE stacks
- **nRF5 SDK**: Direct Nordic SDK access for maximum control

## References
- [Seeed XIAO nRF52840 Wiki](https://wiki.seeedstudio.com/XIAO_BLE/)
- [Nordic nRF52840 Product Page](https://www.nordicsemi.com/Products/nRF52840)
- [nRF52840 Datasheet (PDF)](https://infocenter.nordicsemi.com/pdf/nRF52840_PS_v1.1.pdf)
- [Seeed Arduino Board Package](https://github.com/Seeed-Studio/Adafruit_nRF52_Arduino)
- [CircuitPython for XIAO nRF52840](https://circuitpython.org/board/seeeduino_xiao_nrf52840/)
- [Zephyr RTOS nRF52840 Support](https://docs.zephyrproject.org/latest/boards/arm/nrf52840dk_nrf52840/)
