---
title: "SVDrvr_CM"
description: "SVDrvr_CM: purpose, files, API and documents (Complex Device Drivers (CDD))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house PWM/SV driver CDD (PwmCdd).*
## Purpose and responsibility
Software area `SVDrvr_CM` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `PwmCdd.c` |
| `include/` | `PwmCdd.h` |
## Public API
No C sources in this area (configuration, generated data or tooling only).
## Usage and dependencies
Selected project headers included by this module:
`CDD_Data.h` `CDD_Func.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `PwmCdd.h` `PwmCdd_Cfg.h` `Std_Types.h` `fixmath.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`CalConstants.h` `Compiler_Cfg.h` `MemMap.h` `PwmCdd` `CDD_Data.h` `CDD_Func.h` `PwmCdd_Cfg.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [SVDrvr_CM — PWMCdd_Integration_Manual](./SVDrvr_CM-PWMCdd_Integration_Manual/) | `SVDrvr_CM/doc/PWMCdd_Integration_Manual.docx` |
| [SVDrvr_CM — PWM_CDD_MDD](./SVDrvr_CM-PWM_CDD_MDD/) | `SVDrvr_CM/doc/PWM_CDD_MDD.docx` |

*Repository path: `SVDrvr_CM/`* 
