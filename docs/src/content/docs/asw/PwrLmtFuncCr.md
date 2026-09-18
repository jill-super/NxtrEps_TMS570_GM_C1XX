---
title: "PwrLmtFuncCr"
description: "PwrLmtFuncCr: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_PwrLmtFuncCr).*
## Purpose and responsibility
Documented behaviour (first paragraph of the module design description):

> title: "PwrLmtFuncCr — Power_Limit_Function_CM_Integration_Manual"

## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_PwrLmtFuncCr.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_PwrLmtFuncCr.arxml` |
| Generation templates | `Ap_PwrLmtFuncCr_Cfg.arxml.tt`, `Ap_PwrLmtFuncCr_Cfg.h.tt`, `Ap_PwrLmtFuncCr_Generate.bat`, `Ap_PwrLmtFuncCr_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (23 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Mode_SystemState_Mode` | RTE-generated symbol |
| `Rte_Call_SystemTime_GetSystemTime_mS_u32` | RTE-generated symbol |
| `Rte_IRead_PwrLmtFuncCr_Per1_AltFaultActive_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_PwrLmtFuncCr_Per1_CntDisMtrTrqCmdMRF_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_PwrLmtFuncCr_Per1_EstKe_VpRadpS_f32` | RTE-generated symbol |
| `Rte_IRead_PwrLmtFuncCr_Per1_MotorVelMRF_MtrRadpS_f32` | RTE-generated symbol |
| `Rte_IRead_PwrLmtFuncCr_Per1_PosServEnable_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_PwrLmtFuncCr_Per1_Vecu_Volt_f32` | RTE-generated symbol |
| `Rte_IWrite_PwrLmtFuncCr_Per1_MRFMtrTrqCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_PwrLmtFuncCr_Per1_MRFMtrTrqCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_Call_PwrLmtFuncCr_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_PwrLmtFuncCr_Per1_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_IRead_PwrLmtFuncCr_Per2_CntDisMtrTrqCmdMRF_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_PwrLmtFuncCr_Per2_Vecu_Volt_f32` | RTE-generated symbol |
| `Rte_IWrite_PwrLmtFuncCr_Per2_FltTrqLmt_Uls_f32` | RTE-generated symbol |
| `Rte_IWriteRef_PwrLmtFuncCr_Per2_FltTrqLmt_Uls_f32` | RTE-generated symbol |
| `Rte_IWrite_PwrLmtFuncCr_Per2_ThresholdExceeded_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_PwrLmtFuncCr_Per2_ThresholdExceeded_Cnt_lgc` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_GetNTCStatus` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_SetNTCStatus` | RTE-generated symbol |
| `Rte_Call_SystemTime_DtrmnElapsedTime_mS_u16` | RTE-generated symbol |
| `Rte_Call_PwrLmtFuncCr_Per2_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_PwrLmtFuncCr_Per2_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_DiagMgr.h` `Ap_PwrLmtFuncCr_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_PwrLmtFuncCr.h` `filters.h` `fixmath.h` `float.h` `interpolation.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_DiagMgr.h` `Ap_PwrLmtFuncCr` `Ap_PwrLmtFuncCr_Cfg.h` `Rte.h` `Rte_Ap_PwrLmtFuncCr.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `CalConstants.h` `Compiler_Cfg.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [PwrLmtFuncCr — Power_Limit_Function_CM_Integration_Manual](./PwrLmtFuncCr-Power_Limit_Function_CM_Integration_Manual/) | `PwrLmtFuncCr/doc/Power_Limit_Function_CM_Integration_Manual.docx` |
| [PwrLmtFuncCr — Power_Limit_Function_CM_MDD](./PwrLmtFuncCr-Power_Limit_Function_CM_MDD/) | `PwrLmtFuncCr/doc/Power_Limit_Function_CM_MDD.docx` |

*Repository path: `PwrLmtFuncCr/`* 
