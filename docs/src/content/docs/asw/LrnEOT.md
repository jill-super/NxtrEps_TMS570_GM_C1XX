---
title: "LrnEOT"
description: "LrnEOT: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_LrnEOT).*
## Purpose and responsibility
Software area `LrnEOT` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_LrnEOT.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_LrnEOT.arxml` |
| Generation templates | `Ap_LrnEOT_Cfg.arxml.tt`, `Ap_LrnEOT_Cfg.h.tt`, `Ap_LrnEOT_Generate.bat`, `Ap_LrnEOT_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (30 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Pim_LearnedEOT` | RTE-generated symbol |
| `Rte_IWrite_LrnEOT_Init1_CCWFound_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_LrnEOT_Init1_CCWFound_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWrite_LrnEOT_Init1_CCWPosition_HwDeg_f32` | RTE-generated symbol |
| `Rte_IWriteRef_LrnEOT_Init1_CCWPosition_HwDeg_f32` | RTE-generated symbol |
| `Rte_IWrite_LrnEOT_Init1_CWFound_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_LrnEOT_Init1_CWFound_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWrite_LrnEOT_Init1_CWPosition_HwDeg_f32` | RTE-generated symbol |
| `Rte_IWriteRef_LrnEOT_Init1_CWPosition_HwDeg_f32` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_GetNTCFailed` | RTE-generated symbol |
| `Rte_Call_LearnedEOTData_SetRamBlockStatus` | RTE-generated symbol |
| `Rte_Call_LearnedEOTData_WriteBlock` | RTE-generated symbol |
| `Rte_Call_SystemTime_GetSystemTime_mS_u32` | RTE-generated symbol |
| `Rte_IRead_LrnEOT_Per1_DiagStsHwPosDis_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_LrnEOT_Per1_HandwheelAuthority_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_LrnEOT_Per1_HandwheelPosition_HwDeg_f32` | RTE-generated symbol |
| `Rte_IRead_LrnEOT_Per1_HwTorque_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_LrnEOT_Per1_MtrVelCRF_MtrRadpS_f32` | RTE-generated symbol |
| `Rte_IRead_LrnEOT_Per1_PostLimitTorque_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWrite_LrnEOT_Per1_CCWFound_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_LrnEOT_Per1_CCWFound_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWrite_LrnEOT_Per1_CCWPosition_HwDeg_f32` | RTE-generated symbol |
| `Rte_IWriteRef_LrnEOT_Per1_CCWPosition_HwDeg_f32` | RTE-generated symbol |
| `Rte_IWrite_LrnEOT_Per1_CWFound_Cnt_lgc` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_LrnEOT_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_LrnEOT.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_LrnEOT_Cfg.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h` `Rte.h` `Rte_Ap_LrnEOT.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [LrnEOT — LearnEOT](./LrnEOT-LearnEOT/) | `LrnEOT/doc/LearnEOT.docx` |

*Repository path: `LrnEOT/`* 
