# Hardware

Known hardware plans for Wisteria. Specifications not listed here are **not yet decided**.

## Overview

Wisteria is a battery-powered pocket e-reader built around an ESP32-class microcontroller and an E Ink display.

## Development hardware

| Item | Details |
|------|---------|
| Board | ESP32 CYD (Cheap Yellow Display) |
| Role | Firmware development and prototyping |
| Notes | Not the final product form factor |

## Target hardware (planned)

### Display

- **Type:** E Ink
- **Size:** Approximately 4.7 inches
- **Model:** Not yet selected

### Storage

- **Type:** microSD card
- **Purpose:** On-device book library
- **Status:** Planned

### Input

- **Type:** Physical buttons
- **Purpose:** Page turning (and minimal navigation)
- **Status:** Planned
- **Pin assignments:** TBD

### Power

- **Operation:** Battery-powered
- **Charging:** USB-C
- **Battery chemistry, capacity, and charging IC:** TBD

### Microcontroller

- **Family:** ESP32 (confirmed for development)
- **Final board/module selection:** TBD

## Mechanical

Enclosure and button designs live in `cad/`. Dimensions, materials, and assembly method are **TBD**.

## Documentation locations

| Directory | Contents |
|-----------|----------|
| `hardware/schematics/` | Circuit schematics |
| `hardware/wiring/` | Wiring diagrams |
| `hardware/pinouts/` | GPIO and connector pin assignments |
| `cad/case/` | Main enclosure |
| `cad/buttons/` | Page-turn button parts |
| `cad/cover/` | Cover or lid design |

## Open questions

- Final E Ink display model and driver requirements
- ESP32 module vs. custom PCB
- Battery and charging circuit design
- Button placement and ergonomics for pocket use
- SD card slot type (full-size vs. micro)
