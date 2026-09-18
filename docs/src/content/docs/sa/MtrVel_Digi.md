---
title: "MtrVel_Digi"
description: "MtrVel_Digi: purpose, files, API and documents (Sensor / Actuator Abstraction)."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-Cs (Sa_MtrVel/2/3).*
## Purpose and responsibility
Documented behaviour (first paragraph of the module design description):

> description: "Converted .docx document from MtrVel_Digi/doc."

## Key files
| Area | Files |
| --- | --- |
| `src/` | `Sa_MtrVel.c`, `Sa_MtrVel2.c`, `Sa_MtrVel3.c` |
| `include/` | `Sa_MtrVel.h` |
| AUTOSAR model | 6 `.arxml` file(s), e.g. `Sa_MtrVel.arxml` |
| Generation templates | `Sa_MtrVel2_Cfg.arxml.tt`, `Sa_MtrVel2_Cfg.h.tt`, `Sa_MtrVel2_Generate.bat`, `Sa_MtrVel2_bswmd.arxml`, `Sa_MtrVel_Cfg.arxml.tt`, `Sa_MtrVel_Cfg.h.tt` |
## Public API
Top RTE/component symbols referenced in the sources (37 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_IRead_MtrVel_Per1_AsstAssemblyPolarity_Cnt_s08` | RTE-generated symbol |
| `Rte_IRead_MtrVel_Per1_MechMtrPos2Timestamp_USec_u32` | RTE-generated symbol |
| `Rte_IRead_MtrVel_Per1_MechMtrPos2_Rev_u0p16` | RTE-generated symbol |
| `Rte_IWrite_MtrVel_Per1_HandwheelVel_HwRadpS_f32` | RTE-generated symbol |
| `Rte_IWriteRef_MtrVel_Per1_HandwheelVel_HwRadpS_f32` | RTE-generated symbol |
| `Rte_IWrite_MtrVel_Per1_MotorVelCRF_MtrRadpS_f32` | RTE-generated symbol |
| `Rte_IWriteRef_MtrVel_Per1_MotorVelCRF_MtrRadpS_f32` | RTE-generated symbol |
| `Rte_IWrite_MtrVel_Per1_MotorVelMRF_MtrRadpS_f32` | RTE-generated symbol |
| `Rte_IWriteRef_MtrVel_Per1_MotorVelMRF_MtrRadpS_f32` | RTE-generated symbol |
| `Rte_IWrite_MtrVel_Per1_SysCHandwheelVel_HwRadpS_f32` | RTE-generated symbol |
| `Rte_IWriteRef_MtrVel_Per1_SysCHandwheelVel_HwRadpS_f32` | RTE-generated symbol |
| `Rte_IWrite_MtrVel_Per1_SysCMotorVelMRF_MtrRadpS_f32` | RTE-generated symbol |
| `Rte_IWriteRef_MtrVel_Per1_SysCMotorVelMRF_MtrRadpS_f32` | RTE-generated symbol |
| `Rte_Call_MtrVel_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_MtrVel_Per1_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_IRead_MtrVel_Per2_SysCDiagHwVel_HwRadpS_f32` | RTE-generated symbol |
| `Rte_IRead_MtrVel_Per2_SysCDiagMtrVelMRF_MtrRadpS_f32` | RTE-generated symbol |
| `Rte_IWrite_MtrVel_Per2_HwVelValid_Cnt_lgc` | RTE-generated symbol |
| `Rte_IWriteRef_MtrVel_Per2_HwVelValid_Cnt_lgc` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_GetNTCFailed` | RTE-generated symbol |
| `Rte_Call_NxtrDiagMgr_SetNTCStatus` | RTE-generated symbol |
| `Rte_Call_MtrVel_Per2_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_MtrVel_Per2_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_IRead_MtrVel2_Init_CumMechMtrPosMRF_Deg_f32` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`CalConstants.h` `Float.h` `GlobalMacro.h` `MemMap.h` `MtrVel_Cfg.h` `Rte_Sa_MtrVel.h` `Rte_Sa_MtrVel2.h` `Rte_Sa_MtrVel3.h` `Sa_MtrVel.h` `Sa_MtrVel2_Cfg.h` `Sa_MtrVel_Cfg.h` `Std_Types.h` `filters.h` `fixmath.h` `float.h` `interpolation.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`CalConstants.h` `Compiler_Cfg.h` `MemMap.h` `MtrVel_Cfg.h` `Sa_MtrVel` `Rte.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Sa_MtrVel.h` `Rte_Type.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [MtrVel_Digi — Motor Velocity_Integration_Manual](./MtrVel_Digi-Motor-Velocity_Integration_Manual/) | `MtrVel_Digi/doc/Motor Velocity_Integration_Manual.docx` |
| [MtrVel_Digi — MotorVelocity2_MDD](./MtrVel_Digi-MotorVelocity2_MDD/) | `MtrVel_Digi/doc/MotorVelocity2_MDD.doc` |
| [MtrVel_Digi — MotorVelocity3_MDD](./MtrVel_Digi-MotorVelocity3_MDD/) | `MtrVel_Digi/doc/MotorVelocity3_MDD.doc` |
| [MtrVel_Digi — MotorVelocity_MDD](./MtrVel_Digi-MotorVelocity_MDD/) | `MtrVel_Digi/doc/MotorVelocity_MDD.doc` |

*Repository path: `MtrVel_Digi/`* 
