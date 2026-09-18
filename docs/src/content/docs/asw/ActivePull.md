---
title: "ActivePull"
description: "ActivePull: purpose, files, API and documents (Application Software (ASW))."
---

:::note[Custom — Nexteer in-house]
In-house developed module. RTE contract stubs (`utp/contract`, `tools/contract`) and DaVinci/RTE artefacts referenced by this module are Vector-generated and are not part of the module sources.
:::
*Origin: **Custom** — Nexteer in-house SW-C (Ap_ActivePull).*
## Purpose and responsibility
Software area `ActivePull` in the GM C1XX EPS firmware. See the key files and linked design documents below for normative behaviour.
## Key files
| Area | Files |
| --- | --- |
| `src/` | `Ap_ActivePull.c` |
| AUTOSAR model | 4 `.arxml` file(s), e.g. `Ap_ActivePull.arxml` |
| Generation templates | `Ap_ActivePull_Cfg.arxml.tt`, `Ap_ActivePull_Cfg.h.tt`, `Ap_ActivePull_Generate.bat`, `Ap_ActivePull_bswmd.arxml` |
## Public API
Top RTE/component symbols referenced in the sources (24 unique in total):
| Symbol | Kind |
| --- | --- |
| `Rte_Mode_SystemState_Mode` | RTE-generated symbol |
| `Rte_IRead_ActivePull_Per1_DisableLearning_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_ActivePull_Per1_DisableOutput_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_ActivePull_Per1_HandwheelAuthority_Uls_f32` | RTE-generated symbol |
| `Rte_IRead_ActivePull_Per1_HandwheelPosition_HwDeg_f32` | RTE-generated symbol |
| `Rte_IRead_ActivePull_Per1_HandwheelVelocity_HwRadpS_f32` | RTE-generated symbol |
| `Rte_IRead_ActivePull_Per1_HwTorque_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_ActivePull_Per1_SrlComYawRate_DegpS_f32` | RTE-generated symbol |
| `Rte_IRead_ActivePull_Per1_VehicleSpeedValid_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_ActivePull_Per1_VehicleSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_Call_SystemTime_DtrmnElapsedTime_mS_u32` | RTE-generated symbol |
| `Rte_Call_SystemTime_GetSystemTime_mS_u32` | RTE-generated symbol |
| `Rte_Call_ActivePull_Per1_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_ActivePull_Per1_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_IRead_ActivePull_Per2_DisableOutput_Cnt_lgc` | RTE-generated symbol |
| `Rte_IRead_ActivePull_Per2_VehicleSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_IWrite_ActivePull_Per2_PullCompCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_IWriteRef_ActivePull_Per2_PullCompCmd_MtrNm_f32` | RTE-generated symbol |
| `Rte_Call_ActivePull_Per2_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_ActivePull_Per2_CP1_CheckpointReached` | RTE-generated symbol |
| `Rte_IRead_ActivePull_Per3_HwTorque_HwNm_f32` | RTE-generated symbol |
| `Rte_IRead_ActivePull_Per3_VehicleSpeed_Kph_f32` | RTE-generated symbol |
| `Rte_Call_ActivePull_Per3_CP0_CheckpointReached` | RTE-generated symbol |
| `Rte_Call_ActivePull_Per3_CP1_CheckpointReached` | RTE-generated symbol |
## Usage and dependencies
Selected project headers included by this module:
`Ap_ActivePull_Cfg.h` `CalConstants.h` `GlobalMacro.h` `MemMap.h` `Rte_Ap_ActivePull.h` `filters.h` `fixmath.h` `interpolation.h`

Vector-generated RTE contract stubs used for unit testing (in `utp/contract/`, not shipped):
`Ap_ActivePull_Cfg.h` `CalConstants.h` `Compiler_Cfg.h` `MemMap.h` `Rte.h` `Rte_Ap_ActivePull.h` `Rte_Compiler_Cfg.h` `Rte_MemMap.h` `Rte_Type.h`

Unit-test artefacts live in `utp/` (Tessy reports — see [Unit-test reports](../general/unit-test-reports/).
## Documents
| Document | Source file |
| --- | --- |
| [ActivePull — Active_Pull_Comp_MDD](./ActivePull-Active_Pull_Comp_MDD/) | `ActivePull/doc/Active_Pull_Comp_MDD.docx` |

*Repository path: `ActivePull/`* 
