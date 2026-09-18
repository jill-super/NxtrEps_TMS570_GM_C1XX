---
title: "Dma"
description: "Dma: purpose, files, API and documents (MCAL & MCU Drivers)."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house DMA driver for TMS570.*
## Purpose and responsibility
Software area `Dma` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Dma.c` |
| `include/` | `Dma.h` |
## Public API
No C sources in this area (configuration, generated data or tooling only).
## Usage and dependencies
Selected project headers included by this module:
`Adc.h` `Adc2.h` `Dma.h` `Dma_Cfg.h` `MemMap.h` `Nhet_SENT_Prog.h` `SpiNxt.h` `appinit_cfg.h` `crc_regs.h` `dma_regs.h` `epwm_regs.h` `mibspi_regs.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Adc.h` `Adc2.h` `Compiler_Cfg.h` `Dma_Cfg.h` `MemMap.h` `Nhet_SENT_Prog.h` `SpiNxt.h` `appinit_cfg.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [Dma — Dma Integration Manual](./Dma-Dma-Integration-Manual/) | `Dma/doc/Dma Integration Manual.docx` |
| [Dma — Dma_MDD](./Dma-Dma_MDD/) | `Dma/doc/Dma_MDD.docx` |

*Repository path: `Dma/`* 
