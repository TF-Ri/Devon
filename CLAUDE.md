# Devon — Hardware Inventory Development Guide

## Repository Purpose
This is a development hardware inventory repository. Each subdirectory under `devices/` represents a physical hardware device (or set of related components) with detailed documentation including specifications, development interfaces, capabilities, and brainstormed project ideas.

## Quick Start
- Browse the master inventory: [README.md](README.md)
- Each device: `devices/<device-slug>/README.md`
- Images: `devices/<device-slug>/images/`

## Working with Devices

### Browsing the Inventory
1. Open `README.md` for the full device table with links
2. Navigate to any `devices/<slug>/` directory
3. Read the device README for complete specs and project ideas

### Selecting a Device for Development
When choosing which device to work on:
1. Review the **Capabilities** section to understand what it can do
2. Check **Development Interfaces** to see how to connect and program it
3. Look at **Potential Development Projects** for starter ideas
4. Read **Getting Started** for setup instructions

## Brainstorming Workflow

When brainstorming development projects for a device:

### Phase 1: Understand the Device
- Read the device's README thoroughly
- Note all available interfaces (UART, SPI, I2C, USB, wireless, etc.)
- List the device's unique capabilities and sensors
- Identify the development toolchain (SDK, IDE, language)

### Phase 2: Generate Project Ideas
Consider these categories when brainstorming:
- **Standalone projects**: What can this device do on its own?
- **Cross-device integration**: How can this device work with OTHER devices in the inventory?
- **Data collection**: What data can this device capture or generate?
- **Automation**: What processes can this device automate?
- **Learning projects**: What new skills does developing for this device teach?

### Phase 3: Evaluate and Prioritize
For each project idea, consider:
- Required tools and additional hardware
- Complexity and time investment
- Learning value and skill development
- Practical utility
- Fun factor

### Phase 4: Create the Project
1. Create `devices/<slug>/projects/<project-name>/`
2. Add a project README with goals, architecture, and milestones
3. Implement iteratively — start with the simplest working version
4. Document as you go

## Cross-Device Integration Ideas

The inventory contains complementary devices that can work together:

### Robotics Platform
- **RPLIDAR S2M1** (LiDAR navigation) + **Arduino UNO R4 WiFi** (motor control) + **Analog Devices ToF Camera** (depth sensing)

### IoT Sensor Network
- **STEVAL-STWINBX** (WiFi/BLE sensor node) + **BlueNRG-LP** (BLE beacon) + **SensorTile.box** (additional node) + **Arduino UNO R4 WiFi** (gateway)

### Portable Field Kit
- **LiPo Batteries** (power) + **BLE Camera Module** (imaging) + **NVG Mount** (helmet attachment) + **MIL-Spec Connectors** (rugged wiring)

### Development Workstations
- **Custom Desktop JT-C1** (primary ML/GPU workstation) + **ASUS ROG Zephyrus G814** (portable dev) + **SK Hynix SSD** (additional storage) + **Corning Fiber** (high-speed interconnect)

## Adding New Devices

To add a new device to the inventory:
1. Create `devices/<manufacturer-model>/` directory
2. Add images to `devices/<manufacturer-model>/images/`
3. Create a README following the template in existing device directories
4. Update the master inventory table in `README.md`

### Naming Convention
- Directory names: lowercase kebab-case (`harris-rf-7800v`, `raspberry-pi-4b`)
- Images: Keep original filenames, store in `images/` subdirectory
- Documentation: Markdown format, one `README.md` per device
- Projects: `devices/<slug>/projects/<project-name>/`

## Key Files
| File | Purpose |
|------|---------|
| `README.md` | Master inventory and navigation |
| `CLAUDE.md` | This file — development guide |
| `LICENSE` | Apache 2.0 license |
| `.gitignore` | Excludes temp files and build artifacts |
| `devices/*/README.md` | Individual device documentation |
