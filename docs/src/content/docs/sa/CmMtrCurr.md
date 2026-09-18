---
title: "CmMtrCurr"
description: "CmMtrCurr: purpose, files, API and documents (Sensor / Actuator Abstraction)."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Sa_CmMtrCurr).*
## Purpose and responsibility
Software area `CmMtrCurr` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Sa_CmMtrCurr.c` |
| `include/` | `Sa_CmMtrCurr.h` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Sa_CmMtrCurr.arxml` |
| Generation templates | `Sa_CmMtrCurr_Cfg.arxml.tt`, `Sa_CmMtrCurr_Cfg.h.tt`, `Sa_CmMtrCurr_Generate.bat`, `Sa_CmMtrCurr_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (38 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Pim_CurrTempOffset` | RTE-generated symbol |
| `Rte_Pim_ShCurrCal` | RTE-generated symbol |
| `Rte_Mode_SystemState_Mode` | RTE-generated symbol |
| `Rte_Call_EOLCurrTempOffset_WriteBlock` | RTE-generated symbol |
| `Rte_IRead_CmMtrCurr_Per1_FiltCntrlTemp_DegC_f32` | RTE-generated symbol |
| `Rte_IWrite_CmMtrCurr_Per1_MtrCurr1TempOffset_Volt_f32` | RTE-generated symbol |
| `Rte_IWriteRef_CmMtrCurr_Per1_MtrCurr1TempOffset_Volt_f32` | RTE-generated symbol |
| `Rte_IWrite_CmMtrCurr_Per1_MtrCurr2TempOffset_Volt_f32` | RTE-generated symbol |
| `Rte_IWriteRef_CmMtrCurr_Per1_MtrCurr2TempOffset_Volt_f32` | RTE-generated symbol |
| `Rte_Call_CmMtrCurr_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_CmMtrCurr_Per1_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_IRead_CmMtrCurr_Per2_ADCMtrCurr1_Volts_f32` | RTE-generated symbol |
| `Rte_IRead_CmMtrCurr_Per2_ADCMtrCurr2_Volts_f32` | RTE-generated symbol |
| `Rte_IRead_CmMtrCurr_Per2_CorrMtrCurrPosition_Rev_f32` | RTE-generated symbol |
| `Rte_IRead_CmMtrCurr_Per2_MtrCurrAngle_Rev_f32` | RTE-generated symbol |
| `Rte_IRead_CmMtrCurr_Per2_MtrCurrK1_Amp_f32` | RTE-generated symbol |
| `Rte_IRead_CmMtrCurr_Per2_MtrCurrK2_Amp_f32` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_SetNTCStatus` | RTE-generated symbol |
| `Rte_Call_CmMtrCurr_Per2_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_CmMtrCurr_Per2_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_IRead_CmMtrCurr_Per3_ADCMtrCurr1_Volts_f32` | RTE-generated symbol |
| `Rte_IRead_CmMtrCurr_Per3_ADCMtrCurr2_Volts_f32` | RTE-generated symbol |
| `Rte_IRead_CmMtrCurr_Per3_MtrVel_MtrRadpS_f32` | RTE-generated symbol |
| `Rte_IRead_CmMtrCurr_Per3_SrlComSvcDft_Cnt_b32` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`CalConstants.h` `CmMtrCurr_Cfg.h` `GlobalMacro.h` `Interpolation.h` `MemMap.h` `Rte_Sa_CmMtrCurr.h` `Rte_Type.h` `Sa_CmMtrCurr.h` `Sa_CmMtrCurr_Cfg.h` `filters.h` `fixmath.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`CalConstants.h` `Compiler_Cfg.h` `MemMap.h` `Sa_CmMtrCurr` `Adc2.h` `CDD_Const.h` `CDD_Data.h` `CmMtrCurr_Cfg.h` `Rte.h` `Rte_Compiler_Cfg.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [CmMtrCurr — CmMtrCurr_Integration_Manual](./CmMtrCurr-CmMtrCurr_Integration_Manual/) | `CmMtrCurr/doc/CmMtrCurr_Integration_Manual.docx` |
| [CmMtrCurr — CmMtrCurr_MDD](./CmMtrCurr-CmMtrCurr_MDD/) | `CmMtrCurr/doc/CmMtrCurr_MDD.docx` |

*Repository path: `CmMtrCurr/`* 
