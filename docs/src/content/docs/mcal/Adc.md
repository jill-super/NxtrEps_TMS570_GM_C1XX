---
title: "Adc"
description: "Adc: purpose, files, API and documents (MCAL & MCU Drivers)."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house ADC complex driver for TMS570 (Adc/Adc2/Adc_Common).*
## Purpose and responsibility
Software area `Adc` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Adc.c`, `Adc2.c`, `Adc_Common.c` |
| `include/` | `Adc.h`, `Adc2.h`, `Adc_Common.h` |
## Public API
No C sources in this area (configuration, generated data or tooling only).
## Usage and dependencies
Selected project headers included by this module:
`Adc.h` `Adc2.h` `Adc2_Cfg.h` `Adc_Cfg.h` `Adc_Common.h` `Ap_DiagMgr.h` `CDD_Const.h` `CDD_Data.h` `CalConstants.h` `Calconstants.h` `GlobalMacro.h` `MemMap.h` `Std_Types.h` `SystemTime.h` `adc_regs.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [Adc — Adc2_MDD](./Adc-Adc2_MDD/) | `Adc/doc/Adc2_MDD.docx` |
| [Adc — Adc_Common_MDD](./Adc-Adc_Common_MDD/) | `Adc/doc/Adc_Common_MDD.docx` |
| [Adc — Adc_MDD](./Adc-Adc_MDD/) | `Adc/doc/Adc_MDD.docx` |
| [Adc — Integration_Manual_ADC](./Adc-Integration_Manual_ADC/) | `Adc/doc/Integration_Manual_ADC.docx` |

*Repository path: `Adc/`* 
