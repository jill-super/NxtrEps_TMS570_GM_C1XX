---
title: "ThrmDutyCycle"
description: "ThrmDutyCycle: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_ThrmlDutyCycle).*
## Purpose and responsibility
Documented behaviour (first paragraph of the module design description):

> description: "Converted .docx document from ThrmDutyCycle/doc."

## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_ThrmlDutyCycle.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_ThrmlDutyCycle.arxml` |
| Generation templates | `Ap_ThrmlDutyCycle_Cfg.arxml.tt`, `Ap_ThrmlDutyCycle_Cfg.h.tt`, `Ap_ThrmlDutyCycle_Generate.bat`, `Ap_ThrmlDutyCycle_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (23 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_ThrmlDutyCycle_Init1_DefeatDutySvc_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_ThrmlDutyCycle_Init1_IgnTimeOff_Cnt_u32` | RTE-generated symbol |
| `Rte_IRead_ThrmlDutyCycle_Init1_VehTimeValid_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_ThrmlDutyCycle_Per1_CuTempEst_DegC_f32` | RTE-generated symbol |
| `Rte_IRead_ThrmlDutyCycle_Per1_DefeatDutySvc_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_ThrmlDutyCycle_Per1_FiltMeasTemp_DegC_f32` | RTE-generated symbol |
| `Rte_IRead_ThrmlDutyCycle_Per1_FilteredPkCurr_AmpSq_f32` | RTE-generated symbol |
| `Rte_IRead_ThrmlDutyCycle_Per1_IgnTimeOff_Cnt_u32` | RTE-generated symbol |
| `Rte_IRead_ThrmlDutyCycle_Per1_MagTempEst_DegC_f32` | RTE-generated symbol |
| `Rte_IRead_ThrmlDutyCycle_Per1_MotorVelCRF_MtrRadpS_f32` | RTE-generated symbol |
| `Rte_IRead_ThrmlDutyCycle_Per1_MtrPkCurr_AmpSq_f32` | RTE-generated symbol |
| `Rte_IRead_ThrmlDutyCycle_Per1_SiTempEst_DegC_f32` | RTE-generated symbol |
| `Rte_IRead_ThrmlDutyCycle_Per1_VehTimeValid_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWrite_ThrmlDutyCycle_Per1_DutyCycleLevel_Uls_f32` | RTE-generated symbol |
| `Rte_IWriteRef_ThrmlDutyCycle_Per1_DutyCycleLevel_Uls_f32` | RTE-generated symbol |
| `Rte_IWrite_ThrmlDutyCycle_Per1_ThermLimitPerc_Uls_f32` | RTE-generated symbol |
| `Rte_IWriteRef_ThrmlDutyCycle_Per1_ThermLimitPerc_Uls_f32` | RTE-generated symbol |
| `Rte_IWrite_ThrmlDutyCycle_Per1_ThermalLimit_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_ThrmlDutyCycle_Per1_ThermalLimit_MtrNm_f32` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_GetNTCFailed` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_SetNTCStatus` | RTE-generated symbol |
| `Rte_Call_ThrmlDutyCycle_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_ThrmlDutyCycle_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_ThrmlDutyCycle_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_ThrmlDutyCycle.h` `filters.h` `fixmath.h` `interpolation.h` `math.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_ThrmlDutyCycle_Cfg.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h` `Rte.h` `Rte_Ap_ThrmlDutyCycle.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [ThrmDutyCycle — ThermalDutyCycle_Integration_Manual](./ThrmDutyCycle-ThermalDutyCycle_Integration_Manual/) | `ThrmDutyCycle/doc/ThermalDutyCycle_Integration_Manual.docx` |
| [ThrmDutyCycle — Thermal_Duty_Cycle_MDD](./ThrmDutyCycle-Thermal_Duty_Cycle_MDD/) | `ThrmDutyCycle/doc/Thermal_Duty_Cycle_MDD.docx` |

*Repository path: `ThrmDutyCycle/`* 
