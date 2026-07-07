# Roadmap

Phased plan for Wisteria. Dates and ordering are approximate; scope may shift as hardware decisions are made.

## Phase 0 — Repository scaffold ✓

- Project structure, documentation, and asset directories
- Preserve existing README and development `.gitignore`

## Phase 1 — Development platform bring-up

- ESP32 CYD firmware environment (PlatformIO or equivalent — TBD)
- Basic display output on CYD screen
- Validate build, flash, and debug workflow

## Phase 2 — Core reading (CYD)

- Load a book from storage (CYD SD or other — TBD)
- Render text to display
- Page forward / back via input (CYD touch or temporary buttons)

## Phase 3 — Hardware selection

- Choose ~4.7-inch E Ink display model
- Define pinout, wiring, and power budget
- Document in `hardware/` and `docs/Hardware.md`
- Update `docs/Parts.md` with final BOM

## Phase 4 — Target hardware prototype

- Integrate selected E Ink display
- microSD book storage
- Physical page-turn buttons
- Battery and USB-C charging circuit

## Phase 5 — Enclosure

- Case, button, and cover CAD in `cad/`
- Fit check and pocket ergonomics
- Print or fabricate enclosure

## Phase 6 — Polish and personalization

- Boot screen and assets (`assets/boot/`, `assets/icons/`)
- Polish UI strings (`assets/polish/`) — lightweight only
- Fonts (`assets/fonts/`)

## Phase 7 — Leah-ready device

- Reliable daily reading experience
- Battery life acceptable for regular use
- Physical device assembled and handed off

## Explicitly deferred

- Cloud features, OTA updates, and online book acquisition
- Heavy customization or user profiles
- Features that distract from reading
