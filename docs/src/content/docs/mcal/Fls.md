---
title: "Fls"
description: "Fls: purpose, files, API and documents (MCAL & MCU Drivers)."
---

:::caution[Third-party — Texas Instruments]
Third-party driver/library provided by Texas Instruments for the TMS570 MCU. Do not modify; follow the vendor documentation linked below.
:::
*Origin: **TI** — Texas Instruments F021 Flash API library and headers (third-party).*
## Purpose and responsibility
Documented behaviour (first paragraph of the module design description):

> IMPORTANT – PLEASE CAREFULLY READ THE FOLLOWING LICENSE AGREEMENT, WHICH IS LEGALLY BINDING.  AFTER YOU READ THIS

## Key files
| Area | Files |
| --- | --- |
| `src/` | `F021_API_CortexR4_BE_V3D16.lib` |
| `include/` | `CGT.ARM.h`, `CGT.CCS.h`, `CGT.GHS.h`, `CGT.IAR.h`, `CGT.gcc.h`, `Compatibility.h`, `Constants.h`, `F021.h`, `FapiFunctions.h`, `Helpers.h`, `Registers.h`, `Registers_FMC_BE.h` |
## Public API
No C sources in this area (configuration, generated data or tooling only).
## Usage and dependencies
Selected project headers included by this module:
`CGT.ARM.h` `CGT.CCS.h` `CGT.GHS.h` `CGT.IAR.h` `CGT.gcc.h` `Compatibility.h` `Constants.h` `FapiFunctions.h` `Helpers.h` `Registers.h` `Registers_FMC_BE.h` `Registers_FMC_LE.h` `Types.h`
## Documents
| Document | Source file |
| --- | --- |
| [Fls — F021_Flash_API_License_Agreement](./Fls-F021_Flash_API_License_Agreement/) | `Fls/doc/F021_Flash_API_License_Agreement.pdf` |
| [Fls — Release_Notes](./Fls-Release_Notes/) | `Fls/doc/Release_Notes.pdf` |
| [Fls — SPNA148](./Fls-SPNA148/) | `Fls/doc/SPNA148.pdf` |
| [Fls — SPNU501F](./Fls-SPNU501F/) | `Fls/doc/SPNU501F.pdf` |
| [Fls — SPNZ210](./Fls-SPNZ210/) | `Fls/doc/SPNZ210.pdf` |
| [Fls — build_information](./Fls-build_information/) | `Fls/doc/build_information.txt` |
| [Fls — readme](./Fls-readme/) | `Fls/doc/readme.txt` |

*Repository path: `Fls/`* 
