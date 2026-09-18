---
title: "StabilityComp"
description: "StabilityComp: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-Cs (Ap_StabilityComp/2).*
## Purpose and responsibility
Documented behaviour (first paragraph of the module design description):

> description: "Converted .docx document from StabilityComp/doc."

## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_StabilityComp.c`, `Ap_StabilityComp2.c` |
| AUTOSAR model | 6 `.arxml` file(s), e.g. `Ap_StabilityComp.arxml` |
| Generation templates | `Ap_StabilityComp2_Cfg.arxml.tt`, `Ap_StabilityComp2_Cfg.h.tt`, `Ap_StabilityComp2_Generate.bat`, `Ap_StabilityComp2_bswmd.arxml`, `Ap_StabilityComp_Cfg.arxml.tt`, `Ap_StabilityComp_Cfg.h.tt` |
## Public API
Top RTE/component symbols referenced in the sources (21 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_StabilityComp_Per1_AssistDDFactor_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_StabilityComp_Per1_AsstFWActive_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_StabilityComp_Per1_CombinedAssist_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_StabilityComp_Per1_HwTorque_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_StabilityComp_Per1_SysAssistCmd_MtrNm_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_StabilityComp_Per1_VehicleSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_IWrite_StabilityComp_Per1_AssistCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_StabilityComp_Per1_AssistCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_Call_FaultInjection_SCom_FltInjection` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_SetNTCStatus` | RTE-generated symbol |
| `Rte_Call_StabilityComp_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_StabilityComp_Per1_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_IRead_StabilityComp2_Per1_AssistDDFactor_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_StabilityComp2_Per1_AsstFWActive_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_StabilityComp2_Per1_CombinedAssist_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_StabilityComp2_Per1_HwTorque_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_StabilityComp2_Per1_VehicleSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_IWrite_StabilityComp2_Per1_SysAssistCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_StabilityComp2_Per1_SysAssistCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_Call_StabilityComp2_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_StabilityComp2_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_StabilityComp2_Cfg.h` `Ap_StabilityComp_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_StabilityComp.h` `Rte_Ap_StabilityComp2.h` `filters.h` `fixmath.h` `interpolation.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_StabilityComp` `Ap_StabilityComp_Cfg.h` `Rte.h` `Rte_Ap_StabilityComp.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `Ap_StabilityComp2` `Ap_StabilityComp2_Cfg.h` `Rte.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [StabilityComp — StabilityCompensation2_MDD](./StabilityComp-StabilityCompensation2_MDD/) | `StabilityComp/doc/StabilityCompensation2_MDD.docx` |
| [StabilityComp — StabilityCompensation_MDD](./StabilityComp-StabilityCompensation_MDD/) | `StabilityComp/doc/StabilityCompensation_MDD.docx` |

*Repository path: `StabilityComp/`* 
