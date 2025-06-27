# PSX SIO-qsb

[![License: CERN-OHL-S-2.0](https://img.shields.io/badge/License-CERN--OHL--S--2.0-lightgrey.svg)](LICENSE)  
[![Release](https://img.shields.io/github/v/release/Electroanalog/PSX-SIO-qsb)](../../releases)  
[![Board Type](https://img.shields.io/badge/Board-QSB%20%7C%20FR--4%20%26%20Flex-blue)]()  
[![Pin Count](https://img.shields.io/badge/Signals-4-green)]()  
[![Tested on Hardware](https://img.shields.io/badge/Tested-PlayStation-success)]()

**PSX SIO-qsb** is a compact Quick Solder Board (QSB) for the original PlayStation 1 that replaces the official PSIO Switch Board and compatible third-party alternatives.  
It simplifies installation by minimizing the number of required signals while maintaining full compatibility with PSIO cartridges.  
Designed for minimal footprint and clean routing, the QSB can be fabricated using standard **FR-4** PCBs (1 mm or thinner) or **flex PCBs** for ultra-low profile integration.

---

## Table of Contents

- [Overview](#overview)  
- [Pinout](#pinout)  
- [Installation Notes](#installation-notes)  
- [Gerber Files](#gerber-files)  
- [Gallery](#gallery)  
- [License](#license)  
- [Credits](#credits)  
- [Topics / Tags](#topics--tags)

---

## Overview

The PSIO cartridge enables PS1 consoles to run disc images from an SD Card via the Parallel I/O port, but it requires a supporting Switch Board to access CD subsystem signals not exposed externally.  
**PSX SIO-qsb** serves the same role as the official Switch Board—but with fewer wires, a smaller footprint, and a more installer-friendly layout.  

By routing only the essential signals between the CD controller and the expansion port, this board reduces installation complexity without compromising PSIO functionality.  
It is *not* a modchip, and does *not* alter copy protection or disc authentication logic in any way.

---

## Pinout

| PSIO Signal | SIO-qsb Label |
|-------------|---------------|
| XE          | XE            |
| XI          | XI            |
| CE          | CE            |
| CI          | CI            |

Legacy Switch Board implementations used up to 9 wires for signal redirection. The **PSX SIO-qsb** reduces this count by forwarding only the essential lines required for operation.

---

## Installation Notes

- Recommended PCB material:  
  - **FR-4 Standard**, thickness ≤ 1.0 mm  
  - **Flex PCB**, ENIG finish recommended  
- The board is mounted over the PS1 mainboard, typically adjacent to the CD controller (IC302).  
- Connections should be soldered directly to test points or vias (with soldermask removed).  
- Fine-pitch soldering skills and proper tools (e.g. fine iron tip, magnification) are strongly recommended.  
- The original CD-ROM controller remains active when PSIO is disconnected, as with the official Switch Board design.  

> ℹ️ Installation differs depending on PS1 motherboard revision. Always reference an installation diagram for your console’s PU-xx board code.

---

## Gerber Files

This repository includes ready-to-manufacture **Gerber files** and supporting layer previews for the PSX SIO-qsb.  
Fabrication notes:

- 2-layer board  
- 1.0 mm thickness recommended (FR-4)  
- ENIG or HASL finish  
- Optionally available as **flex PCB**  
- All signal names are silkscreened  

---

## Gallery

*Coming soon.*  
Photos of the assembled board, installation examples on PU-18 and PU-22 boards, and Flex PCB variants will be added here.

---

## License

This project is licensed under the **CERN Open Hardware Licence Version 2 – Strongly Reciprocal (CERN-OHL-S v2)**.  
You may copy, modify, and distribute the design files, but any modified versions must also be licensed under the same terms.

For full license text, see the [LICENSE](LICENSE) file or visit the [CERN-OHL-S v2 official page](https://gitlab.com/ohwr/project/cernohl/-/wikis/Documents/CERN-OHL-version-2).

---

## Credits

Created by **Electroanalog (2025)**  
Compatible with PSIO by **Cybdyn Systems** and verified with high-quality third-party cartridges.

---

## Topics / Tags

`psx` `playstation` `psio` `switchboard` `qsb` `modchip` `hardware` `retro` `flexpcb` `gerber`
