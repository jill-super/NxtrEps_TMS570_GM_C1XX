---
title: "SVDiag"
description: "SVDiag: purpose, files, API and documents (Sensor / Actuator Abstraction)."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house diagnostics SW-Cs (Sa_MtrDrvDiag, Ap_DigPhsReasDiag).*
## Purpose and responsibility
Software area `SVDiag` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_DigPhsReasDiag.c`, `Sa_MtrDrvDiag.c` |
| AUTOSAR model | 5 `.arxml` file(s), e.g. `Ap_DigPhsReasDiag.arxml` |
| Generation templates | `Ap_DigPhsReasDiag_Cfg.arxml.tt`, `Ap_DigPhsReasDiag_Cfg.h.tt`, `Ap_DigPhsReasDiag_Generate.bat`, `Ap_DigPhsReasDiag_bswmd.arxml`, `Sa_MtrDrvDiag_Cfg.arxml.tt`, `Sa_MtrDrvDiag_Cfg.h.tt` |
## Public API
Top RTE/component symbols referenced in the sources (40 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Mode_SystemState_Mode` | RTE-generated symbol |
| `Rte_IRead_DigPhsReasDiag_Per1_ExpectedOnTimeA_Cnt_u32` | RTE-generated symbol |
| `Rte_IRead_DigPhsReasDiag_Per1_ExpectedOnTimeB_Cnt_u32` | RTE-generated symbol |
| `Rte_IRead_DigPhsReasDiag_Per1_ExpectedOnTimeC_Cnt_u32` | RTE-generated symbol |
| `Rte_IRead_DigPhsReasDiag_Per1_GateDriveResetActive_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_DigPhsReasDiag_Per1_LRPRCorrectedMtrPosCaptured_Rev_f32` | RTE-generated symbol |
| `Rte_IRead_DigPhsReasDiag_Per1_LRPRModulationIndexCaptured_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_DigPhsReasDiag_Per1_LRPRPhaseadvanceCaptured_Cnt_s16` | RTE-generated symbol |
| `Rte_IRead_DigPhsReasDiag_Per1_MeasuredOnTimeA_Cnt_u32` | RTE-generated symbol |
| `Rte_IRead_DigPhsReasDiag_Per1_MeasuredOnTimeB_Cnt_u32` | RTE-generated symbol |
| `Rte_IRead_DigPhsReasDiag_Per1_MeasuredOnTimeC_Cnt_u32` | RTE-generated symbol |
| `Rte_IRead_DigPhsReasDiag_Per1_MotorVelMRFUnfiltered_MtrRadpS_f32` | RTE-generated symbol |
| `Rte_IRead_DigPhsReasDiag_Per1_MtrElecMechPolarity_Cnt_s08` | RTE-generated symbol |
| `Rte_IRead_DigPhsReasDiag_Per1_PDActivateTest_Cnt_lgc` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_SetNTCStatus` | RTE-generated symbol |
| `Rte_Call_DigPhsReasDiag_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_DigPhsReasDiag_Per1_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_IRead_MtrDrvDiag_Per1_MtrDrvrInitStart_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWrite_MtrDrvDiag_Per1_FETFaultPhase_Cnt_enum` | RTE-generated symbol |
| `Rte_IWriteRef_MtrDrvDiag_Per1_FETFaultPhase_Cnt_enum` | RTE-generated symbol |
| `Rte_IWrite_MtrDrvDiag_Per1_FETFaultType_Cnt_enum` | RTE-generated symbol |
| `Rte_IWriteRef_MtrDrvDiag_Per1_FETFaultType_Cnt_enum` | RTE-generated symbol |
| `Rte_IWrite_MtrDrvDiag_Per1_GateDriveResetActive_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_MtrDrvDiag_Per1_GateDriveResetActive_Cnt_lgc` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_DigPhsReasDiag_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Os.h` `Rte_Ap_DigPhsReasDiag.h` `Rte_Sa_MtrDrvDiag.h` `Sa_MtrDrvDiag_Cfg.h` `filters.h` `fixmath.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_DigPhsReasDiag` `Ap_DigPhsReasDiag_Cfg.h` `Rte.h` `Rte_Ap_DigPhsReasDiag.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [SVDiag — DigPhsReasDiag_MDD](./SVDiag-DigPhsReasDiag_MDD/) | `SVDiag/doc/DigPhsReasDiag_MDD.docx` |
| [SVDiag — Motor_Driver_Diagnostics_MDD](./SVDiag-Motor_Driver_Diagnostics_MDD/) | `SVDiag/doc/Motor_Driver_Diagnostics_MDD.docx` |
| [SVDiag — SVDiag_Integration_Manual](./SVDiag-SVDiag_Integration_Manual/) | `SVDiag/doc/SVDiag_Integration_Manual.docx` |

*Repository path: `SVDiag/`* 
