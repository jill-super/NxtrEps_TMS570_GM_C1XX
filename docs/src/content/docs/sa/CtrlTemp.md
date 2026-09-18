---
title: "CtrlTemp"
description: "CtrlTemp: purpose, files, API and documents (Sensor / Actuator Abstraction)."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Sa_CtrlTemp).*
## Purpose and responsibility
Software area `CtrlTemp` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Sa_CtrlTemp.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Sa_CtrlTemp.arxml` |
| Generation templates | `Sa_CtrlTemp_Cfg.arxml.tt`, `Sa_CtrlTemp_Cfg.h.tt`, `Sa_CtrlTemp_Generate.bat`, `Sa_CtrlTemp_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (13 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_CtrlTemp_Init1_TemperatureADC_Volt_f32` | RTE-generated symbol |
| `Rte_IWrite_CtrlTemp_Init1_FiltMeasTemp_DegC_f32` | RTE-generated symbol |
| `Rte_IWriteRef_CtrlTemp_Init1_FiltMeasTemp_DegC_f32` | RTE-generated symbol |
| `Rte_IRead_CtrlTemp_Per1_DiagStsTempRdPrf_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_CtrlTemp_Per1_TemperatureADC_Volt_f32` | RTE-generated symbol |
| `Rte_IWrite_CtrlTemp_Per1_FiltMeasTemp_DegC_f32` | RTE-generated symbol |
| `Rte_IWriteRef_CtrlTemp_Per1_FiltMeasTemp_DegC_f32` | RTE-generated symbol |
| `Rte_Call_CtrlTemp_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_CtrlTemp_Per1_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_IRead_CtrlTemp_Per2_AmbTemp_DegC_f32` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_SetNTCStatus` | RTE-generated symbol |
| `Rte_Call_CtrlTemp_Per2_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_CtrlTemp_Per2_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Sa_CtrlTemp.h` `Sa_CtrlTemp_Cfg.h` `filters.h` `fixmath.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`CalConstants.h` `Compiler_Cfg.h` `MemMap.h` `Sa_CtrlTemp` `Rte.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Sa_CtrlTemp.h` `Rte_Type.h` `Sa_CtrlTemp_Cfg.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [CtrlTemp — Controller_Temperature_MDD](./CtrlTemp-Controller_Temperature_MDD/) | `CtrlTemp/doc/Controller_Temperature_MDD.docx` |
| [CtrlTemp — CtrlTemp_Integration_Manual](./CtrlTemp-CtrlTemp_Integration_Manual/) | `CtrlTemp/doc/CtrlTemp_Integration_Manual.docx` |

*Repository path: `CtrlTemp/`* 
