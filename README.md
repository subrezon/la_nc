# This keyboard has been succeeded by [Lancer](https://github.com/subrezon/lancer). If you're interested in la_nc - I recommend building a Lancer instead.

# la_nc

![subrezon/la_nc](https://i.imgur.com/xYDcTts.jpg)

Inspired by keyboards like Planck, Lumberjack and Lesovoz, la_nc aims to deliver a lightly split, ortho typing experience in a similar footprint, as well as an easy build process.

The name comes from the design process: take a Planck, remove a column from each side, then split it down the middle. Planck -> lanc -> la_nc.

# Features

- 42 keys in a unique take on ortholinear layouts
- Supports MX switches through Kailh hotswap sockets, with reinforced ai03's antishear socket pads
- Powered by a ProMicro or a compatible MCU board
- Optional support for an SSD1306 OLED screen

# BOM

- PCB
- top plate
- bottom plate
- ProMicro compatible MCU board
- 42x SMD diodes (1N4148W SOD123)
- 42x Kailh hotswap sockets
- 1x 3x6mm 2-pin tactile reset button
- 16x M2x5 screws
- 8x M2x8 standoffs
- 42x MX switches
- 42x 1U keycaps

Optionally:

- ProMicro socket (24-pin wide)
- SSD1306 128x32 OLED screen
- OLED socket (4-pin)

# Build guide

TODO

# QMK Firmware

You can find the firmware under subrezon/la_nc in the official QMK repository: https://github.com/qmk/qmk_firmware/tree/master/keyboards/subrezon/la_nc

Here's an example of flashing the keyboard with the default firmware:

	make subrezon/la_nc:default:flash

Or, using the QMK CLI:

	qmk flash -kb subrezon/la_nc -km default

If you're unsure what to do with this information, check out the [QMK Documentation](https://docs.qmk.fm/#/) for information on how to get started with QMK.

If you're building la_nc without the OLED screen, make sure to disable it in the rules.mk of your keymap:

	OLED_ENABLE = false

# Coming soon

- Build guide
- Acrylic cover for the gap in the middle
- Soldered PCB option (MX, Alps, Choc)
- Hotswap Choc support
- OR, Support for 2U keys in the bottom row
- High & Low profile 3D-printable cases

# Special thanks

- ai03 and foostan - for the Kicad libraries
- The r/MechanicalKeyboards and r/ErgoMechKeyboards - for the feedback, critique and support
