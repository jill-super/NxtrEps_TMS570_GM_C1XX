---
title: "WhlImbRej"
description: "WhlImbRej: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_WhlImbRej).*
## Purpose and responsibility
Software area `WhlImbRej` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_WhlImbRej.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_WhlImbRej.arxml` |
| Generation templates | `Ap_WhlImbRej_Cfg.arxml.tt`, `Ap_WhlImbRej_Cfg.h.tt`, `Ap_WhlImbRej_Generate.bat`, `Ap_WhlImbRej_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (25 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Mode_SystemState_Mode` | RTE-generated symbol |
| `Rte_IRead_WhlImbRej_Per1_DiagStsWIRDisable_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_WhlImbRej_Per1_HwTrq_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_WhlImbRej_Per1_QualWhlFreqL_Hz_f32` | RTE-generated symbol |
| `Rte_IRead_WhlImbRej_Per1_QualWhlFreqR_Hz_f32` | RTE-generated symbol |
| `Rte_IRead_WhlImbRej_Per1_VehSpdValid_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_WhlImbRej_Per1_VehSpd_Kph_f32` | RTE-generated symbol |
| `Rte_IRead_WhlImbRej_Per1_WIRMfgEnable_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_WhlImbRej_Per1_WhlFreqQualified_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWrite_WhlImbRej_Per1_WIRCmdAmpBlnd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_WhlImbRej_Per1_WIRCmdAmpBlnd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWrite_WhlImbRej_Per1_WhlImbRejCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_WhlImbRej_Per1_WhlImbRejCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_SetNTCStatus` | RTE-generated symbol |
| `Rte_Call_SystemTime_DtrmnElapsedTime_mS_u16` | RTE-generated symbol |
| `Rte_Call_SystemTime_DtrmnElapsedTime_mS_u32` | RTE-generated symbol |
| `Rte_Call_SystemTime_GetSystemTime_mS_u32` | RTE-generated symbol |
| `Rte_Call_WhlImbRej_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_WhlImbRej_Per1_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_WhlImbRej_Per2_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_WhlImbRej_Per2_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_IWrite_WhlImbRej_Per3_WhlImbRejCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_WhlImbRej_Per3_WhlImbRejCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_Call_WhlImbRej_Per3_CP0_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_WhlImbRej_Cfg.h` `CalConstants.h` `Filter_Types.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_WhlImbRej.h` `filters.h` `fixmath.h` `interpolation.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_WhlImbRej_Cfg.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h` `Rte.h` `Rte_Ap_WhlImbRej.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [WhlImbRej — Wheel_Imbalance_Rejection_MDD](./WhlImbRej-Wheel_Imbalance_Rejection_MDD/) | `WhlImbRej/doc/Wheel_Imbalance_Rejection_MDD.docx` |

*Repository path: `WhlImbRej/`* 
