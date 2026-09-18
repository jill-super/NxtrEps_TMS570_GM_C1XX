---
title: "I2cNxtr"
description: "I2cNxtr: purpose, files, API and documents (MCAL & MCU Drivers)."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house I2C driver (I2cNxtr).*
## Purpose and responsibility
Software area `I2cNxtr` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `I2cNxtr.c`, `I2cNxtr_Irq.c` |
| `include/` | `I2cNxtr.h` |
## Public API
No C sources in this area (configuration, generated data or tooling only).
## Usage and dependencies
Selected project headers included by this module:
`I2cNxtr.h` `I2cNxtr_Cfg.h` `MemMap.h` `Metrics.h` `Os.h` `Std_Types.h` `SystemTime.h` `i2c_regs.h` `interrupts.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Compiler_Cfg.h` `I2cNxtr_Cfg.h` `MemMap.h` `Metrics.h` `Os.h` `interrupts.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [I2cNxtr — I2cNxtr_Integration_Manual](./I2cNxtr-I2cNxtr_Integration_Manual/) | `I2cNxtr/doc/I2cNxtr_Integration_Manual.docx` |
| [I2cNxtr — I2cNxtr_MDD](./I2cNxtr-I2cNxtr_MDD/) | `I2cNxtr/doc/I2cNxtr_MDD.docx` |

*Repository path: `I2cNxtr/`* 
