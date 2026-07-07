# Architecture

High-level structure of the Wisteria project. Details marked **TBD** are not yet decided.

## Repository layout

| Path | Purpose |
|------|---------|
| `firmware/` | Device firmware (ESP32) |
| `firmware/src/` | Application source |
| `firmware/include/` | Headers |
| `firmware/lib/` | Local libraries and modules |
| `firmware/test/` | Firmware tests |
| `hardware/` | Schematics, wiring diagrams, pinouts |
| `cad/` | Enclosure and mechanical design |
| `assets/` | Fonts, icons, boot imagery, Polish UI strings |
| `docs/` | Project documentation |

## Development platform

**Current:** ESP32 CYD (Cheap Yellow Display)

The CYD is used for early firmware development and prototyping. It is a stand-in for the final hardware, not the target product.

## Target hardware (planned)

| Component | Status |
|-----------|--------|
| Display | ~4.7-inch E Ink — exact model **not yet selected** |
| Storage | microSD for book library (**planned**) |
| Input | Physical page-turn buttons (**planned**) |
| Power | Battery operation with USB-C charging (**planned**) |

## Software layers (planned)

Firmware has not been written yet. The intended layering is:

1. **Hardware abstraction** — Display, SD card, buttons, power management
2. **Reading engine** — Book loading, pagination, progress
3. **UI** — Minimal interface focused on the current page and library
4. **Personalization** — Lightweight touches (boot screen, Polish phrases, etc.)

Exact module boundaries and libraries are **TBD** until hardware is finalized and prototyping begins.

## Data flow (planned)

```
microSD (books) → firmware (parse & paginate) → E Ink display
                      ↑
              physical buttons (page turn)
```

Book formats, parsing libraries, and on-device file layout are **TBD**.

## Out of scope (for now)

- Cloud sync or online book stores
- Wi-Fi features beyond what development requires
- Heavy theming or plugin systems
