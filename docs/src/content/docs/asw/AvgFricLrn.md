---
title: "AvgFricLrn"
description: "AvgFricLrn: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_AvgFricLrn).*
## Purpose and responsibility
Software area `AvgFricLrn` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_AvgFricLrn.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_AvgFricLrn.arxml` |
| Generation templates | `Ap_AvgFricLrn_Cfg.arxml.tt`, `Ap_AvgFricLrn_Cfg.h.tt`, `Ap_AvgFricLrn_Generate.bat`, `Ap_AvgFricLrn_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (27 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Pim_AvgFricLrnData` | RTE-generated symbol |
| `Rte_IWrite_AvgFricLrn_Init1_FricOffset_HwNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_AvgFricLrn_Init1_FricOffset_HwNm_f32` | RTE-generated symbol |
| `Rte_Mode_SystemState_Mode` | RTE-generated symbol |
| `Rte_Call_SystemTime_GetSystemTime_mS_u32` | RTE-generated symbol |
| `Rte_IRead_AvgFricLrn_Per1_CRFMtrTrq_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_AvgFricLrn_Per1_DefeatFricLearning_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_AvgFricLrn_Per1_HwAng_HwDeg_f32` | RTE-generated symbol |
| `Rte_IRead_AvgFricLrn_Per1_HwPosAuthority_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_AvgFricLrn_Per1_HwTrq_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_AvgFricLrn_Per1_HwVel_HwRadpS_f32` | RTE-generated symbol |
| `Rte_IRead_AvgFricLrn_Per1_LatAcc_g_f32` | RTE-generated symbol |
| `Rte_IRead_AvgFricLrn_Per1_Temperature_DegC_f32` | RTE-generated symbol |
| `Rte_IRead_AvgFricLrn_Per1_VehSpd_Kph_f32` | RTE-generated symbol |
| `Rte_IRead_AvgFricLrn_Per1_VehicleSpeedValid_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWrite_AvgFricLrn_Per1_EstFric_HwNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_AvgFricLrn_Per1_EstFric_HwNm_f32` | RTE-generated symbol |
| `Rte_IWrite_AvgFricLrn_Per1_FricOffset_HwNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_AvgFricLrn_Per1_FricOffset_HwNm_f32` | RTE-generated symbol |
| `Rte_IWrite_AvgFricLrn_Per1_SatEstFric_HwNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_AvgFricLrn_Per1_SatEstFric_HwNm_f32` | RTE-generated symbol |
| `Rte_Call_FltInjection_SCom_FltInjection` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_SetNTCStatus` | RTE-generated symbol |
| `Rte_Call_AvgFricLrnData_WriteBlock` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_AvgFricLrn_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_AvgFricLrn.h` `filters.h` `fixmath.h` `interpolation.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_AvgFricLrn` `Ap_AvgFricLrn_Cfg.h` `Rte.h` `Rte_Ap_AvgFricLrn.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `Ap_AvgFricLrn_Cfg.h` `CalConstants.h` `Compiler_Cfg.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [AvgFricLrn — Average_Friction_Learning_MDD](./AvgFricLrn-Average_Friction_Learning_MDD/) | `AvgFricLrn/doc/Average_Friction_Learning_MDD.docx` |
| [AvgFricLrn — AvgFricLrn_Integration_Manual](./AvgFricLrn-AvgFricLrn_Integration_Manual/) | `AvgFricLrn/doc/AvgFricLrn_Integration_Manual.docx` |

*Repository path: `AvgFricLrn/`* 
