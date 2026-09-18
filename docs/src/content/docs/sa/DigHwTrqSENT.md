---
title: "DigHwTrqSENT"
description: "DigHwTrqSENT: purpose, files, API and documents (Sensor / Actuator Abstraction)."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Sa_DigHwTrqSENT).*
## Purpose and responsibility
Documented behaviour (first paragraph of the module design description):

> description: "Converted .docx document from DigHwTrqSENT/doc."

## Key files
| Area | Files |
| --- | --- |
| `src/` | `Sa_DigHwTrqSENT.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Sa_DigHwTrqSENT.arxml` |
| Generation templates | `Sa_DigHwTrqSENT_Cfg.arxml.tt`, `Sa_DigHwTrqSENT_Cfg.h.tt`, `Sa_DigHwTrqSENT_Generate.bat`, `Sa_DigHwTrqSENT_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (26 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Pim_DigTrqTrim` | RTE-generated symbol |
| `Rte_IRead_DigHwTrqSENT_Init1_MECCounter_Cnt_enum` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_SetNTCStatus` | RTE-generated symbol |
| `Rte_Call_NvM_DigHwTrqSENTTrim_Srv_GetErrorStatus` | RTE-generated symbol |
| `Rte_IRead_DigHwTrqSENT_Per1_T1_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_DigHwTrqSENT_Per1_T2_HwNm_f32` | RTE-generated symbol |
| `Rte_IWrite_DigHwTrqSENT_Per1_HwTorque_HwNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_DigHwTrqSENT_Per1_HwTorque_HwNm_f32` | RTE-generated symbol |
| `Rte_IWrite_DigHwTrqSENT_Per1_SysCHwTorque_HwNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_DigHwTrqSENT_Per1_SysCHwTorque_HwNm_f32` | RTE-generated symbol |
| `Rte_Call_FaultInjection_SCom_FltInjection` | RTE-generated symbol |
| `Rte_Call_DigHwTrqSENT_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_DigHwTrqSENT_Per1_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_IWrite_DigHwTrqSENT_Per2_SrlComHwTrqValid_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_DigHwTrqSENT_Per2_SrlComHwTrqValid_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWrite_DigHwTrqSENT_Per2_SrlComHwTrq_HwNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_DigHwTrqSENT_Per2_SrlComHwTrq_HwNm_f32` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_GetNTCStatus` | RTE-generated symbol |
| `Rte_Call_DigHwTrqSENT_Per2_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_DigHwTrqSENT_Per2_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_DigHwTrqSENT_Per3_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_DigHwTrqSENT_Per3_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_Read_MECCounter_Cnt_enum` | RTE-generated symbol |
| `Rte_Call_NvM_DigHwTrqSENTTrim_Srv_WriteBlock` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_DiagMgr.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Sa_DigHwTrqSENT.h` `Sa_DigHwTrqSENT_Cfg.h` `filters.h` `fixmath.h` `interpolation.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_DiagMgr.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h` `Rte.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Sa_DigHwTrqSENT.h` `Rte_Type.h` `Sa_DigHwTrqSENT_Cfg.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [DigHwTrqSENT — DigHwTrqSENT_Integration_Manual](./DigHwTrqSENT-DigHwTrqSENT_Integration_Manual/) | `DigHwTrqSENT/doc/DigHwTrqSENT_Integration_Manual.docx` |
| [DigHwTrqSENT — DigHwTrqSENT_MDD](./DigHwTrqSENT-DigHwTrqSENT_MDD/) | `DigHwTrqSENT/doc/DigHwTrqSENT_MDD.docx` |

*Repository path: `DigHwTrqSENT/`* 
