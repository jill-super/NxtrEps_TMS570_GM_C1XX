---
title: "ShtdnMech"
description: "ShtdnMech: purpose, files, API and documents (Sensor / Actuator Abstraction)."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Sa_ShtdnMech).*
## Purpose and responsibility
Software area `ShtdnMech` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Sa_ShtdnMech.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Sa_ShtdnMech.arxml` |
| Generation templates | `Sa_ShtdnMech_Cfg.arxml.tt`, `Sa_ShtdnMech_Cfg.h.tt`, `Sa_ShtdnMech_Generate.bat`, `Sa_ShtdnMech_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (5 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Call_FetDrvReset_OP_GET` | RTE-generated symbol |
| `Rte_Call_SysFault2_OP_GET` | RTE-generated symbol |
| `Rte_Call_SysFault3_OP_GET` | RTE-generated symbol |
| `Rte_Call_ShtdnMech_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_ShtdnMech_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`MemMap.h` `Rte_Sa_ShtdnMech.h` `Sa_ShtdnMech_Cfg.h` `n2het_regs.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Compiler_Cfg.h` `MemMap.h` `Sa_ShtdnMech` `Rte.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Sa_ShtdnMech.h` `Rte_Type.h` `Sa_ShtdnMech_Cfg.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [ShtdnMech — Shutdown_Mechanisms_MDD](./ShtdnMech-Shutdown_Mechanisms_MDD/) | `ShtdnMech/doc/Shutdown_Mechanisms_MDD.docx` |

*Repository path: `ShtdnMech/`* 
