---
title: "SpiNxt"
description: "SpiNxt: purpose, files, API and documents (MCAL & MCU Drivers)."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SPI driver (SpiNxt).*
## Purpose and responsibility
Software area `SpiNxt` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `SpiNxt.c`, `SpiNxt_Irq.c` |
| `include/` | `SpiNxt.h` |
| AUTOSAR model | 3 `.arxml` file(s), e.g. `SpiNxt.arxml` |
| Generation templates | `SpiNxt_Cfg.h.tt`, `SpiNxt_Generate.bat`, `SpiNxt_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (2 unique in total):
| Symbol | Kind |
| --- | --- |
| `SchM_Enter_SpiNxt` | component symbol |
| `SchM_Exit_SpiNxt` | component symbol |
## Usage and dependencies
Selected project headers included by this module:
`Dio.h` `MemMap.h` `Metrics.h` `Os.h` `SchM_SpiNxt.h` `Spi.h` `SpiNxt.h` `SpiNxt_Cfg.h` `Std_Types.h` `mibspi_regs.h` `sys_common.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Compiler_Cfg.h` `Dio.h` `Dio_Cfg.h` `MemMap.h` `Metrics.h` `Os.h` `SchM_SpiNxt.h` `Spi.h` `SpiNxt` `SpiNxt_Cfg.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [SpiNxt — Spi_Nexteer_Integration_Manual](./SpiNxt-Spi_Nexteer_Integration_Manual/) | `SpiNxt/doc/Spi_Nexteer_Integration_Manual.docx` |
| [SpiNxt — Spi_Nexteer_MDD](./SpiNxt-Spi_Nexteer_MDD/) | `SpiNxt/doc/Spi_Nexteer_MDD.docx` |

*Repository path: `SpiNxt/`* 
