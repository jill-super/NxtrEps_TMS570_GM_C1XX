---
title: "NvMMgr"
description: "NvMMgr: purpose, files, API and documents (Basic Software (BSW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house Flash/EEPROM interface (Cd_FeeIf) above the TI FEE driver.*
## Purpose and responsibility
Software area `NvMMgr` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Cd_FeeIf.c`, `Fapi_UserDefinedFunctions.c` |
| `include/` | `Cd_FeeIf.h` |
| Generation templates | `Cd_NvMMgr_Cfg.h.tt`, `Cd_NvMMgr_Generate.bat`, `Cd_NvMMgr_bswmd.arxml` |
## Public API
No C sources in this area (configuration, generated data or tooling only).
## Usage and dependencies
Selected project headers included by this module:
`Cd_FeeIf.h` `Cd_NvMMgr_Cfg.h` `F021.h` `MemIf_Types.h` `Os.h` `Std_Types.h` `fee.h` `trustfct.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Cd_NvMMgr_Cfg.h` `Compiler_Cfg.h` `F021.h` `MemIf_Types.h` `MemMap.h` `Os.h` `fee.h` `trustfct.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [NvMMgr — Fee_Interface_MDD](./NvMMgr-Fee_Interface_MDD/) | `NvMMgr/doc/Fee_Interface_MDD.docx` |
| [NvMMgr — NvMMgr_Integration_Manual](./NvMMgr-NvMMgr_Integration_Manual/) | `NvMMgr/doc/NvMMgr_Integration_Manual.docx` |

*Repository path: `NvMMgr/`* 
