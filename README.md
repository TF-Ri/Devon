# Devon — Development Hardware Inventory

A cataloged inventory of development hardware, tools, and components with detailed documentation, specifications, and development project ideas for each item.

## Inventory

| # | Device | Type | Images | Category |
|---|--------|------|--------|----------|
| 1 | [STM32F469I-DISCO](devices/stm32f469i-disco/README.md) | Discovery Board | 1 | Dev Board |
| 2 | [Analog Devices ToF Camera](devices/analog-devices-tof-camera/README.md) | Depth Camera Module | 1 | Sensor |
| 3 | [Slamtec RPLIDAR S2M1-R2](devices/slamtec-rplidar-s2m1/README.md) | 2D LiDAR Scanner | 1 | Sensor |
| 4 | [ST BlueNRG-LP + STEVAL-MKI221V1](devices/st-bluenrg-lp-steval-mki221v1/README.md) | BLE Sensor Eval Kit | 1 | Dev Board |
| 5 | [ST SensorTile.box](devices/st-sensortile-box/README.md) | Wireless Sensor Kit | 1 | Dev Board |
| 6 | [STEVAL-STWINBX CS1A](devices/st-steval-stwinbx-cs1a/README.md) | Industrial Sensor Node | 1 | Dev Board |
| 7 | [BLE Camera Module](devices/ble-camera-module/README.md) | Wireless Camera/Sensor | 2 | Sensor |
| 8 | [Arduino UNO R4 WiFi](devices/arduino-uno-r4-wifi/README.md) | Microcontroller Board | 1 | Dev Board |
| 9 | [MIL-Spec Connectors](devices/mil-spec-connectors/README.md) | Circular Connectors | 2 | Connector |
| 10 | [DJI Mavic Pro Controller](devices/dji-mavic-pro-controller/README.md) | Drone Remote | 3 | UAV |
| 11 | [MIL Dome Light MS-51073-1](devices/mil-dome-light-ms51073/README.md) | Military Dome Light | 2 | Tactical |
| 12 | [ASUS ROG Strix GL503V](devices/asus-rog-strix-gl503v/README.md) | Gaming Laptop | 1 | Computer |
| 13 | [ASUS ZenBook UX3407Q](devices/asus-zenbook-ux3407q/README.md) | Ultrabook | 1 | Computer |
| 14 | [Custom Desktop JT-C1](devices/custom-desktop-jt-c1/README.md) | Desktop Workstation | 1 | Computer |
| 15 | [ASUS ROG Zephyrus G814](devices/asus-rog-zephyrus-g814/README.md) | Gaming Laptop | 1 | Computer |
| 16 | [Corning Fiber Optic Cables](devices/corning-fiber-optic/README.md) | Fiber Cables | 2 | Networking |
| 17 | [LiPo Batteries](devices/lipo-batteries/README.md) | 3.7V LiPo Cells | 2 | Power |
| 18 | [NVG Mounting System](devices/nvg-mounting-system/README.md) | J-Arm + VAS Shroud | 2 | Tactical |
| 19 | [Electronics Components Kit](devices/electronics-components-kit/README.md) | Connectors & Supplies | 1 | Components |
| 20 | [SK Hynix SH920 512GB SSD](devices/sk-hynix-sh920-ssd/README.md) | 2.5" SATA SSD | 1 | Storage |
| 21 | [Google Chromecast 2nd Gen](devices/google-chromecast-2nd-gen/README.md) | Streaming Dongle | 1 | Media |
| 22 | [Seeed XIAO nRF52840](devices/seeed-xiao-nrf52840/README.md) | BLE Dev Board | 1 | Dev Board |

**Total: 22 items | 31 images**

## Repository Structure

```
Devon/
  devices/
    stm32f469i-disco/            # STM32 Discovery board with 4" touchscreen
    analog-devices-tof-camera/   # Depth-sensing camera module
    slamtec-rplidar-s2m1/        # 360-degree LiDAR scanner
    st-bluenrg-lp-steval-mki221v1/ # BLE + sensor evaluation stack
    st-sensortile-box/           # Compact wireless sensor kit
    st-steval-stwinbx-cs1a/      # Industrial WiFi/BLE sensor node
    ble-camera-module/           # Wireless camera/sensor module
    arduino-uno-r4-wifi/         # Arduino with WiFi and LED matrix
    mil-spec-connectors/         # Military circular connectors
    dji-mavic-pro-controller/    # DJI drone remote controller
    mil-dome-light-ms51073/      # MIL-L-45068 24V military dome light
    asus-rog-strix-gl503v/       # ROG gaming laptop (GTX 1060/1070)
    asus-zenbook-ux3407q/        # ZenBook ultrabook
    custom-desktop-jt-c1/        # i9-9900K + RTX 5070 workstation
    asus-rog-zephyrus-g814/      # ROG Zephyrus G14 (2024)
    corning-fiber-optic/         # Single-mode fiber cables (SC/APC)
    lipo-batteries/              # 3.7V LiPo cells (250-480mAh)
    nvg-mounting-system/         # J-arm + OpsCore VAS shroud
    electronics-components-kit/  # Powerpole connectors, heat shrink
    sk-hynix-sh920-ssd/          # 512GB 2.5" SATA SSD
    google-chromecast-2nd-gen/   # Google Cast streaming dongle
    seeed-xiao-nrf52840/         # Nordic nRF52840 BLE dev board
  README.md              # This file — master inventory
  CLAUDE.md              # Claude Code development guide
  LICENSE                # Apache 2.0
  .gitignore             # Excludes temp files and artifacts
```

## Categories

### Dev Boards (6)
STM32F469I-DISCO, BlueNRG-LP + MKI221V1, SensorTile.box, STEVAL-STWINBX, Arduino UNO R4 WiFi, Seeed XIAO nRF52840

### Sensors (3)
Analog Devices ToF Camera, Slamtec RPLIDAR S2M1, BLE Camera Module

### Computers (4)
ASUS ROG Strix GL503V, ASUS ZenBook UX3407Q, Custom Desktop JT-C1, ASUS ROG Zephyrus G814

### Connectivity & Networking (2)
Corning Fiber Optic Cables, Google Chromecast 2nd Gen

### UAV (1)
DJI Mavic Pro Controller GL200A

### Tactical (2)
NVG Mounting System (J-Arm + VAS Shroud), MIL Dome Light MS-51073-1

### Components & Accessories (4)
MIL-Spec Connectors, LiPo Batteries, Electronics Components Kit, SK Hynix SSD

## Development Workflow

This repository is set up for iterative development using Claude Code CLI. See [CLAUDE.md](CLAUDE.md) for the brainstorming and development workflow.

Each device directory contains:
- **images/** — Converted JPG photos of the device
- **README.md** — Detailed specs, interfaces, capabilities, and project ideas

As development progresses, each device folder can grow with:
- **projects/** — Code and firmware for specific development projects
- **docs/** — Additional documentation, datasheets, pinout diagrams
- **scripts/** — Utility scripts for interfacing with the device

## License

Apache 2.0 — See [LICENSE](LICENSE)
