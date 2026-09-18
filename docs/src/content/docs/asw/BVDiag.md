---
title: "BVDiag"
description: "BVDiag: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_BVDiag).*
## Purpose and responsibility
Software area `BVDiag` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_BVDiag.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_BVDiag.arxml` |
| Generation templates | `Ap_BVDiag_Cfg.arxml.tt`, `Ap_BVDiag_Cfg.h.tt`, `Ap_BVDiag_Generate.bat`, `Ap_BVDiag_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (6 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_BVDiag_Per1_Batt_Volt_f32` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_SetNTCStatus` | RTE-generated symbol |
| `Rte_Call_SystemTime_DtrmnElapsedTime_mS_u16` | RTE-generated symbol |
| `Rte_Call_SystemTime_GetSystemTime_mS_u32` | RTE-generated symbol |
| `Rte_Call_BVDiag_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_BVDiag_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_BVDiag_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_BVDiag.h` `SystemTime.h` `fixmath.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_BVDiag` `Ap_BVDiag_Cfg.h` `Rte.h` `Rte_Ap_BVDiag.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [BVDiag — Battery_Voltage_Diagnostics](./BVDiag-Battery_Voltage_Diagnostics/) | `BVDiag/doc/Battery_Voltage_Diagnostics.doc` |

*Repository path: `BVDiag/`* 
