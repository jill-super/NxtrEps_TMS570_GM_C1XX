---
title: "SF47_TSMit_Implementation"
description: "SF47_TSMit_Implementation: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_TSMit).*
## Purpose and responsibility
Documented behaviour (first paragraph of the module design description):

> title: "SF47_TSMit_Implementation — TSMit_Integration_Manual"

## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_TSMit.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_TSMit.arxml` |
| Generation templates | `Ap_TSMit_Cfg.arxml.tt`, `Ap_TSMit_Cfg.h.tt`, `Ap_TSMit_Generate.bat`, `Ap_TSMit_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (25 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Pim_TSMitDisableEOL` | RTE-generated symbol |
| `Rte_Pim_TSMitGainLrn` | RTE-generated symbol |
| `Rte_Call_SystemTime_GetSystemTime_mS_u32` | RTE-generated symbol |
| `Rte_Call_TSMitGainLrn_SetRamBlockStatus` | RTE-generated symbol |
| `Rte_IRead_TSMit_Per1_HandwheelAuthority_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_TSMit_Per1_HandwheelPosition_HwDeg_f32` | RTE-generated symbol |
| `Rte_IRead_TSMit_Per1_HandwheelVelocity_HwRadpS_f32` | RTE-generated symbol |
| `Rte_IRead_TSMit_Per1_HwTorque_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_TSMit_Per1_PreLimitMtrTrqCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IRead_TSMit_Per1_SrlComABSActive_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_TSMit_Per1_SrlComESCActive_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_TSMit_Per1_SrlComTCSActive_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_TSMit_Per1_SrlComTransmissionTrq_TransNm_f32` | RTE-generated symbol |
| `Rte_IRead_TSMit_Per1_SrlComYawRate_DegpS_f32` | RTE-generated symbol |
| `Rte_IRead_TSMit_Per1_TSMitDefeat_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_TSMit_Per1_VehicleSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_IWrite_TSMit_Per1_TSMitCommand_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_TSMit_Per1_TSMitCommand_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWrite_TSMit_Per1_TSMitLearningEnabled_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_TSMit_Per1_TSMitLearningEnabled_Cnt_lgc` | RTE-generated symbol |
| `Rte_Call_SystemTime_DtrmnElapsedTime_mS_u16` | RTE-generated symbol |
| `Rte_Call_TSMit_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_TSMit_Per1_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_TSMitGainLrn_WriteBlock` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_TSMit_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_TSMit.h` `filters.h` `fixmath.h` `interpolation.h`
## Documents
| Document | Source file |
| --- | --- |
| [SF47_TSMit_Implementation — TSMit_Integration_Manual](./SF47_TSMit_Implementation-TSMit_Integration_Manual/) | `SF47_TSMit_Implementation/doc/TSMit_Integration_Manual.docx` |
| [SF47_TSMit_Implementation — Torque_Steer_Mitigation_MDD](./SF47_TSMit_Implementation-Torque_Steer_Mitigation_MDD/) | `SF47_TSMit_Implementation/doc/Torque_Steer_Mitigation_MDD.docx` |

*Repository path: `SF47_TSMit_Implementation/`* 
