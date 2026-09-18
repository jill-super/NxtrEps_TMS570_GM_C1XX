---
title: "EOTActuatorMng"
description: "EOTActuatorMng: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_EOTActuatorMng).*
## Purpose and responsibility
Documented behaviour (first paragraph of the module design description):

> title: "EOTActuatorMng — End_of_Travel_Actuator_Management_MDD"

## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_EOTActuatorMng.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_EOTActuatorMng.arxml` |
| Generation templates | `Ap_EOTActuatorMng_Cfg.arxml.tt`, `Ap_EOTActuatorMng_Cfg.h.tt`, `Ap_EOTActuatorMng_Generate.bat`, `Ap_EOTActuatorMng_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (19 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_EOTActuatorMng_Per1_CcwEOT_HwDeg_f32` | RTE-generated symbol |
| `Rte_IRead_EOTActuatorMng_Per1_CcwFound_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_EOTActuatorMng_Per1_CwEOT_HwDeg_f32` | RTE-generated symbol |
| `Rte_IRead_EOTActuatorMng_Per1_CwFound_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_EOTActuatorMng_Per1_EOTDisable_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_EOTActuatorMng_Per1_HandWheelAuth_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_EOTActuatorMng_Per1_HandWheelPos_HwDeg_f32` | RTE-generated symbol |
| `Rte_IRead_EOTActuatorMng_Per1_HwTorque_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_EOTActuatorMng_Per1_MotorVel_MtrRadpS_f32` | RTE-generated symbol |
| `Rte_IRead_EOTActuatorMng_Per1_PreLimitTorque_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_EOTActuatorMng_Per1_VehicleSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_IWrite_EOTActuatorMng_Per1_AssistEOTDamping_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_EOTActuatorMng_Per1_AssistEOTDamping_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWrite_EOTActuatorMng_Per1_AssistEOTGain_Uls_f32` | RTE-generated symbol |
| `Rte_IWriteRef_EOTActuatorMng_Per1_AssistEOTGain_Uls_f32` | RTE-generated symbol |
| `Rte_IWrite_EOTActuatorMng_Per1_AssistEOTLimit_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_EOTActuatorMng_Per1_AssistEOTLimit_MtrNm_f32` | RTE-generated symbol |
| `Rte_Call_EOTActuatorMng_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_EOTActuatorMng_Per1_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_EOTActuatorMng_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_EOTActuatorMng.h` `filters.h` `fixmath.h` `fpmtype.h` `interpolation.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_EOTActuatorMng_Cfg.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h` `Rte.h` `Rte_Ap_EOTActuatorMng.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [EOTActuatorMng — End_of_Travel_Actuator_Management_MDD](./EOTActuatorMng-End_of_Travel_Actuator_Management_MDD/) | `EOTActuatorMng/doc/End_of_Travel_Actuator_Management_MDD.docx` |

*Repository path: `EOTActuatorMng/`* 
